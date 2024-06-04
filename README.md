# RAG with Jina Embeddings and LlamaIndex

This repo contains a notebook that guides you through the process of using Jina Embeddings V2 in a retrieval augmented generation pipeline.
It uses the model `jinaai/jina-embeddings-v2-base-de` from HuggingFace, which is a bilingual German-English embedding model trained by Jina AI.

Install the requirements in `requirements.txt` in a fresh environment.

To run the notebook `rag.ipynb`, it is also necessary to host a service that serves a (small) large language model. You can do this on an ordinary local machine without GPUs using [ollama](https://github.com/ollama/ollama). To setup such a service:

1. Follow the installation instruction for [ollama](https://github.com/ollama/ollama)
2. Pull the mistral (or any other small) LLM model using `ollama pull mistral`
3. Start a service by running `ollama serve`

Now you can execute all blocks in the notebook.

**Disclaimer**: The data in the `data/` folder was generated using GPT4 for the purpose of demonstrating the RAG pipeline on unseen, "private" data.