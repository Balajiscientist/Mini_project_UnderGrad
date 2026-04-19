![Banner](banner1.png)
# RAG-Based-Researcher-Research-Analyst
🏙️ **Researcher Research Assistant**

Researchers and analysts often fail not due to lack of time, but because they **cannot read and process all research papers, news articles, and documents efficiently**.  
This AI-powered tool uses **RAG (Retrieval-Augmented Generation)** to make research effortless. Users can **input article URLs or upload documents** and ask questions to instantly retrieve relevant insights. Initially focused on the **real estate domain**, it can be extended to any field.


---

## Features

### 🔹 URL-Based Research
- Load multiple article URLs.
- Extract content using **LangChain's UnstructuredURL Loader**.
- Split text, generate embeddings using **HuggingFace**, and store in **ChromaDB**.
- Ask questions via **Llama3 (Groq)** and receive answers with source URLs.

### 🔹 Document & File Upload Research
- Upload **PDFs, DOCX, TXT, CSV, and images**.
- Automatic text extraction and semantic indexing.
- Ask questions across your **private research repository**.

### 🔹 Smart AI Q&A
- Ask questions in natural language.
- Answers are **relevant, contextual, and include sources** for validation.

### Set-up

1. Run the following command to install all dependencies. 

    ```bash
    pip install -r requirements.txt
    ```

2. Create a .env file with your GROQ credentials as follows:
    ```text
    GROQ_MODEL=MODEL_NAME_HERE
    GROQ_API_KEY=GROQ_API_KEY_HERE
    ```

3. Run the streamlit app by running the following command.

    ```bash
    streamlit run main.py
    ```

##  Team Contributions & Roles

| Name | Role | Key Contributions |
|------|------|------------------|
| **B. Balaji** | GenAI & Full Stack Developer | • Designed overall system architecture (RAG pipeline)<br>• Integrated frontend (Streamlit) & backend (FastAPI)<br>• Implemented LLM (Llama3 via Groq) and API workflows |
| **K. Surya Akhil Varma** | Backend & Data Engineer | • Built REST APIs using FastAPI<br>• Managed document processing & data pipelines<br>• Handled database (ChromaDB / MySQL) and embeddings |
| **K. Yuva Sankar** | Frontend & UI Developer | • Developed interactive UI using Streamlit<br>• Implemented user workflows (URL input, file upload, Q&A)<br>• Improved usability and responsiveness |
| **Navya Sree** | UI/UX Designer & Research Analyst | • Designed Figma prototypes and wireframes<br>• Created user journey and layout planning<br>• Conducted research on user needs & optimized UX |
