# AI-Powered-Store-Customer-Service-Chatbot
[🎥 Demo Video](https://drive.google.com/file/d/1gjqrZ4s4Z-qcvUumfmJU-WpKBTH_4tIO/view?usp=sharing)
## 📝 Project Overview
Developed and implemented an **intelligent AI chatbot** for a PC store's **Facebook Messenger** platform, enabling automated customer service and product recommendations in **Egyptian Arabic**.  
The system features **automated data ingestion from Google Drive** and a **dual vector database architecture** for high availability.

---

## 🚀 Technical Achievements
- Engineered an **n8n workflow** integrating **OpenAI GPT-4**, **Pinecone vector database**, **Supabase**, and **Facebook Messenger API**  
- Implemented **Arabic natural language processing** for customer interactions in **Egyptian dialect**  
- Designed an **automated data pipeline** from Google Drive to vector databases with **real-time synchronization**  
- Built a **dual vector store architecture** (Pinecone + Supabase) for redundancy and performance optimization  
- Created an **automated webhook system** for seamless **Facebook Messenger integration**  

---

## 🎯 Key Responsibilities
- Architected complete **AI agent workflow** from concept to deployment  
- Configured **automated data ingestion pipeline** from Google Drive  
- Implemented **multi-vector database strategy** for high availability  
- Designed **conversation memory and context management system**  
- Optimized AI responses for **local language and cultural context**  

---

## 🛠 Technologies Used
- **Workflow Automation:** n8n  
- **AI/ML:** OpenAI GPT-4, Vector Embeddings  
- **Databases:** Pinecone, Supabase  
- **Cloud Storage:** Google Drive API  
- **APIs:** Facebook Messenger API, Webhooks  
- **Languages:** JavaScript, JSON  

---

## 📈 Business Impact
- Automated **80% of routine customer inquiries**  
- Reduced response time from **hours to seconds**  
- Enabled **automatic product catalog updates** without manual intervention  
- Improved customer satisfaction through **24/7 availability**  
- Implemented **scalable, fault-tolerant architecture**  

---

## ✨ Key Features
- Multi-language support (**Egyptian Arabic focus**)  
- Real-time **product specification queries**  
- **Automated data synchronization** from cloud storage  
- **Dual vector database architecture** for redundancy  
- **Intelligent recommendation engine**  
- **Conversation history and context maintenance**  
- Seamless **Facebook Messenger integration**  

---

## 🗂 Workflow Architecture

Architecture
Core Components

Webhook (Facebook Messenger Integration)

Receives incoming messages from Facebook
Validates webhook subscriptions
Routes messages to appropriate processors


Media Processing Layer

Switch Node: Routes attachments by type
Transcribe Recording: Converts voice messages to text using OpenAI
Analyze Image: Extracts laptop details from product images
HTTP Request: Fetches attachment payloads


AI Agent Core

OpenAI Chat Model (GPT-4o): Powers the conversational AI
Simple Memory: Maintains conversation context per user session
Supabase Vector Store: Retrieves laptop inventory data via semantic search
Custom System Prompt: Defines agent personality and behavior (Egyptian colloquial Arabic, sales techniques, store policies)


Data Persistence

Google Sheets Integration: Saves confirmed orders with customer details


Response Handler

Code Node: Formats responses for Facebook compatibility
HTTP Request: Sends formatted responses back to Facebook Messenger  

**Chat Processing:**  
Facebook Messenger webhook → AI agent with memory → Vector store retrieval → Response generation  

**Error Handling:**  
Comprehensive error handling and retry mechanisms for all external API calls  
