# RAG_BedRock
There is a lot of investment information in the 10-K. However, human's ability to read through all documents is pretty slow compared to machines. This is an example QA app to help information retrieval. 

## Package usage 
- LangChain
- Pinecone Vector DB
- Amazon Titan model 
- Amazon Bedrock  

## Steps 
- Prepare 10-K documents
- Chunks
- Create embedding using the Amazon Bedrock Titan Embeddings model
- Save it in vectorDB Pinecone
- When the user inputs a request
- Make requests into embedding vectors
- Find the document(s) relevant to the question being asked
- Feed it to LLM with prompt
- Finally, return the answer with the document source. 
