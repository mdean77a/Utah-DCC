# Explanation of Repository
This is a private repository for developing apps for the UU Data Coordinating Center.

The CDE_Retriever folder will / does contain files for the first app I am developing in my class.  It will
allow downloading the entire repository from the NIH in JSON format, extraction of relevant portions of the download into a CSV file, 
and then chunk the CSV file prior to vectorization.  Then the chat application will allow the CDM to enter the data element and get a download of relevant data elements, with most of the parameters, and including a live web link to the element in the NLM repository.

The grants, guidelines, and protocols folders contain documents that we can use to experiment with development of other apps.

The notebooks folder contains interesting Jupyter notebooks that illustrate something that may be useful in our development efforts.
I get these from the AIM bootcamp or other courses, and most of them were originally run in Colab, so they can easily be run there.  Otherwise, I run them in a local Jupyter environment on my own machines.

## Who are our customers?
The DCC assists three different audiences:
1.  Investigators in networks for which we are the funded DCC.  We are obliged to work with these investigators from their initial idea, through development of a draft protocol and grant proposal that is then submitted to the NIH, CDC, or other Federal agencies.
2.  Investigators who are **not** inside one of our funded activities, but have heard of our services.  We usually are brought in at the pre-grant submission phase similar to the network investigators, but we are **not** obliged to take their projects on.  In general, we try to help these investigators because it increases our reputation.  In addition, if investigators are from within the University of Utah, there are obvious pressures to help them simply because of citizenship.
3.  Industry related trials come from small startup drug or device manufacturers, or might come from clinical research organizations (CRO) who already have a protocol and simply want a DCC.  In the case of small start up companies, they often need assistance with trial design, etc., similar to investigators listed earlier.  But more often, the protocol is already final, and they want implementation.  This category of customer is important to us financially to offset losses that we incur on NIH and other Federal grants.
    
## Project Ideas for Data Coordinating Center (DCC) Apps
### Very LOW Hanging Fruit Projects
- Put all our documents from DCC into vector database and build a simple chat app that will allow
access to all our corporate knowledge.  How do we scrape our eRoom, OneNote, and SharePoint instances.  
- Could start with the DCC web site - crawl and scrape, and then there is access to what we offer.
### Grant preparation
Ideas about improving grants.
### Tasks after grant is funded
Ideas about tasks
### Potential projects
- CDE retrieval application - CDM provides data element, or a list of data elements, and application retrieves from CDE repository, including a link that will allow CDM to directly read information from NIH repository web pages.
- application that accepts grant materials and produces a draft protocol
- grant improvement apps that can read specific aim pages, research narratives, and biosketches, and can suggest improvements or identify inconsistencies.
- application that accepts grant narratives and produces a timeline for inclusion
- application that can identify data elements in a protocol and outputs a listing
- application that can create a RedCAP database automatically from a protocol
- application to produce training materials, quiz questions, etc.
