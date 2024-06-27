# MultiQueryRetriever

<img width="946" alt="image" src="https://github.com/AshishCodeCraft26/RAG-MultiQueryRetriever/assets/135592934/e36ae018-48f0-45e6-9e8f-d240e783a4ec">

<br>

Distance-based vector database retrieval embeds (represents) queries in high-dimensional space and finds similar embedded documents based on "distance".
But, retrieval may produce different results with subtle changes in query wording or if the embeddings do not capture the semantics of the data well. 
Prompt engineering / tuning is sometimes done to manually address these problems, but can be tedious.

The <code>MultiQueryRetriever</code> automates the process of prompt tuning by using an LLM to generate multiple queries from different perspectives 
for a given user input query. For each query, it retrieves a set of relevant documents and takes the unique union across all queries to get a 
larger set of potentially relevant documents. By generating multiple perspectives on the same question, 
the <code>MultiQueryRetriever</code> might be able to overcome some of the limitations of the distance-based retrieval and get a richer set of results.

Docs:
https://python.langchain.com/v0.1/docs/modules/data_connection/retrievers/MultiQueryRetriever/




