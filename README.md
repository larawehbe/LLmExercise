# LLmExercise
This repository serves as a descrption for the exercise. 


## Objective:

In this exercise, you have deeper understanding of Large Language Models, Vector Datababse, and RAG Architecture.
You need to use RAG, with any open-source llm of your choice, and any open-source dataset, saved in a vector db.

## Technologies:
- LLM: Use **Ollama**, it is a tool that facilitates downloading open source llms such as llama2, llama3, phi, mistral, and others. **While it's best case scenario to use ollama, you can use other models from huggingface as an example, stating WHY YOU DIDN'T USE OLLAMA**.
- **Hugging Face:** Hub of NLP. 1 Million open-source models, and many more open-source datasets. You can use for text embedding models, and open-source datasets to feed to RAG
- **Vector Database:** Here's a list of open source vector dbs you can use: Chromadb (best option, recommended), FAISS. These are the main two. feel free to use any other one
- **Langchain:** Framework to chain LLm, VectorDB, and RetrievalQA Chain. **I CAN'T STRESS THIS ENOUGH, DEVELOPING WITH LANGCHAIN IS A GEM**
- **Python:**. obvious no?. 

### Here are some ideas:
- Develop an LLM with RAG to answer FAQ. These FAQ will be passed first as PDF, loaded and splitted using langchain, saved in a vector database. Then this vectordb will be used as a retreiver, linked to a RetrievalQAChain also from langchain (This step requires LLM, you need to do your research), then the user can ask questions to this model, it should answer from these FAQ.
- Developm an LLM with RAG to answer questions from any given PDF, say its a research paper and you want to extract information from it without reading it all. Take this question for example: "What is the methodology used in this paper?", using RAG implemented by langchain, you should be able to answer this question from your pdf.
- I think you got the idea now.


You are expected to:
- Prepare dataset (Option 1: easy). A List of PDFs 
- Prepare dataset (Option 2: intermediate-harder than 1). Find a dataset online (ex: from huggingface), or scrape data (ex: from reddit, using reddit api). 
- Add this data to a vector database. Use Langchain text splitter and add them to vector database.
- Adding data to vector database requires you to use an embedding model. I would suggest you use anyone from hugging face.
- Use ollama to download an open source model. make sure to choose a model of 7B (7billion) parameters only, to avoid cpu crashing. Also, you can use phi model from ollama for low storage (i tested on it).
- Use langchian to load model ( whether model from llama, ollama, or hugging face), retreive data from vectordb, and retreival chains for QA.

### Bonus points: ( points are not necessarily in priority order)
- Wrap it in Gradio for user interface
- Create a conversational chat chain, and not a retreivalqa chain, where user can interact with the data source, and not only ask one question
- Use FlaskAPI to wrap it in an API with POST Request.
- Write a small report: Difference between finetuning and RAG architecture, Procs and cons, when do we use what, and why.
- Apply finetuning ( if needed ) before RAG 

## Resources:
