# **Agentic AI System for Automated RFP Discovery, Analysis & Response**

This repository contains the implementation of a fully autonomous **Agentic AI–driven RFP (Request for Proposal) Automation Platform** designed to transform the traditional, manual, and time-consuming RFP workflow for industrial manufacturing enterprises.

The system detects new RFPs, summarizes key requirements, performs technical SKU matching, estimates pricing, and generates submission-ready proposals — all with human-in-the-loop oversight.

---

## **1. Overview**

Industrial B2B RFP handling is still highly manual, leading to:

* Delayed identification of new opportunities
* Hours spent manually matching product specifications
* Lower win rates due to late or incorrect submissions
* Inefficient use of sales, technical, and pricing resources

Since **90%+ of RFP wins depend on timely submissions**, automated intelligence becomes essential.

This project delivers a **multi-agent AI platform** that autonomates the entire lifecycle:

1. Discover new RFPs
2. Summarize requirements
3. Match product specifications
4. Estimate pricing
5. Generate complete RFP responses

---

## **2. Key Features**

### **Autonomous RFP Lifecycle Management**

* Automated scanning of predefined government/enterprise portals
* Extraction and summarization of RFP documents
* Intelligent routing to technical and pricing agents

### **AI-Driven Technical Matching**

* NLP-based requirement extraction
* FAISS-enabled similarity search
* Automatic SKU mapping with “Spec Match %” scoring

### **Automated Pricing Engine**

* Pricing lookup using internal rate tables
* Approximate cost calculations via mock APIs

### **End-to-End Proposal Generation**

* Auto-generated structured RFP responses
* Export to downloadable **PDF** and **Excel** formats

### **Interactive Web Dashboard**

* Status tracking
* RFP-level analytics
* Multi-role access for sales, technical, and leadership teams

---

## **3. System Architecture**

### **Agentic Architecture Components**

* **Main Agent (Orchestrator)**
  Coordinates the end-to-end workflow and integrates outputs from other agents.

* **Sales Agent**
  Crawls/scans URLs, extracts RFPs, and generates summaries.

* **Technical Agent**
  Performs requirement extraction and SKU/spec matching.

* **Pricing Agent**
  Computes material & service costs.

* **Report Generator**
  Produces submission-ready RFP documents.

### **Technology Stack**

#### **Backend**

* Python
* FastAPI
* Celery (background agent orchestration)

#### **Frontend**

* React
* Bootstrap

#### **Storage**

* PostgreSQL
* FAISS (vector similarity search)

#### **AI/NLP**

* LangChain
* OpenAI Embeddings
* Tesseract OCR for document extraction

#### **Deployment**

* Backend: AWS
* Frontend: Netlify

---

## **4. Benefits & KPIs**

### **Impact**

* **80%+ reduction** in manual effort
* **30–40% increase** in timely RFP identification
* **20%+ improvement** in win rates
* Improved visibility for decision-makers
* Scalable to hundreds of simultaneous RFPs

---

## **5. Repository Structure** *(recommended)*

```
/backend
    /api
    /agents
    /models
    /services
    /pricing
    /rpf_scanner
    main.py
/frontend
    /src
    /components
    /pages
    App.tsx
/docs
    architecture-diagram.png
    sample-rfp.pdf
/scripts
    data_ingestion.py
    faiss_indexer.py
README.md
```

---

## **6. Getting Started**

### **Prerequisites**

* Python 3.10+
* Node.js 18+
* PostgreSQL
* AWS credentials (optional for deployment)

### **Backend Setup**

```
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### **Frontend Setup**

```
cd frontend
npm install
npm run dev
```

---

## **7. Future Enhancements**

* Integration with SAP/ERP systems
* Fine-tuned domain-specific LLMs for spec extraction
* Automated bidding decision engine
* Multi-language RFP parsing

---

## **8. Contributors**

* Harlee
* Ajay
* Akash
* Akil
* Kavin