# 🔐 AI-Powered Security Risk Assessment (SAR) Agent

An intelligent security risk assessment agent built with LangChain, Ollama (LLaMA 3), and ChromaDB that automates the evaluation of software tools against enterprise security policies using a RAG (Retrieval-Augmented Generation) pipeline.

---

## 🎯 Project Overview

Security analysts at enterprises like KPMG manually review hundreds of Software Assessment Requests (SARs) — evaluating whether a tool complies with security policies like NIST 800-53 and ISO 27001. This process is time-consuming and repetitive.

This project automates that workflow using AI:
- User describes a software tool
- AI searches policy knowledge base
- AI returns: risk level + policy citations + recommendation

---

## 🏗️ Architecture
---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| **LangChain** | AI orchestration framework |
| **Ollama + LLaMA 3** | Local LLM (no API key needed) |
| **ChromaDB** | Vector database for policy documents |
| **RAG Pipeline** | Connects AI to policy knowledge base |
| **Streamlit** | Web-based chat interface |
| **Python 3.12** | Core language |

---

## 📋 Security Frameworks Covered

- NIST 800-53 Security Controls
- ISO 27001 Information Security Standards

---

## 🚀 Getting Started

### Prerequisites
- Python 3.9+
- Ollama installed
- 4GB+ RAM

### Installation

```bash
# Clone the repository
git clone https://github.com/dikshach957/security-risk-assessment-ai.git
cd security-risk-assessment-ai

# Create virtual environment
python3 -m venv venv
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Pull LLaMA 3 model
ollama pull llama3

# Run the application
streamlit run app.py
```

---

## 📁 Project Structure
---

## 💡 Use Case Example

**Input:**
> "We want to use Slack to share internal project files and client communications"

**Output:**
> ⚠️ MEDIUM RISK — Slack may violate data residency requirements under ISO 27001 Annex A.8. NIST 800-53 SC-8 requires transmission confidentiality. Recommend: encryption at rest, data classification policy review, and vendor security assessment before approval.

---

## 👩‍💻 Author

**Diksha Chaudhary**
Cybersecurity Postgraduate — Conestoga College 2025-2026
[LinkedIn](https://linkedin.com/in/your-profile) | [GitHub](https://github.com/dikshach957)

---

## 📌 Status
🔄 In Progress — Active Development
