<div align="center">

# Youssef Alaa Abdelrady

**Applied AI Engineer** · Cairo, Egypt

[LinkedIn](https://www.linkedin.com/in/youssef-alaa-334581406/) · [Email](mailto:youssefalaa.1356@gmail.com) · [Featured Projects](#featured-projects) · [Experience](#experience) · [Contact](#contact)

</div>

I build AI systems end to end: preparing the data, training and integrating the models, wrapping them in APIs and interfaces, and deploying them where they are actually used — from factory inspection lines to clinical decision-support tools.

My work concentrates on three areas: **computer vision for industrial inspection**, **RAG / LLM systems with real data pipelines**, and **applied ML for healthcare and predictive maintenance** — supported by an embedded & IoT background that lets me take intelligence to the edge.

---

## Featured Projects

### [AI Cable Defect Detection System — Elsewedy Electric](https://github.com/Youssef-Al-eng/Smart-Cable-Inspection-System-ElSewedy-Defect-Detection)
`Computer Vision` `Real-Time` `Industrial AI`

- **Problem:** Manual visual inspection of cable surfaces on production lines is slow and inconsistent; surface defects, label errors, and water contamination slip through.
- **What I built:** A 5-stage real-time inspection pipeline — Intel RealSense D435i synchronized RGB+depth capture (60 FPS) → custom-trained YOLOv8 detector for 3 defect classes → SSIM-based frame deduplication (95% threshold) → 3D surface analysis from depth data → operator review workflow. Training used K-fold validation, class-aware augmentation, and anti-bias analysis.
- **Stack:** Python · Ultralytics YOLOv8 · OpenCV · Intel RealSense
- **Results (documented in the repository):** ~90–95% detection accuracy in project evaluation, ~60% reduction in manual inspection, ~40% faster response time.
- Academic project, The Knowledge Hub – Coventry University (2026), supervised by Dr. Khaled Elgeneidy.

### [FinSight — Banking Document & Chart Q&A Agent](https://github.com/Youssef-Al-eng/Banking-Rag-Agent)
`RAG` `Vision LLM` `FastAPI`

- **Problem:** Financial analysts need exact figures buried in long annual reports, statements, and decks — including figures that only exist *inside charts*.
- **What I built:** A FastAPI backend + web frontend that ingests PDF, DOCX, XLSX/CSV, and TXT; extracts page text and every embedded chart in true reading order (PyMuPDF); sends each chart to a Groq vision model that returns exact `Category: value` data points; indexes text chunks, chart descriptions, and merged records with `all-MiniLM-L6-v2` embeddings in persistent ChromaDB; keeps multi-turn memory in SQLite; and exports branded Word / PDF / PowerPoint deliverables.
- **Stack:** Python · FastAPI · Groq (LLM + vision) · ChromaDB · sentence-transformers · SQLite

### [AI Physio — Shoulder Clinical Decision Support](https://github.com/Youssef-Al-eng/AI-Physio-Shoulder-CDS)
`Healthcare AI` `Multilingual RAG` `Docker`

- **Problem:** Physiotherapy triage for shoulder pathologies, accessible to patients in English and Egyptian Arabic.
- **What I built:** A multilingual RAG assistant covering 6 clinical conditions (impingement, frozen shoulder, rotator cuff tear, AC joint sprain, SLAP lesion, biceps tendinopathy) — multilingual sentence-transformer embeddings → FAISS vector search → LangGraph retrieval node, with distance-based confidence scoring, red-flag clinical alerts, 3-phase evidence-based protocols, and condition-specific exercise programs. Shipped with a production Docker setup (multi-stage build, health checks, non-root user).
- **Stack:** Python · LangGraph · FAISS · sentence-transformers · Streamlit · Docker

### [Predictive Maintenance Intelligence Platform — Schindler](https://github.com/Youssef-Al-eng/Schindler-AI-Maintenance-Intelligence-Platform)
`Predictive Maintenance` `Ensemble ML`

- **Problem:** Elevator fleets need maintenance risk prediction from real inspection data, usable by both engineers and administrators.
- **What I built:** A full-stack web app predicting maintenance needs with a soft-voting ensemble of four ML/DL models trained on **23,617 real inspection records** — single-unit diagnostics from technician checklists, bulk fleet analysis, role-based access, PDF/Excel reporting, and an in-app assistant chatbot.
- **Stack:** Python · TensorFlow · scikit-learn · Streamlit

### [AI-Powered Laptop Recommendation System](https://github.com/Youssef-Al-eng/Laptop-recommendation-system)
`RAG` `Agentic AI` `Recommendation`

- **Problem:** Laptop shopping requires reasoning over raw e-commerce specifications, not keyword matching.
- **What I built:** A full-stack recommendation engine — Amazon data scraping → spec parsing into a structured products database → RAG retrieval over technical specs (FAISS) → Llama 3.3 agent orchestration for context-aware, conversational recommendations, presented in Streamlit.
- **Stack:** Python · LangChain · FAISS · Llama 3.3 · Streamlit
- **Demo:** [Recorded walkthrough on YouTube](https://youtu.be/Rl3DawK-n4c)

### [Smart Cable Drum Monitoring — Embedded IoT](https://github.com/Youssef-Al-eng/Smart-Cable-Drum-Monitoring-System)
`IoT` `ESP32` `Edge Sensing`

- **Problem:** Cable drums on construction sites run untracked — material shortages, overheating, and off-site loss are detected too late.
- **What I built:** An ESP32 system written in native C that fuses MPU6050 (motion), LM35 (temperature), and GPS readings to track cable consumption, temperature, and location in real time; pushes to Firebase and visualizes everything in a Flask dashboard with alerting (≤5 m remaining cable, ≥40 °C).
- **Stack:** C/C++ · ESP32 · I2C/UART sensor drivers · Firebase · Flask

---

## End-to-End AI Engineering

Evidence across the lifecycle, drawn from the repositories above:

| Stage | Where I've done it |
|---|---|
| Problem framing & data preparation | Cable inspection (K-fold, class-aware augmentation), [ETL embedding pipeline](https://github.com/Youssef-Al-eng/etl-embedding-pipeline) (cleaning, chunking, checkpoint/resume) |
| Model development & evaluation | [Neural network from scratch in NumPy](https://github.com/Youssef-Al-eng/neural-network-from-scratch) (>95% MNIST), YOLOv8 training, ensemble ML |
| GenAI & LLM integration | RAG systems (FinSight, AI Physio, Laptop advisor), agent pipelines ([cognitive-pipelines](https://github.com/Youssef-Al-eng/cognitive-pipelines)), chart understanding with vision LLMs |
| APIs & backends | FastAPI services, Flask dashboards, JWT auth ([UrbanMind AI](https://github.com/Youssef-Al-eng/urbanmind-ai)) |
| User interfaces | Streamlit apps, React + Vite frontends ([Coloring Book AI Director](https://github.com/Youssef-Al-eng/ColoR_book_web)) |
| LLM operations | Routing, fallbacks, caching, rate limiting, cost tracking ([LLMOps Control Plane](https://github.com/Youssef-Al-eng/LLMOps-Control-Plane), [NexusAI](https://github.com/Youssef-Al-eng/NexusAI)) |
| Deployment | Dockerized services, production patterns (health checks, non-root containers) |
| Edge & embedded integration | ESP32 firmware, RealSense depth sensing, Firebase telemetry |

## More Engineering Work

| Project | What it is |
|---|---|
| [UrbanMind AI](https://github.com/Youssef-Al-eng/urbanmind-ai) | Full-stack smart-city platform: citizen portal + government dashboard, RAG over city documents (Qdrant), YOLOv8 incident detection, LangGraph sub-agents, FastAPI, PostgreSQL/Redis/Kafka |
| [Coloring Book AI Director (web)](https://github.com/Youssef-Al-eng/ColoR_book_web) | FastAPI + React app that turns a child's photo into a personalized print-ready coloring book PDF via an LLM + image-generation pipeline |
| [ResumeIQ (CV-Match)](https://github.com/Youssef-Al-eng/CV-Match) | Resume parsing and ranking vs. job descriptions: match scoring, ATS score, skill-gap detection |
| [AI Systems Design Suite](https://github.com/Youssef-Al-eng/AI-Systems-Design-) | Design-doc generation, cross-provider LLM cost optimization, multi-agent orchestration framework |
| [NER Pipeline](https://github.com/Youssef-Al-eng/named-entity-recognition-pipeline) | spaCy entity extraction with interactive highlighting and filtering |

## Research

Engineering-first research code, written and documented by me:

- **[GenAI-NetOpt](https://github.com/Youssef-Al-eng/GenAI-NetOpt)** — cross-layer protocol optimization with generative AI (LLM traffic prediction, CVAE-PPO congestion control, DQN edge offloading). Manuscript submitted to *IEEE Potentials* (2026).
- **[AdaptiveQoS-LLM](https://github.com/Youssef-Al-eng/AdaptiveQoS-LLM)** — cross-layer transformer for fine-grained QoS traffic classification. *IEEE Potentials* submission (2026).
- **[PINN for Structural Steel Alloys](https://github.com/Youssef-Al-eng/pinn-alloy-properties)** — physics-informed neural networks embedding Hall-Petch and thermodynamic constraints for mechanical property prediction. Research code for a paper submitted to *Next Materials* (Elsevier).

---

## Experience

| Role | Organization | Focus | Period |
|------|-------------|-------|--------|
| AI Engineer Intern | Genius Technology Center | RAG pipeline · FAISS · LangChain | Oct–Dec 2025 |
| IoT Engineer Intern | Elsewedy Electric | Industrial IoT · ESP32 · GPS monitoring | Jul–Sep 2025 |
| Innovation Engineer Intern | Schindler Group | ML for maintenance intelligence | Jul–Sep 2024 |
| IoT & Computer Vision Intern | The Sparks Foundation | Edge AI · cloud–edge trade-offs | Jun–Aug 2024 |

## Education

**B.Eng. Electrical and Electronics Engineering**
Coventry University — delivered at The Knowledge Hub Universities, Cairo, Egypt

## Technical Skills

- **Programming & Data:** Python · C/C++ (embedded) · JavaScript · SQL · pandas · NumPy
- **ML & DL:** PyTorch · TensorFlow · scikit-learn · XGBoost · spaCy
- **Computer Vision:** Ultralytics YOLOv8 · OpenCV · Intel RealSense · image processing & deduplication (SSIM)
- **GenAI / LLM:** RAG · LangChain · LangGraph · FAISS · ChromaDB · Qdrant · Groq API (Llama 3.x + vision) · sentence-transformers · prompt engineering
- **Backends & APIs:** FastAPI · Flask · Streamlit · REST · JWT authentication
- **Databases & Pipelines:** PostgreSQL · SQLite · Firebase · Redis · ETL design
- **Embedded & IoT:** ESP32 · Arduino/ATmega32 · UART/I2C/SPI · PWM/ADC · sensor fusion (MPU6050, LM35, GPS) · FSM design
- **Tooling & Deployment:** Docker · Git · Linux · Kafka · Plotly

---

## Contact

- **Email:** [youssefalaa.1356@gmail.com](mailto:youssefalaa.1356@gmail.com)
- **LinkedIn:** [youssef-alaa](https://www.linkedin.com/in/youssef-alaa-334581406/)
- **GitHub:** [Youssef-Al-eng](https://github.com/Youssef-Al-eng)

I'm open to AI engineering roles (computer vision, GenAI/LLM, applied ML) and to thesis-based graduate study starting Fall 2027.
