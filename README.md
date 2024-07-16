# Semantic Chunking for RAG
LLMs are bound to hallucinate and then we have different strategies to mitigate this hallucination behaviour of LLMs. One such strategy is Retrieval Augmented Generation (RAG), where a knowledge base is already augmented/provided to the LLM to retrieve the information from and this way LLMs won't hallucinate since the knowledge base is already specified.
RAG involves a step by step process of loading the documents/data, splitting the documents into chunks using any AI framework such as LangChain or LlamaIndex, and vector embeddings generation for the data and storing these embeddings in a vector database.

So, broadly we can devide the RAG into two main parts, Storing and Retrieval. 

While enahncing our RAG pipeline, one thing we need to looak at is the retriavl strategy and technoques involved. We can improve retrieval in RAG using the proper chunking strategy. But finding the right chunk size for any given text is a very hard question in general.

Today, we will see how semantic chunking works. Semantic Chunking considers the relationships within the text. It divides the text into meaningful, semantically complete chunks. This approach ensures the information’s integrity during retrieval, leading to a more accurate and contextually appropriate outcome.

Let's experiment with Semantic chunking & see the results

## Tech Stack Used
### LangChain - Open source AI framework to load, split and to create embeddings of the data
### SingleStore - As a robust vector database to store vector embeddings. [Sign up & get a free account](https://www.singlestore.com/cloud-trial/?utm_medium=referral&utm_source=pavan&utm_term=yt&utm_content=semRAG).
### Groq and HuggingFace - To choose our LLMs and embedding models

If you like this content, I am sure you are going to love my other AI/ML/Data related content too. 
I create tutorials on my YouTube channel on different AI/ML/Data related concepts. [Subscribe to my YouTube channel](https://www.youtube.com/@pavanbelagatti)😊

#### Credits:
This tutorial is inspired by Plaban Nayak's [article on Medium](https://medium.com/the-ai-forum/semantic-chunking-for-rag-f4733025d5f5).
