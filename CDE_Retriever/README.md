# Explanation of files

Data files:
- SearchExport.json is a download from https://cde.nlm.nih.gov/cde/search site which offers json, CSV, or xml format.  This is an 86Mb file.
- SearchExport.csv is much smaller but only includes a small fraction of the fields.  It is not adequate to provide sufficient information to CDM.
- output.csv is created by one of my notebooks by parsing the JSON file and selecting fields of interest.
  
Jupyter notebooks:
- RetrieveJsonElements.ipynb contains code that parses SearchExport.json to pull relevant deta from the file and populates a new csv file called output.csv; this is basically similar to the version from NIH but has additional fields that I think have semantic relevance.
- CDE_Lookup.ipynb has code that reads the output.csv file, splits it into over 20,000 documents (one per line), and then uses an embedding model to vectorize each document, and then we stick it in Chroma (a reasonable vector database), and then sets up a way to ask for data elements.

Right now app.py is empty.  My plan is to create a ChainLit application that you can run locally (chainlit run app.py), or that can be
dockerized and then loaded onto HuggingFace or on our premises.  Since this particular application contains no intellectual property of value to us,
I think putting it on HF is not terrible, but since this will access OpenAI, will create a private space on HF that is only open to our organization.

To see the rough structure, I have another folder (DeployPythonicRAG) that includes a RAG application that you can run locally or you could try to run 
on our premises using Docker.
