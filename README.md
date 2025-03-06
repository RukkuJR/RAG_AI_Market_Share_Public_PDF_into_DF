# RAG_AI_Market_Share_Public_PDF_into_DF

![image](https://github.com/user-attachments/assets/91cb0cc5-de06-4a4c-b2b6-a3f78ac3179b)

This is A POC on doing RAG(Retrieval Generation Augmentaion) for internal Data.

Use Case:

Imagine we want to do market share comparison between our brand vs the others? Who's leading in the market. 
For this ussualy we buy data eg sample sales data from Nielson, DunnHumby on periodical basis on subscription than integrate into our datapiple into insigts.

POC:

Now RAG is available. We could just scrape available public data online. Best Eg would be Yearly Annual Results PDF's of pubic listed companies.
These Data we could ingest into VectorDB than let LLM do its magic using natural language and store into a DataFrame for future use cases. Eg ingesetion into RDMBS, Integration with other central sources.

![image](https://github.com/user-attachments/assets/fed09bea-2f76-4169-b65b-351c21d61496)


The text from these PDF could be  extracted and then split into multiple chunks and then be loaded into Vector Databases(interms of embeeddings). These are neccesary to do nearby searches using natural language later.


![image](https://github.com/user-attachments/assets/0331e079-9350-4835-9014-bb36967b79d8)

The Above is sample architecture but the process remains the same

1)Load & Preprocess PDFs

2)Embed & Store Data in ChromaDB

3)Extract sales trends using LLaMA 3.2 via ollama

4)Store the extracted values in a Pandas DataFrame dynamically for future use cases

Output
------
![image](https://github.com/user-attachments/assets/d5d918e5-c4c4-495e-b3c2-6909caf2f9fb)
![image](https://github.com/user-attachments/assets/2d323292-8f50-49b0-9e37-a677470e3829)
![image](https://github.com/user-attachments/assets/22b4a356-6241-477b-897f-774807ad07d8)
![image](https://github.com/user-attachments/assets/feeb4197-d177-49d7-947b-62c1446dbca4)






