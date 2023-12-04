# ANU Scholarly KG (ASKG) for UniverseTBD: `ASKG4UTBD`

---
## Participants

Students:  
- (2022-S2) Bowen Zhang  
- (2023-S2) Runsong Jia  

Supervisors:  
- Dr. Sergio J. Rodríguez Méndez 
- Dr. Pouya Ghiasnezhad Omran 

---
## Project Description:
The goal of this project is to build and evolve a proof of concept of an academic Knowledge Graph (KG) for ANU researchers (*ASKG – ANU Scholarly KG*) by using, testing, and improving a set of existing tools named **KGCP**, that have been developed by the *KG Engineering Team (KGET)* at the School of Computing.  
  
Under UniverseTBD's scope, we are replicating the construction process and structure of *ASKG* in creating a similar KG for 1,000 astronomy papers.  We call this KG, *ASKG4UTBD*.  
  
KGCP stands for *“Knowledge Graph Construction Pipeline”* and it consists of several tools, such as:
- [**MEL**](https://w3id.org/kgcp/MEL-TNNT): Metadata Extractor & Loader; metadata extraction and pre-processing pipeline component. [KGC Tutorial 2022 demo video](https://youtu.be/hWMZ1O-PSjE) 
- [**g0-Builder + J2RM**](https://w3id.org/kgcp/J2RM): Initial graph (g0) creation component with a *JSON-2-RDF Mappings* annotations tool for domain-ontologies.  [KGC Tutorial 2022 demo video](https://youtu.be/F3CGGby74OM) 
- [**TNNT**](https://w3id.org/kgcp/MEL-TNNT): The NLP/NER (_Named Entity Recognition_) Toolkit; supports 9 tools and 21 models.  [KGC Tutorial 2022 demo video](https://youtu.be/D4DEULn8EtU) 
- **KG-I**: _KG Integration_ package. 
  
ASKG structure includes basic and public information about ANU researchers (*researchers.anu.edu.au*), grants (*ANDS* Web Service), and publications (research papers).  
Several external data sources will be used to enrich the KG (matching and adding entities), such as:
- Microsoft Academic Knowledge Graph.  
- The Microsoft Academic API.  
- Scholarly Data.  
- Wikidata, etc.  
  
From the data and model perspective, there are multiple problems to solve. Firstly, the initial version of the Web crawler (and data collector) needs to be created/extended to add more online data sources, with several improvements to make its structure easy to maintain and extensible.  
Next, the data from the new sources should be cleaned (pre-processed) and merged. For this, various algorithms will be designed, tested, and improved.  
Afterwards, the existing ASKG ontology will be built, revised, and evolved (adding new concepts and relationships), along with the necessary mappings to enrich and evolve the KG.  
During the KG construction process, the **KGCP** toolkit will be used, especially the **KG-I**, to enrich the data graph with external KGs such as Wikidata.  
Finally, various SPARQL queries will be designed to statistically analyse the final KG structure.  
  
The following are the various tools that will be used for this project: 
- Python is the primary programming language using various packages such as **RDFLib**, **BeautifulSoap**, and **Requests**.  
- **MEL** and **TNNT** will help extract content and keywords from research papers that will be analysed to enrich ASKG.  
- **J2RM** will be used to design the necessary JSON-to-RDF mappings to construct the KG.  
- **KG-I** will be used to expand and enrich the initial KG with external KGs and sources (research papers).  
- **Protégé** is a powerful **OWL2** Ontology editor that will be used to edit and manage the ASKG ontology.  
- **Cmap Tool** will be used for ontology modelling.  
- **SPARQL** is the query language for RDF-based graphs; it will be used to query the final ASKG.  

---
## Semantic Web & Knowledge Graphs Technologies and Tools
Below is a none-comprehensive list of various technologies and tools that we will use for the project: 

### Technologies
- Understanding the concepts "URI" (IRIs) and "Resource": [Architecture of the World Wide Web, Volume One](https://www.w3.org/TR/webarch/) 
- An overview of the Semantic Web Technology Stack: [SWTS](https://sjrm.medium.com/isoc-w3c-standards-in-the-internet-ecosystem-8cbaf919f73c) | [W3C Standards Overview (by Sergio Rodríguez Méndez).pdf](https://anu365-my.sharepoint.com/:b:/g/personal/u1085404_anu_edu_au/EVRbWWfgxqVAv61KIsD4mRYB7pyf6t-4VQPr4StrCL7M2Q?e=sHW3q7) 
- Resource Description Framework: [RDF 1.1 Primer](https://www.w3.org/TR/rdf11-primer/) 
- Other high-level concepts to "know about": RDFS, OWL2, and SPARQL (see the second item) 
- Terse RDF Triple Language: [RDF 1.1 Turtle](https://www.w3.org/TR/turtle/) 

### Tools
- Graph modeling: [IHMC Cmap Tool](https://cmap.ihmc.us/) 
- OWL2 Ontology Editor: [Protégé](https://protege.stanford.edu/) 
- RDFLib Python Library: [RDFLib](https://rdflib.dev/) 

---
## Related Papers

The following papers are good to get familiar with the domain: 

[1] A. Hogan et al., “*Knowledge Graphs*”, arXiv Prepr., 2020, http://arxiv.org/abs/2003.02320.  
[2] Z. Zhao, S.-K. Han, and I.-M. So, “*Architecture of Knowledge Graph Construction Techniques*”, Int. J. Pure Appl. Math., vol. 118, no. 19, pp. 1869–1883, 2018.  
[3] I. Mondal, Y. Hou, and C. Jochim, “*End-to-End Construction of NLP Knowledge Graph*”, in Findings of the Association for Computational Linguistics: {ACL/IJCNLP} 2021, Online Event, August 1-6, 2021, 2021, pp. 1885–1895, doi: 10.18653/v1/2021.findings-acl.165.  
[4] Cheng Deng, Yuting Jia, Hui Xu, Chong Zhang, Jingyao Tang, Luoyi Fu, Weinan Zhang, Haisong Zhang, Xinbing Wang, Chenghu Zhou. *GAKG: A Multimodal Geoscience Academic Knowledge Graph*. CIKM 2021: 4445-4454.  

---
*$Last Update: 2023-12-04$*  
