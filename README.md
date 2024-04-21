# Dio-Azure-Lab04
Pesquisa cognitiva do Azure

In this lab, I should create Azure resources, extract data from a data source,
enrich data with AI skills, use Azure’s indexer in the Azure portal
query the search index, and review results saved to a Knowledge Store.

I created three resources for the lab: 

* An Azure AI Search resource to manage indexing and querying.
* An Azure AI services resourceto provide AI services for skills that can be used to enrich the data in the data source with AI-generated insights.
* A Storage account with blob containers, which will store raw documents and other collections of tables, objects, or files.

The next step is uploading the documents to Azure Storage.

In the Azure portal there is the Import data wizard that automatically create an index and indexer for supported data sources.

I attached Cognitive Services, added enrichments and I saved enrichments to a knowledge store

In the search explorer, you can edit a JSON file with 
{
"search": "*",
    "count": true
    }
to get all the index you have chosen. 

<img src="https://github.com/vverdum/Dio-Azure-Lab04/assets/157656254/2799c057-4fa5-4bb5-a6eb-c672a02ff9ec" width="600" height="300">

By the way, if we edit JSON with
{
 "search": "locations:'Chicago'",
 "count": true
}
we can obtain all times Chicago appears in the analyzed data. 


![image](https://github.com/vverdum/Dio-Azure-Lab04/assets/157656254/e61f4109-cdfd-4e09-a1e3-79ac14fb58e9)

Inside the knowledge store, I have found the enriched data extracted by AI skills  in the form of projections and tables.


![image](https://github.com/vverdum/Dio-Azure-Lab04/assets/157656254/60b6f54f-c598-4c70-b70b-6e7ac110836f)

I have selected the table coffeeSkillsetKeyPhrases to see all the content captured in the reviews. As many of the fields are keys, it is possible to link the tables like a relational database. The last field shows the key phrases that were extracted by the skillset.

![image](https://github.com/vverdum/Dio-Azure-Lab04/assets/157656254/70a6125f-d1a1-4237-acbf-154da6456ba3)

