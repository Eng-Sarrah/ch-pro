# 🤖 Cloud-based Intelligent Chatbot

A cloud-native intelligent chatbot that retrieves accurate, context-aware answers from PDF documents using Retrieval-Augmented Generation (RAG). Built with FastAPI and Streamlit, deployed on Microsoft Azure with scalability, security, and best practices for CI/CD in mind. ☁️

---

## 🚀 Project Overview

This project was developed as part of the Cloud Computing Bootcamp organized by the Saudi Digital Academy, in collaboration with a team of aspiring cloud professionals. 🌍

The chatbot enables users to upload PDF documents and interact with them through natural language questions. It provides intelligent and context-aware answers using a combination of retrieval and generation techniques, making document search smarter and easier. 📚💬

---

## ✨ Key Features

- 🔍 Retrieval-Augmented Generation (RAG) using [ChromaDB]: Accurate answers based on embedded content in PDFs.
- ⚙️ Flexible architecture: Frontend using [Streamlit] and backend using [FastAPI].
- ☁️ Cloud Deployment on Azure: Scalability and security using VM Scale Sets, Application Gateway, and Blob Storage.
- 🔐 Secrets Management with [Azure Key Vault].
- 🗃️ Data storage using [Azure PostgreSQL].
- 🔄 CI/CD with [GitHub Actions] for continuous integration and deployment.

---

## 🛠️ Tech Stack

| Layer               | Technology                            |
|---------------------|---------------------------------------|
| Frontend            | Streamlit                             |
| Backend             | FastAPI                               |
| Retrieval & Generation | ChromaDB + LangChain (optional)     |
| Storage             | Azure Blob Storage                    |
| Database            | Azure Database for PostgreSQL         |
| Secrets Management  | Azure Key Vault                       |
| Compute             | Azure VM Scale Sets                   |
| Networking          | Azure Application Gateway             |
| CI/CD               | GitHub Actions                        |

---

## 🕒 Development Timeline

🧪 Stage 1–4: Local Application Development

| Stage | Description |
|-------|-------------|
| 1     | Built a simple chatbot using Streamlit |
| 2     | Separated frontend (Streamlit) and backend (FastAPI) |
| 3     | Integrated PostgreSQL for chat history storage |
| 4     | Implemented RAG using Chroma to support question answering from PDFs |

✅ Result: Fully functional local chatbot with context-aware answers from PDFs.

---

## ☁️ Stage 5–6.5: Cloud Deployment & Automation

| Stage | Description |
|-------|-------------|
| 5     | Manually deployed the app on Azure VM and set up PostgreSQL database |
| 6     | Migrated to cloud services on Azure: Blob Storage and PostgreSQL |
| 6.1   | Added scalability with VM Scale Sets and load balancing using Application Gateway |
| 6.5   | Enhanced security with Azure Key Vault |
| 🔄    | Automated deployment using Terraform and GitHub Actions |

## 🧭 Architecture Diagram
The following diagram illustrates the overall cloud-based architecture of the chatbot application and how the components interact in a secure, scalable, and efficient manner. 🧱☁️
![image](https://github.com/user-attachments/assets/7ed4dc22-54b1-4e24-9ae1-c87359f442ed)

---

## ⚙️ How the Project Works (Behind the Scenes)

1. 📄 The user uploads a PDF via the Streamlit interface.
2. 📚 The content is converted into embeddings using Chroma.
3. ❓ The user asks a question.
4. 🔍 Chroma searches for the most relevant content.
5. 🧠 FastAPI generates an answer based on the retrieved content.
6. 💬 The answer is displayed to the user on Streamlit.

---

## 📁 Project Structure
- `app/backend.py` – FastAPI backend code  
- `streamlit_app/chatbot.py` – Streamlit frontend code  
- `.github/workflows/stage6deploy.yml` – GitHub Actions for CI/CD  
- `requirements.txt` – Project dependencies  
- `setup.sh` – Script for environment setup  
- `update_app.sh` – Script to update the app  
- `README.md` – Project documentation  

