# AI-Document-Assistant

Input: RAG takes multiple pdf as input.
VectoreStore: The pdf's are then converted to vectorstore using FAISS and all-MiniLM-L6-v2 Embeddings model from Hugging Face.
Memory: Conversation buffer memory is used to maintain a track of previous conversation which are fed to the llm model along with the user query.
Text Generation with GPT-3.5 Turbo: The embedded input is fed to the GPT-3.5 Turbo model from the OpenAI API, which produces the final output.
User Interface: Streamlit is used to create the interface for the application.
