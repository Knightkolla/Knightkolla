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
**Builder · Researcher · 2nd Year @ RNSIT · CGPA 9.4**

*I don't just study ML — I ship it.*

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/dhavalakartikeyasomayaji/)
[![GitHub](https://img.shields.io/badge/GitHub-161B22?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Knightkolla)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:kartikeyadhavalaofficial@gmail.com)

</div>

---

## What I'm About

```python
dhavala = {
    "currently_building": "FALCON — RL-guided crime localization in surveillance video",
    "obsessed_with":      ["Reinforcement Learning", "Computer Vision", "Systems that scale"],
    "belief":             "Go deep on the math. The creativity follows.",
    "status":             "2nd year undergrad shipping production ML",
    "founded":            "Persona Labs @ RNSIT Incubation Center",
}
```

> *"Most people use deep learning. I want to understand it well enough to break it."*

---

## FALCON — My Flagship Project

<div align="center">

**Frame-Aware Crime Localization Agent**
`PPO · ViT · Hierarchical Attention · UCF-Crime Dataset`

</div>

**The problem:** You have a 45-hour surveillance recording. A crime happened somewhere. Finding it frame-by-frame is impossible at scale.

**What FALCON does:** An RL agent navigates the video like a detective seeing only **20% of frames**  and pinpoints the exact crime onset in **2–4 minutes**.

```
┌─────────────────────────────────────────────────────────────┐
│  RAW VIDEO (45hrs)                                          │
│       ↓ segment into 10-frame chunks @ 1fps low-res        │
│  ViT EMBEDDINGS ──→ Global Segment Map                      │
│       ↓                                                     │
│  PPO AGENT navigates map (budget: 20% of segments)         │
│       ↓ on selected segment:                               │
│  HAFED (Hierarchical Attention)                             │
│    ├── Frame-level attention  @ 30fps high-res             │
│    └── Segment-level gating → anomaly score                │
│       ↓                                                     │
│  FGlobal propagates knowledge to neighboring segments       │
│       ↓                                                     │
│  EXACT CRIME FRAME + forensic audit trail                 │
└─────────────────────────────────────────────────────────────┘
```

**Results on UCF-Crime (13 categories, 1,900 videos):**
-  **4× speedup** over brute-force scanning
-  **95% accuracy** on test subset
-  Shipped as Flask web app with full agent navigation trail

---

## Projects

### Self-Initiated Research Agent
`LangGraph · LangChain · Gemini · Pinecone · Tavily`

Autonomous multi-agent system that **formulates its own research questions**, retrieves literature, detects contradictions across multi-hop chains, and writes structured reports  without human intervention. Self-evaluates and iteratively refines outputs.

---

### Confidence-Based Early Exit Inference
`PyTorch · Transformers · YAML`

Attached lightweight classifier heads at intermediate Transformer layers. Model exits early when confidence exceeds threshold — trades FLOPs for speed automatically. Automated sweep pipeline benchmarks 7 thresholds against full-depth baseline.

---

### SaaS Lead Generation Platform
`FastAPI · React · MongoDB · Docker · Playwright`

End-to-end B2B company discovery platform with real-time WebSocket updates, Gemini-powered automated scoring, and containerized deployment. Built and shipped to production during internship at **Caprae Capital Partners**.

---

## Experience

**Machine Learning Engineer Intern — Caprae Capital Partners** *(Jul 2025 – Jan 2026)*
- Agentic query system over **50k+ company records** → 40% reduction in manual research
- ML scoring pipeline → 20% faster task completion
- ** 1st Place / 25 Teams** — internal hackathon, shipped to production

**Co-Organizer (Technical Lead) — Google Developer Groups** *(May 2025 – Present)*
- Technical curriculum for **200+ students**
- Mentored 3 teams end-to-end to deployed ML projects

**Founder — Persona Labs** *(RNSIT Incubation Center)*
- Selected from **150+ startup ideas** for official institutional incubation

---

## Stack

<div align="center">

**ML / Research**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikit-learn&logoColor=white)
![LangGraph](https://img.shields.io/badge/LangGraph-8D6EFF?style=flat-square)
![Pinecone](https://img.shields.io/badge/Pinecone-00C4CC?style=flat-square)

**Backend & Systems**

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)

**Frontend & Data**

![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white)

</div>

---

## GitHub Stats

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Knightkolla&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true" height="170"/>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Knightkolla&theme=tokyonight&hide_border=true&layout=compact" height="170"/>
</div>

<div align="center">
  <img src="https://nirzak-streak-stats.vercel.app/?user=Knightkolla&theme=tokyonight&hide_border=true" height="170"/>
</div>

---

## What I'm After

I'm not here to fine-tune pretrained models on Kaggle datasets.

I want to work on problems where the architecture itself is the research where getting to the right answer means going back to the math and questioning assumptions the field takes for granted. Generalization, sample efficiency, and the gap between what LLMs appear to do and what they actually do that's the territory I want to work in.

If you're building something in that space, let's talk.

---

<div align="center">

**`kartikeyadhavalaofficial@gmail.com`**

*Bengaluru, India · Open to research internships*

![Profile Views](https://komarev.com/ghpvc/?username=Knightkolla&color=00C9FF&style=flat-square)

</div>
