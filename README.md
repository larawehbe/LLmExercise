# LLmExercise
This repository serves as a descrption for the exercise. 

It will include two versions. Choose anyone of them that is more suitable for you.

## Objective:

In this exercise, you have deeper understanding of Large Language Models, Vector Datababse, and RAG Architecture.
You need to use RAG, with any open-source llm of your choice, and an opensource dataset, saved in a vector db.

## Technologies:
- LLM: Use **Ollama**, it is a tool that facilitates downloading open source llms such as llama2, llama3, phi, mistral, and others. **While it's best case scenario to use ollama, you can use other models from huggingface as an example, stating WHY YOU DIDN'T USE OLLAMA**.
- **Hugging Face:** Hub of NLP. 1 Million open-source models, and many more open-source datasets. You can use for text embedding models, and open-source datasets to feed to RAG
- **Vector Database:** Here's a list of open source vector dbs you can use: Chromadb (best option, recommended), FAISS. These are the main two. feel free to use any other one
- **Langchain:** Framework to chain LLm, VectorDB, and RetrievalQA Chain. **I CAN'T STRESS THIS ENOUGH, DEVELOPING WITH LANGCHAIN IS A GEM**
- **Python:**. obvious no?. 

You are expected to:
- Find an online open source dataset
- Add this data to a vector database. Use Langchain text splitter and add them to vector database.
- Adding data to vector database requires you to use an embedding model. I would suggest you use anyone from hugging face.
- Use ollama to download an open source model. make sure to choose a model of 7B (7billion) parameters only, to avoid cpu crashing. Also, you can use phi model from ollama for low storage (i tested on it).


