<div align="center">

# Hi, I'm Arun Yadav 👋

**B.Tech Computer Science & Engineering · Delhi Technological University · 2023–2027**

![Python](https://img.shields.io/badge/Python-%23378ADD?style=for-the-badge&logo=python&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-%231D9E75?style=for-the-badge&logo=sqlite&logoColor=white)
![Software Engineering](https://img.shields.io/badge/Software%20Engineering-%237F77DD?style=for-the-badge)
![ML & AI](https://img.shields.io/badge/ML%20%26%20AI-%23993C1D?style=for-the-badge)
![C++](https://img.shields.io/badge/C%2B%2B-%23D85A30?style=for-the-badge&logo=cplusplus&logoColor=white)
![Open to Internships & Full-time](https://img.shields.io/badge/Open%20to%20Internships%20%26%20Full--time%20%F0%9F%94%8D-%23BA7517?style=for-the-badge)

</div>

---

> Fourth-year CS student who builds tools that keep running after the demo. I like problems where real people and real data meet: getting field data off unreliable links intact, making sure the numbers a team relies on are actually right, and writing the runbook so someone who isn't an engineer can operate it. I also work on NLP, federated learning and retrieval systems, and I turn complex ideas into working, tested code.

**How I work**

- **Own it end to end.** I take a tool from the first version to something tested, containerised and running in CI, then keep improving it.
- **Make failures visible.** Metrics, structured logs and alerts, so a problem is noticed before someone has to ask.
- **Check the numbers.** Every headline figure in my projects comes from a script you can re-run, and I report results that came out flat or negative too.
- **Write it down.** READMEs, architecture notes and SOPs written for the person who has to use the tool.

---

## 🚀 Featured Projects

### 📦 [Offloader](https://github.com/yadavaruncs/offloader)
An upload agent that gets multi-gigabyte recordings off field kits and into S3 over slow, intermittent site internet. Uploads **resume from the last acknowledged part** using a **SQLite journal**, and integrity is checked twice, with per-part ETags and a whole-file SHA-256. A watchdog alerts on **stalled** uploads, not just failed ones, and **Prometheus metrics** cover the whole pipeline. A fault-injection benchmark shows resume cutting bytes moved by **50%** versus a naive restart, with **zero corrupted objects**. It ships with a **field SOP** for non-technical site staff, plus 77 tests at about 90% coverage and CI on GitHub Actions.

![Python](https://img.shields.io/badge/Python-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white&logo=python)
![AWS S3](https://img.shields.io/badge/AWS%20S3-%23FBEAE3?style=flat&labelColor=%23D85A30&color=%23D85A30&logoColor=white&logo=amazons3)
![SQLite](https://img.shields.io/badge/SQLite-%23E1F5EE?style=flat&labelColor=%231D9E75&color=%231D9E75&logoColor=white&logo=sqlite)
![Prometheus](https://img.shields.io/badge/Prometheus-%23FAEEDA?style=flat&labelColor=%23BA7517&color=%23BA7517&logoColor=white&logo=prometheus)
![Docker](https://img.shields.io/badge/Docker-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white&logo=docker)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-%23EEEDFE?style=flat&labelColor=%237F77DD&color=%237F77DD&logoColor=white&logo=githubactions)

### 🧠 [AI Doubt Engine](https://github.com/yadavaruncs/AI-Doubt-Engine)
A physics doubt-solver built on **RAG** with a **LangGraph** agent. It routes each question, retrieves textbook passages with **hybrid dense + BM25 search** in Qdrant, and sends every calculation to a sandboxed **SymPy** tool instead of trusting the LLM's arithmetic. An ablation on 75 questions showed hybrid search lifting the hit rate on paraphrased questions from 84% to 94%, while a cross-encoder reranker did not earn its latency.

![Python](https://img.shields.io/badge/Python-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white&logo=python)
![LangGraph](https://img.shields.io/badge/LangGraph-%23EEEDFE?style=flat&labelColor=%237F77DD&color=%237F77DD&logoColor=white)
![Qdrant](https://img.shields.io/badge/Qdrant-%23FBEAE3?style=flat&labelColor=%23D85A30&color=%23D85A30&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-%23E1F5EE?style=flat&labelColor=%231D9E75&color=%231D9E75&logoColor=white&logo=fastapi)

### 📈 [Prediction Market Calibration](https://github.com/yadavaruncs/Prediction-market-calibration)
Are Polymarket prices honest probabilities? A calibration study of **897 resolved markets** using clustered bootstrap intervals, a Murphy decomposition, and a **walk-forward backtest with no lookahead**. Prices proved well calibrated (Brier skill score 0.51), and an apparent 9.2% trading return could not be distinguished from zero.

![Python](https://img.shields.io/badge/Python-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white&logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23FAEEDA?style=flat&labelColor=%23BA7517&color=%23BA7517&logoColor=white&logo=scikitlearn)
![statsmodels](https://img.shields.io/badge/statsmodels-%23EEEDFE?style=flat&labelColor=%237F77DD&color=%237F77DD&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-%23E1F5EE?style=flat&labelColor=%231D9E75&color=%231D9E75&logoColor=white&logo=pandas)

### 🔒 [FECL-EmotionAI](https://github.com/yadavaruncs/FECL-EmotionAI)
Measures what privacy really costs in emotion classification, comparing centralized training, **Federated Learning**, and federated training with **Differential Privacy** on a frozen **DistilBERT** encoder. Raw text never leaves the client, and Macro-F1 drops from 0.56 to 0.43, then to 0.20 at ε≈1.37.

![PyTorch](https://img.shields.io/badge/PyTorch-%23EEEDFE?style=flat&labelColor=%237F77DD&color=%237F77DD&logoColor=white&logo=pytorch)
![DistilBERT](https://img.shields.io/badge/DistilBERT-%23E1F5EE?style=flat&labelColor=%231D9E75&color=%231D9E75&logoColor=white)
![HuggingFace](https://img.shields.io/badge/HuggingFace-%23FAEEDA?style=flat&labelColor=%23BA7517&color=%23BA7517&logoColor=white)
![Federated Learning](https://img.shields.io/badge/Federated%20Learning-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white)

### ⚡ [SearchX](https://github.com/yadavaruncs/Search-X)
A search engine built from scratch in **C++20** — inverted index, TF-IDF ranking, Trie autocomplete, and a hand-built LRU cache, with multithreaded indexing and a benchmark suite showing 150x+ speedup over linear search.

![C++20](https://img.shields.io/badge/C%2B%2B20-%23FBEAE3?style=flat&labelColor=%23D85A30&color=%23D85A30&logoColor=white&logo=cplusplus)
![Data Structures](https://img.shields.io/badge/Data%20Structures-%23EEEDFE?style=flat&labelColor=%237F77DD&color=%237F77DD&logoColor=white)
![Multithreading](https://img.shields.io/badge/Multithreading-%23E6F1FB?style=flat&labelColor=%23185FA5&color=%23185FA5&logoColor=white)
![CMake](https://img.shields.io/badge/CMake-%23E1F5EE?style=flat&labelColor=%231D9E75&color=%231D9E75&logoColor=white&logo=cmake)

### More projects

- 💬 [Vera Bot](https://github.com/yadavaruncs/vera-bot): a WhatsApp merchant-engagement bot built for the magicpin AI challenge, with a live demo that runs the real bot in the browser.
- 🛗 [Lift Management System](https://github.com/yadavaruncs/Lift-Management-System): multi-floor lift scheduling in C++, designed to cut wait times and energy use across concurrent operations.
- 🎓 [Student Performance Predictor](https://github.com/yadavaruncs/Student-performance-predictor): an ML model that predicts student academic outcomes with 85% accuracy, served through a Streamlit app.

## 🛠️ Toolbox

- **Languages:** Python · SQL · C++
- **Data & storage:** SQLite · pandas · AWS S3 (boto3) · Qdrant
- **Ops & delivery:** Docker · GitHub Actions · Prometheus metrics · structured logging · pytest
- **Apps & ML:** FastAPI · Streamlit · PyTorch · HuggingFace · scikit-learn · LangGraph

## 📬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-%23E6F1FB?style=for-the-badge&logo=linkedin&labelColor=%23185FA5&color=%23185FA5&logoColor=white)](https://www.linkedin.com/in/arun-yadav-18281035b)
[![Email](https://img.shields.io/badge/Email-%23FAECE7?style=for-the-badge&logo=gmail&labelColor=%23993C1D&color=%23993C1D&logoColor=white)](mailto:arunyadav_23cs081@dtu.ac.in)
