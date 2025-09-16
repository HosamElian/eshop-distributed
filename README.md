# 🛒 AI-Powered E-Shop with .NET Aspire & GenAI

This project demonstrates how to design and implement **cloud-native distributed architectures** using the **.NET Aspire framework**, while integrating **Generative AI (GenAI)** capabilities with **Microsoft Extensions AI** and **Semantic Kernel**.  

The system is built around an **E-Shop platform** with **Catalog** and **Basket microservices**, leveraging **PostgreSQL**, **Redis**, and **RabbitMQ** for data storage, caching, and messaging. It also incorporates **secure authentication** via Keycloak and intelligent AI features such as **semantic search** and **Q&A chatbots**.

---

## 🚀 What You'll Learn

- Cloud-Native Distributed Architectures  
- .NET Aspire Framework for Distributed Development  
- Catalog Service with PostgreSQL + RabbitMQ  
- Basket Service with Redis + Keycloak Authentication  
- Messaging & Event-Driven Patterns with RabbitMQ & MassTransit  
- Blazor Web Client for the E-Shop Platform  
- Containerization & Deployment to Azure Container Apps  
- Generative AI Integration with Semantic Kernel & Ollama Models  

---

## 🏗️ Architecture Overview

- **Catalog Microservice**  
  - PostgreSQL for product storage  
  - Publishes integration events (e.g., `ProductPriceChanged`) via RabbitMQ  

- **Basket Microservice**  
  - Redis for fast basket storage  
  - Syncs with Catalog service  
  - Secured with Keycloak (JWT Bearer tokens)  

- **Event-Driven Messaging**  
  - RabbitMQ + MassTransit for async communication  
  - Reliable publish/subscribe patterns with error handling  

- **Blazor Client App**  
  - User-facing e-commerce front end  
  - Connects to services via .NET Aspire Service Discovery  

- **GenAI Features**  
  - AI-powered Q&A chatbot with Semantic Kernel + Ollama  
  - Semantic product search with RAG (Retrieval-Augmented Generation)  

---

## 🧑‍💻 Tech Stack

- **Backend**: .NET Aspire, ASP.NET Core, MassTransit  
- **Frontend**: Blazor WebAssembly  
- **Databases**: PostgreSQL (Catalog), Redis (Basket)  
- **Messaging**: RabbitMQ  
- **Authentication**: Keycloak (JWT Bearer)  
- **Deployment**: Azure Container Apps, Docker  
- **AI/ML**: Microsoft Extensions AI, Semantic Kernel, Ollama (Llama/Phi models)  

---

## ⚙️ Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/your-username/eshop-aspire-genai.git
   cd eshop-aspire-genai
Run Services with .NET Aspire

bash
Copy code
dotnet run
Deploy to Azure Container Apps

bash
Copy code
azd up
🧠 GenAI Use Cases
Customer Support Chatbot

Context-aware Q&A using Semantic Kernel

Real-time responses powered by Ollama models

Semantic Product Search (RAG)

Vector-based embeddings for product search

Personalized recommendations for users

📦 Project Structure
├── src/
│   ├── CatalogService/
│   ├── BasketService/
│   ├── BlazorClient/
│   ├── Shared/
│   └── Aspire.AppHost/
├── infra/
│   ├── docker-compose.yml
│   └── azure-deployment/
└── README.md

🌐 Deployment
Local development with Docker and .NET Aspire

Cloud deployment with Azure Container Apps

CI/CD ready project structure with azd up / azd down

📜 License
This project is licensed under the MIT License.

yaml





