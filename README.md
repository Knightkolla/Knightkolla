<div align="center">

```
██████╗ ██╗  ██╗ █████╗ ██╗   ██╗ █████╗ ██╗      █████╗ 
██╔══██╗██║  ██║██╔══██╗██║   ██║██╔══██╗██║     ██╔══██╗
██║  ██║███████║███████║██║   ██║███████║██║     ███████║
██║  ██║██╔══██║██╔══██║╚██╗ ██╔╝██╔══██║██║     ██╔══██║
██████╔╝██║  ██║██║  ██║ ╚████╔╝ ██║  ██║███████╗██║  ██║
╚═════╝ ╚═╝  ╚═╝╚═╝  ╚═╝  ╚═══╝  ╚═╝  ╚═╝╚══════╝╚═╝  ╚═╝
```

### `Dhavala Kartikeya Somayaji`
**ML Engineer · Researcher · 2nd Year @ RNSIT · CGPA 9.4**

*I build things that work in production. I research things that push what's possible.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhavalakartikeyasomayaji/)
[![GitHub](https://img.shields.io/badge/GitHub-161B22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Knightkolla)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kartikeyadhavalaofficial@gmail.com)

</div>

```python
dhavala = {
    "currently_building": "FALCON — RL-guided crime localization in surveillance video",
    "obsessed_with":      ["Reinforcement Learning", "Computer Vision", "Scalable backend systems"],
    "belief":             "Understand the math deeply enough, and the engineering gets easier.",
    "mode":               "Research on weekdays. Production on weekends. Sometimes both.",
}
```

> *"Most people use deep learning. I want to understand it well enough to break it."*

## Research Projects

### FALCON — Frame-Aware Crime Localization Agent
`PPO · ViT · Hierarchical Attention · UCF-Crime Dataset`

**Problem:** Surveillance footage can run 45+ hours. Manually scanning it to find where a crime occurred is not feasible at scale — and existing methods process every frame, which is computationally brutal.

**Approach:** Treat it as a search problem. A PPO-based RL agent navigates a low-resolution segment map of the video with a hard budget of 20% of total frames. For each segment it visits, HAFED (a two-scale Vision Transformer) zooms into the full 30fps high-resolution clip and runs frame-level and segment-level attention to score anomaly likelihood. FGlobal then propagates that knowledge to neighboring unvisited segments, so the agent gets smarter without spending its budget. The policy learns to hunt — moving toward high-anomaly regions like a hot-and-cold detector.

```
RAW VIDEO (45hrs)
     ↓ segment @ 1fps low-res
ViT EMBEDDINGS → Global Segment Map
     ↓
PPO AGENT (budget: 20% of segments)
     ↓ on selected segment:
HAFED — frame-level + segment-level attention @ 30fps
     ↓
FGlobal — propagates knowledge to neighboring segments
     ↓
EXACT CRIME FRAME + forensic audit trail
```

**Result:** 4x speedup over brute-force scanning · 95% accuracy on UCF-Crime subset · Shipped as a Flask web app with a full forensic audit trail of the agent's navigation path

### Confidence-Based Early Exit Inference
`PyTorch · Transformers · YAML`

**Problem:** Large Transformer models spend the same compute on every input regardless of difficulty — a simple sample gets the same treatment as a hard one, which is wasteful at scale.

**Approach:** Attached lightweight classifier heads at intermediate layers of the network. During inference, if a layer's prediction confidence crosses a configurable threshold, the model exits early and skips the remaining layers entirely. Trained all exit heads jointly with weighted cross-entropy so each layer learns to be independently useful. Built an automated sweep pipeline that evaluates accuracy vs FLOPs trade-offs across 7 thresholds and reports computational savings against the full-depth baseline.

**Result:** Measurable FLOPs reduction with configurable accuracy trade-off · Fully reproducible via seeded RNGs and YAML-driven config

### Self-Initiated Research Agent
`LangGraph · LangChain · Gemini · Pinecone · Tavily`

**Problem:** Research is slow because it requires a human in the loop at every step — forming questions, finding papers, synthesizing findings, spotting contradictions.

**Approach:** Built a fully autonomous multi-agent system using LangGraph where modular nodes handle query planning, web retrieval, evidence aggregation, and contradiction detection across multi-hop reasoning chains. Grounded outputs in domain-specific knowledge via RAG over a Pinecone vector store to reduce hallucination. The agent self-evaluates its own output quality and iteratively rewrites reports until they meet a coherence threshold — no human needed between runs.

**Result:** End-to-end research pipeline that runs without intervention and produces progressively more coherent structured reports across successive reasoning steps

## Production Work

### ML Engineer Intern — Caprae Capital Partners *(Jul 2025 – Jan 2026)*

Private equity firm needed analysts to search and evaluate thousands of companies faster without sacrificing quality.

- Built an agentic query system over **50k+ company records** on AWS EC2 — analysts can now query conversationally instead of manually, cutting research effort by 40%
- Designed an ML-based company scoring pipeline using real-time web data to standardize senior-level evaluation — 20% faster task completion
- **1st Place / 25 Teams** internal hackathon — keyword-driven niche company discovery microservice shipped directly to production and actively used
- Stack: FastAPI · LangGraph · Flask · Pinecone · Docker · AWS

### SaaS Lead Generation Platform
`FastAPI · React · MongoDB · Docker · Playwright`

**Problem:** B2B lead research is manual, inconsistent, and slow — sales teams waste hours finding and scoring companies by hand.

**Approach:** Built an end-to-end automated company discovery platform that continuously scrapes and collects B2B data from the web, scores each company using Gemini for standardized evaluation, and pushes updates to users in real time via WebSockets so they act on new leads immediately without refreshing. Containerized the entire backend with Docker for consistent deployments across environments.

**Result:** Automated pipeline replacing hours of manual research · Real-time lead visibility · Production-ready containerized deployment

## Stack

**Research & ML**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-8D6EFF?style=flat-square)
![Pinecone](https://img.shields.io/badge/Pinecone-00C4CC?style=flat-square)

**Production & Systems**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

## Beyond the Code

**Google Developer Groups — Technical Lead** *(May 2025 – Present)*
Technical curriculum for 200+ students · Mentored 3 teams to production deployment

**Persona Labs — Co-Founder & CEO** · Co-founded and leading a startup selected from 150+ ideas for official incubation at the RNSIT Incubation Center

**Endorsed by** Zackery Beckham, Co-Founder, Caprae Capital Partners

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Knightkolla&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Knightkolla&theme=tokyonight&hide_border=true&layout=compact" height="165"/>
</div>

<div align="center">
  <img src="https://nirzak-streak-stats.vercel.app/?user=Knightkolla&theme=tokyonight&hide_border=true" height="165"/>
</div>

<div align="center">

*Bengaluru, India · Open to SDE, ML Engineering, and Research internships*

![Profile Views](https://komarev.com/ghpvc/?username=Knightkolla&color=00C9FF&style=flat-square)

</div>
