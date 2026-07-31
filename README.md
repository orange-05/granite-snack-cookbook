# Granite Snack Cookbook (Fork)

![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg?style=for-the-badge)
![Fork](https://img.shields.io/badge/Fork-of_ibm--granite--community/granite--snack--cookbook-blue?style=for-the-badge)
![Upstream Stars](https://img.shields.io/github/stars/ibm-granite-community/granite-snack-cookbook?style=for-the-badge&label=Upstream%20Stars)

> **Granite Snack Cookbook** — Easily consumable recipes (Python notebooks) showcasing IBM Granite model capabilities. This is a fork of the official IBM Granite Community cookbook.

---

## ⚠️ **This is a Fork**

**Upstream Repository:** https://github.com/ibm-granite-community/granite-snack-cookbook

**For the latest recipes, updates, and contributions, visit the upstream repository.**

This fork exists for:
- Personal experimentation with Granite models
- Offline access to recipes
- Testing modifications locally
- Potential upstream contributions

---

## 🌟 Overview

The **Granite Snack Cookbook** is a collection of Jupyter notebooks ("recipes") demonstrating the capabilities of IBM's **Granite** family of foundation models. Each notebook is a self-contained, runnable example covering tasks like:

- **RAG (Retrieval-Augmented Generation)**
- **Function Calling / Tool Use**
- **Summarization**
- **Code Generation**
- **Question Answering**
- **Agent Workflows**
- **Fine-tuning / LoRA**

---

## 📚 Recipe Categories (Upstream)

| Category | Description | Example Notebooks |
|----------|-------------|-------------------|
| **RAG** | Document QA, vector search, LangChain integration | `RAG_with_Langchain.ipynb` |
| **Function Calling** | Tool use, structured output, API integration | `Function_Calling.ipynb` |
| **Summarization** | Long document summarization, key point extraction | `Summarize.ipynb` |
| **Agents** | Multi-step reasoning, ReAct, planning | `AI-Agents/` |
| **Code** | Code generation, explanation, translation | `Code_Generation.ipynb` |
| **Fine-tuning** | LoRA, QLoRA, parameter-efficient tuning | `Fine_tuning/` |

---

## 🛠 Tech Stack

| Component | Technology |
|-----------|------------|
| **Environment** | Jupyter Notebook / JupyterLab |
| **Language** | Python 3.9+ |
| **Models** | IBM Granite (via WatsonX, Hugging Face, Ollama) |
| **Frameworks** | LangChain, LlamaIndex, Haystack, Transformers |
| **Hardware** | CPU / GPU / Apple Silicon (MPS) |
| **License** | Creative Commons Attribution 4.0 International |

---

## 📁 Project Structure (Upstream)

```text
granite-snack-cookbook/
├── recipes/
│   ├── RAG/
│   │   ├── RAG_with_Langchain.ipynb
│   │   ├── RAG_with_LlamaIndex.ipynb
│   │   └── ...
│   ├── Function-Calling/
│   │   └── Function_Calling.ipynb
│   ├── Summarize/
│   │   └── Summarize.ipynb
│   ├── AI-Agents/
│   │   ├── ReAct_Agent.ipynb
│   │   └── ...
│   ├── Code-Generation/
│   ├── Fine-Tuning/
│   └── ...
├── assets/                 # Shared data, images
├── requirements.txt        # Common dependencies
├── environment.yml         # Conda environment
├── CONTRIBUTING.md         # Upstream contribution guide
├── LICENSE                 # CC BY 4.0
└── README.md               # This file (fork version)
```

---

## 🚀 Quick Start

### Prerequisites
- Python 3.9+
- Jupyter: `pip install jupyterlab`
- IBM WatsonX account **or** local Ollama **or** Hugging Face token

### Installation

```bash
# Clone this fork
git clone https://github.com/orange-05/granite-snack-cookbook.git
cd granite-snack-cookbook

# Create environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
# or: conda env create -f environment.yml

# Start Jupyter
jupyter lab
```

### Running a Recipe

1. Open a notebook in `recipes/<category>/`
2. **Configure credentials** (first cells):
   ```python
   # WatsonX
   WATSONX_APIKEY = "your_key"
   WATSONX_URL = "https://us-south.ml.cloud.ibm.com"
   PROJECT_ID = "your_project_id"
   
   # OR Ollama (local)
   # ollama pull granite3.1-dense:8b
   ```
3. Run cells sequentially (`Shift+Enter`)

---

## 🔑 Model Access Options

| Platform | Setup | Best For |
|----------|-------|----------|
| **WatsonX** | IBM Cloud account, API key | Production, enterprise |
| **Ollama** | `ollama pull granite3.1-dense:8b` | Local dev, privacy, free |
| **Hugging Face** | HF token, `transformers` | Experimentation, fine-tuning |
| **Replicate** | API token | Quick API access |

---

## 🔄 Keeping This Fork Updated

```bash
# Add upstream (once)
git remote add upstream https://github.com/ibm-granite-community/granite-snack-cookbook.git

# Fetch and merge
git fetch upstream
git checkout main
git merge upstream/main
git push origin main
```

---

## 🤝 Contributing

**Contribute to upstream!** They welcome:
- New recipes for Granite capabilities
- Bug fixes in existing notebooks
- Documentation improvements
- Support for new frameworks

See upstream [CONTRIBUTING.md](https://github.com/ibm-granite-community/granite-snack-cookbook/blob/main/CONTRIBUTING.md).

---

## 📄 License

**Creative Commons Attribution 4.0 International (CC BY 4.0)** — Same as upstream.

You may share and adapt with attribution to **IBM Granite Community**.

---

## 👤 Fork Owner

**Karthikeyan K** (BCA Analytics)
- GitHub: [@orange-05](https://github.com/orange-05)
- Location: Bengaluru, India

---

*Forked for Granite model exploration — contribute upstream!* — Last synced July 2026