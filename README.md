# RAGtime: Hybrid Search RAG System with LangChain and Pinecone

This project demonstrates a Retrieval Augmented Generation (RAG) system that combines semantic and keyword-based search to answer questions using a large language model (LLM).

## Features

* **Hybrid Search:**  Combines the power of dense vector embeddings (semantic search) and sparse vectors (BM25) for improved retrieval accuracy and flexibility.
* **Pinecone Vector Database:**  Efficiently stores and retrieves embeddings and metadata, enabling fast and scalable search capabilities.
* **LangChain Framework:** Streamlines the development of the RAG pipeline, integrating the LLM, retriever, and prompt templates.
* **Hugging Face Transformers:** Leverages state-of-the-art Hugging Face models for embeddings and language modeling.
* **SQuAD Dataset:** Uses the SQuAD dataset for training and evaluation of the question-answering capabilities.

## Setup

1. **Clone the Repository:**

   ```bash
   git clone [(https://github.com/WizKnight/RAGtime.git)]
   cd hybrid-search-rag-project

2. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt

3. **Set Up Environment Variables:**
   Create a .env file in the project root directory and add your API keys and other 
   credentials:

   ```bash
   PINECONE_API_KEY=your-pinecone-api-key
   PINECONE_ENV=your-pinecone-environment
   HF_TOKEN=your-hugging-face-api-token

4. **Run The Code:**
  * Data Processing, Embedding, and Upserting: Execute the relevant scripts or notebook cells to preprocess your data, generate embeddings, and upsert them into Pinecone.
  * Querying and Evaluation: Run the main.py script or the corresponding notebook cells to interact with the RAG system, ask questions, and evaluate its performance.

## Usage

1. **Ensure Data is Upserted:** Make sure you've run the data processing, embedding, and upserting steps to populate your Pinecone index.
2. **Run `main.py`:** Execute the `main.py` script to start the interactive query interface.
3. **Ask Questions:** Enter your questions at the prompt, and the system will retrieve relevant contexts and generate answers.

## Evaluation
* The project includes code to evaluate the system's performance using the SQuAD evaluation metric (Exact Match and F1 score).

## Customization
* **Dataset:** You can easily replace the SQuAD dataset with your own data by modifying the data loading and preprocessing steps.
* **Embedding Model:** Experiment with different Hugging Face embedding models by changing the `model_name` in the code.
* **LLM:** Explore various Hugging Face LLMs for question answering by adjusting the `repo_id`.
**Retrieval Parameters:** Fine-tune the retrieval process by adjusting the `top_k` parameter or experimenting with different hybrid search weighting strategies.

## License
This project is licensed under the Apache 2.0 License.




