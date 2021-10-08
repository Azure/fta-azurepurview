## Delivery guidance

This delivery guidance is for FastTrack for Azure engineers to deliver FTA Live for Purview sessions, to identify dedicated FTA data governance project down the road. 

### Top questions to ask: 
Some example questions that you may run into during the initial phase:
1.	What are the main organization data sources and data systems?
2.	Who are the users?
3.	How to integrate with existing systems?
4.	How to integrate the platform with existing critical assets, glossary terms, and contacts?

### Identify key scenarios: 
These scenarios can cross business unit boundaries or impact multiple user personas either upstream or downstream, so suggest including at least these five dimensions:
1.	Persona – Who are the users?
2.	Source system – What are the data sources such as Azure Data Lake Storage Gen2 or Azure SQL Database?
3.	Impact Area – What is the category of this scenario?
4.	Detail scenarios – How the users use Purview to solve problems?
5.	Expected outcome – What is the success criteria?

### Some example scenarios that you can use:

| Scenario| Detail| Persona |
|-----  |-----|---------- |
| Catalog business-critical assets|I need to have information about each data sets to have a good understanding of what it is. This scenario includes both business and technical metadata data about the data set in the catalog. The data sources include Azure Data Lake Storage Gen2, Azure Synapse DW, and/or Power BI. This scenario also includes on-premise resource such as SQL Server.	| Business Analyst, Data Scientist, Data Engineer|
|Discover business-critical assets| I need to have a search engine that can search through all metadata in the catalog. I should be able to search using technical term, business term with either simple or complex search using wildcard.	| Business Analyst, Data Scientist, Data Engineer, Data Admin| 
| Track data to understand its origin and troubleshoot data issues	| I need to have data lineage to track data in reports, predictions, or models back to its original source and understand the changes and where the data has resided through the data life cycle. This scenario needs to support prioritized data pipelines Azure Data Factory and Databricks.	| Data Engineer, Data Scientist| 
| Enrich metadata on critical data assets	| I need to enrich the data set in the catalog with technical metadata that is generated automatically. Classification and labeling are some examples.	| Data Engineer, Domain/Business Owner| 
| Govern data assets with friendly user experience| 	I need to have a Business glossary for business-specific metadata. The business users can use Purview for self-service scenarios to annotate their data and enable the data to be discovered easily via search.	| Domain/Business Owner, Business Analyst, Data Scientist, Data Engineer|


### Include the right stakeholders: 
To ensure the success of implementing Purview for the entire enterprise, it’s important to involve the right stakeholders.  Some key stakeholders that you may want to include:


|Persona|Roles|
|-----  |-----|
|Chief Data Officer| The CDO oversees a range of functions that may include data management, data quality, master data management, data science, business intelligence, and creating data strategy. They can be the sponsor of the Purview implementation project.|
|Domain/Business Owner	| A business person who influences usage of tools and has budget control|
| Data Analyst	| Able to frame a business problem and analyze data to help leaders make business decisions|
|Data Architect	| Design databases for mission-critical line-of-business apps along with designing and implementing data security| 
| Data Engineer	| Operate and maintain the data stack, pull data from different sources, integrate and prepare data, set up data pipelines|
| Data Scientist|	Build analytical models and set up data products to be accessed by APIs|
| DB Admin|	Own, track, and resolve database-related incidents and requests within service-level agreements (SLAs); May set up data pipelines|
|DevOps	| Line-of-Business application development and implementation; may include writing scripts and orchestration capabilities|
|Data Security Specialist	| Assess overall network and data security, which involves data coming in and out of Purview|

