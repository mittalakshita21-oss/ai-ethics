<img width="1252" height="718" alt="image" src="https://github.com/user-attachments/assets/29076723-64a4-466f-b3d1-a26015e77d97" /># 🤖 AI Conversational RAG Chatbot (Flowise)

This project is a **Conversational AI chatbot built using Retrieval-Augmented Generation (RAG)** with Flowise.  
The chatbot can answer questions from uploaded documents by retrieving relevant context and generating accurate responses using an LLM.

It combines **document retrieval, embeddings, vector search, and conversational memory** to provide context-aware responses.

---

# 🚀 Project Overview

This chatbot uses a **RAG pipeline** where documents are loaded, split into chunks, converted into embeddings, stored in a vector database, and then retrieved during conversation to generate answers.

The system allows users to ask questions related to the uploaded documents while maintaining conversation history.

---

# 🧠 Architecture

The system workflow follows these steps:

1. **Document Loading**
   - Documents are loaded using the File Loader node.

2. **Text Splitting**
   - Documents are divided into smaller chunks using Recursive Character Text Splitter.

3. **Embedding Generation**
   - Each chunk is converted into vector embeddings using Google Gemini Embeddings.

4. **Vector Storage**
   - Embeddings are stored in an In-Memory Vector Store.

5. **Retrieval**
   - Relevant document chunks are retrieved based on user queries.

6. **Response Generation**
   - The Mistral LLM generates answers using retrieved context.

7. **Conversation Memory**
   - Buffer Memory stores chat history to maintain conversation continuity.

---

# ⚙️ Technologies Used

- **Flowise AI**
- **Mistral AI (LLM)**
- **Google Gemini Embeddings**
- **Vector Store (In-Memory)**
- **Conversational Retrieval QA Chain**
- **RAG (Retrieval Augmented Generation)**

---

# 🏗 System Components

### 1️⃣ File Loader
Loads documents such as PDFs or other supported files.

### 2️⃣ Recursive Character Text Splitter
Splits documents into smaller chunks for better embedding and retrieval.

### 3️⃣ Google Gemini Embeddings
Generates vector embeddings for document chunks.

### 4️⃣ In-Memory Vector Store
Stores embeddings and retrieves the most relevant chunks during queries.

### 5️⃣ Mistral AI Chat Model
Generates responses using retrieved document context.

### 6️⃣ Buffer Memory
Stores conversation history to maintain context across interactions.

### 7️⃣ Conversational Retrieval QA Chain
Combines retrieval + LLM + memory to produce contextual answers.

---

# 🔄 RAG Pipeline

```
User Question
      │
      ▼
Vector Search (Retriever)
      │
      ▼
Relevant Document Chunks
      │
      ▼
LLM (Mistral AI)
      │
      ▼
Final Answer
```

---

# 📊 Features

✔ Conversational document question answering  
✔ Retrieval-Augmented Generation (RAG)  
✔ Context-aware responses  
✔ Chat history memory  
✔ Vector-based semantic search  
✔ Modular Flowise pipeline

---

# 📸 Screenshots

Add screenshots of your workflow here.

Example:

```
/screenshots
   ├── flowise-dashboard.png
   ├── chat-interface.png
   └── pipeline-architecture.png
```
<img width="712" height="696" alt="image" src="https://github.com/user-attachments/assets/ec2fc29c-7b61-4c02-bc98-1c695d24bb7c" />
<img width="1252" height="718" alt="image" src="https://github.com/user-attachments/assets/19df9fff-88b2-4ab6-a870-82d83fbcbdd2" />
Then embed them like:

```markdown
![Dashboard](screenshots/flowise-dashboard.png)
![Chat Interface](screenshots/chat-interface.png)
```

---

# 🛠 How to Use

### 1️⃣ Install Flowise
```
npm install -g flowise
```

### 2️⃣ Start Flowise
```
npx flowise start
```

### 3️⃣ Import the Chatflow
- Open Flowise Dashboard
- Import the provided JSON chatflow file
- Configure API keys

### 4️⃣ Add API Keys

Required APIs:

- Mistral AI API Key
- Google Generative AI API Key

---

# 📁 Project Structure

```
project-folder
│
├── chatbot-chatflow.json
├── screenshots/
│   ├── dashboard.png
│   └── pipeline.png
│
└── README.md
```

---

# 🔮 Future Improvements

- Use **persistent vector databases (Pinecone / Chroma / Weaviate)**
- Add **multi-document support**
- Improve **prompt engineering**
- Add **web interface for users**
- Implement **authentication and user sessions**
- Deploy chatbot using **Docker or cloud services**

---

# 🎯 Learning Outcomes

This project demonstrates:

- RAG architecture
- Vector search and embeddings
- Conversational AI pipelines
- Document-based question answering
- Flowise AI workflow design

---

# 👩‍💻 Author

**Akshita**

AI & Automation Enthusiast  
Exploring Conversational AI, RAG systems, and AI workflows.

---
