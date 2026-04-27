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

---

```python
dhavala = {
    "currently_building": "FALCON — RL-guided crime localization in surveillance video",
    "obsessed_with":      ["Reinforcement Learning", "Computer Vision", "Scalable backend systems"],
    "belief":             "Understand the math deeply enough, and the engineering gets easier.",
    "mode":               "Research on weekdays. Production on weekends. Sometimes both.",
}
```

> *"Most people use deep learning. I want to understand it well enough to break it."*

---

## Research Projects

### FALCON — Frame-Aware Crime Localization Agent
`PPO · ViT · Hierarchical Attention · UCF-Crime Dataset`

An RL agent that finds the exact crime frame in a 45-hour surveillance video by inspecting only **20% of frames** — in under 4 minutes.

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

- 4x speedup over brute-force · 95% accuracy on UCF-Crime subset · Shipped as Flask web app

---

### Confidence-Based Early Exit Inference
`PyTorch · Transformers`

Lightweight classifier heads at intermediate Transformer layers — model exits early when confidence clears a threshold. Automated sweep across 7 thresholds benchmarks accuracy vs FLOPs against full-depth baseline.

---

### Self-Initiated Research Agent
`LangGraph · LangChain · Gemini · Pinecone`

Autonomous multi-agent system that formulates its own research questions, retrieves literature, detects contradictions across multi-hop chains, and iteratively refines structured reports without human intervention.

---

## Production Work

### ML Engineer Intern — Caprae Capital Partners *(Jul 2025 – Jan 2026)*

- Agentic query system over **50k+ company records** deployed on AWS EC2 — 40% reduction in manual research effort
- ML-based company scoring pipeline using real-time web data — 20% faster task completion
- **1st Place / 25 Teams** internal hackathon — microservice shipped directly to production
- Stack: FastAPI · LangGraph · Flask · Pinecone · Docker · AWS

### SaaS Lead Generation Platform
`FastAPI · React · MongoDB · Docker · Playwright`

End-to-end B2B company discovery platform with real-time WebSocket updates, Gemini-powered scoring, and containerized deployment.

---

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

---

## Beyond the Code

**Google Developer Groups — Technical Lead** *(May 2025 – Present)*
Technical curriculum for 200+ students · Mentored 3 teams to production deployment

**Persona Labs — Founder** · Selected from 150+ ideas for RNSIT Incubation Center

**Endorsed by** Zackery Beckham, Co-Founder, Caprae Capital Partners

---

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Knightkolla&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" height="165"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Knightkolla&theme=tokyonight&hide_border=true&layout=compact" height="165"/>
</div>

<div align="center">
  <img src="https://nirzak-streak-stats.vercel.app/?user=Knightkolla&theme=tokyonight&hide_border=true" height="165"/>
</div>

---

<div align="center">

*Bengaluru, India · Open to SDE, ML Engineering, and Research internships*

![Profile Views](https://komarev.com/ghpvc/?username=Knightkolla&color=00C9FF&style=flat-square)

</div>
