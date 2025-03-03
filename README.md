# 🌍 Retrieval-Augmented Generation (RAG) for Climate Tweets  

## 📖 Project Overview  
This project implements a **Retrieval-Augmented Generation (RAG) system** using Hugging Face datasets and language models (LLMs).  
The goal is to build an AI-powered assistant that retrieves relevant **climate change tweets** and generates **context-aware responses**.  

## 🛠 How It Works  
1. **Retrieve relevant tweets** from the **TweetEval** dataset (stance on climate change).  
2. **Convert text into vector embeddings** using **Hugging Face Embeddings**.  
3. **Store embeddings in a vector database (FAISS)** for efficient retrieval.  
4. **Use a language model (GPT-2)** to generate responses based on retrieved tweets.  
5. **Deploy a simple user interface** with **Gradio** to interact with the model.  

## 📦 Tech Stack  
- 🧠 **LLM:** GPT-2 (or any model from Hugging Face)  
- 📄 **Dataset:** TweetEval (stance_climate subset)  
- 📊 **Embeddings:** Hugging Face Embeddings  
- 🔍 **Vector Storage:** FAISS  
- 🏗 **Framework:** LangChain  
- 🎨 **UI:** Gradio  

## 🚀 How to Run It  
### **1️⃣ Install Dependencies**  
Run the following in your terminal:  
```bash
pip install langchain langchain-community faiss-cpu huggingface-hub gradio

```

## Project Organization

```
├── LICENSE            <- Open-source license if one is chosen
├── Makefile           <- Makefile with convenience commands like `make data` or `make train`
├── README.md          <- The top-level README for developers using this project.
├── data
│   ├── external       <- Data from third party sources.
│   ├── interim        <- Intermediate data that has been transformed.
│   ├── processed      <- The final, canonical data sets for modeling.
│   └── raw            <- The original, immutable data dump.
│
├── docs               <- A default mkdocs project; see www.mkdocs.org for details
│
├── models             <- Trained and serialized models, model predictions, or model summaries
│
├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
│                         the creator's initials, and a short `-` delimited description, e.g.
│                         `1.0-jqp-initial-data-exploration`.
│
├── pyproject.toml     <- Project configuration file with package metadata for 
│                         rag and configuration for tools like black
│
├── references         <- Data dictionaries, manuals, and all other explanatory materials.
│
├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
│   └── figures        <- Generated graphics and figures to be used in reporting
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── setup.cfg          <- Configuration file for flake8
│
└── rag   <- Source code for use in this project.
    │
    ├── __init__.py             <- Makes rag a Python module
    │
    ├── config.py               <- Store useful variables and configuration
    │
    ├── dataset.py              <- Scripts to download or generate data
    │
    ├── features.py             <- Code to create features for modeling
    │
    ├── modeling                
    │   ├── __init__.py 
    │   ├── predict.py          <- Code to run model inference with trained models          
    │   └── train.py            <- Code to train models
    │
    └── plots.py                <- Code to create visualizations
```

--------
