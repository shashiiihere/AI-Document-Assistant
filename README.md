# AI-Document-Assistant

We leverage the Retrieval Augmented Generation (RAG) methodology to create a user-centric and intelligent system that enhances information retrieval from PDF documents through natural language queries.

1. Input: RAG takes multiple pdf as input.
2. VectoreStore: The pdf's are then converted to vectorstore using FAISS and all-MiniLM-L6-v2 Embeddings model from Hugging Face.
3. Memory: Conversation buffer memory is used to maintain a track of previous conversation which are fed to the llm model along with the user query.
4. Text Generation with GPT-3.5 Turbo: The embedded input is fed to the GPT-3.5 Turbo model from the OpenAI API, which produces the final output.
5. User Interface: Streamlit is used to create the interface for the application.
