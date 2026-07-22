<h1 align="center">Md Jahid Hasan</h1>

<h3 align="center">AI Engineer — Agentic Systems · Multi-Agent Workflows · Production ML</h3>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=20&duration=3500&pause=1000&center=true&vCenter=true&width=640&lines=Shipped+production+vision-language+systems;Scaling+geospatial+pipelines+on+AWS;Now+building+reliable+multi-agent+workflows;LangGraph+%C2%B7+LangChain+%C2%B7+Claude+Agent+SDK" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://www.linkedin.com/in/hellojahid/"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="https://medium.com/@hellojahid"><img src="https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white" /></a>
  <a href="https://scholar.google.com/citations?user=7gQWnDMAAAAJ&hl"><img src="https://img.shields.io/badge/Google%20Scholar-4285F4?style=for-the-badge&logo=googlescholar&logoColor=white" /></a>
  <a href="mailto:jahid2rmit@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

---

## 🚧 What I'm Building

My work sits at the convergence of three tracks and the interesting part is where they meet.

```
   🖼️ Computer Vision                📊 Data Science                🤖 Agentic AI
   ───────────────────               ───────────────────            ───────────────────
   PhD × Carsales.com                Research Fellow @ RMIT         Build-in-public series
   CarDNet → GroundingCarDD          Large-scale mobility &         PromptProof → AgentProof
   → CarDVLM (production             geospatial analytics on        → UDA-Hub (LangGraph
   vision-language system)           AWS (PySpark · Sedona)         multi-agent system)
   ✅ shipped                        ✅ in production               ✅ shipped · 🚧 more coming
            \                              |                              /
             \                             |                             /
              └──────────────── 🎯 where I'm headed ────────────────────┘

        Agentic systems that SEE and REASON over data. Vision-language agents
        that inspect, verify, and act. Multi-agent workflows that orchestrate
        data pipelines, ground every claim in evidence, and prove their own
        behaviour through recorded, evaluated trajectories.
```

The agentic track is a **build-in-public series**, with each project documented as it ships.
First came **PromptProof**, a self-correcting prompting engine that fact-checks its own claims.
Then came **AgentProof**, a from-scratch agent runtime with no LangGraph and no CrewAI,
built to master the mechanics of agent loops, tool gating, and evaluation from first principles.
With the fundamentals proven by hand, **UDA-Hub** applies production frameworks, a
**LangGraph and LangChain** multi-agent system built on the Supervisor pattern. Now I'm
extending the series with the **Claude Agent SDK**, applying the same reliability patterns
at the next level of agent autonomy.

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>✈️ <a href="https://github.com/HelloJahid/AgentProof">AgentProof</a></h3>
      <p><i>"PromptProof made prompts trustworthy. AgentProof makes agents measurable."</i></p>
      <p>
        A from-scratch agent runtime with no LangGraph and no CrewAI. Around 1,500 lines of
        readable Python, because the point is to show the mechanics and
        <b>prove</b> they work.
      </p>
      <ul>
        <li><b>State-machine core</b> with typed state (Pydantic), conditional routing, and step budgets so loops can never mean forever</li>
        <li><b>Gate-checked tool use</b> where arguments are validated before the world is touched and responses are validated before the model sees them</li>
        <li><b>Flight recorder</b> writing crash-safe JSONL traces so any run reconstructs fully from its file alone</li>
        <li><b>CI regression gate</b> with golden datasets, a bias-aware LLM-as-judge, and 90+ fully mocked tests needing no keys and no network</li>
      </ul>
      <img src="https://img.shields.io/badge/Agent%20Runtime-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Eval%20Harness-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/LLM--as--Judge-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
    </td>
    <td width="50%" valign="top">
      <h3>🔁 <a href="https://github.com/HelloJahid/PromptProof">PromptProof</a></h3>
      <p><i>Can I trust this output?</i></p>
      <p>
        A self-correcting prompting engine that verifies information instead of
        assuming it. The reliability DNA that AgentProof later inherits.
      </p>
      <ul>
        <li><b>Prompt chaining</b> that decomposes complex questions into focused, verifiable steps</li>
        <li><b>Pydantic gate checks</b> validating every step's output against a schema before the chain continues</li>
        <li><b>Live search grounding</b> so claims are verified against real sources rather than model memory</li>
        <li><b>Evaluator loop</b> where a critic grades the answer and feeds corrections back until it holds up</li>
      </ul>
      <img src="https://img.shields.io/badge/Prompt%20Engineering-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Fact%20Grounding-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Self--Correction-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3>🎛️ <a href="https://github.com/HelloJahid/udahub_solution">UDA-Hub</a></h3>
      <p><i>Multi-agent customer support with LangGraph.</i></p>
      <p>
        The fundamentals proven by hand in AgentProof, now applied with production
        frameworks. A <b>LangGraph-powered multi-agent system</b> that reads,
        reasons, routes, and resolves support tickets end to end.
      </p>
      <ul>
        <li><b>Supervisor pattern</b> across six agents, with the StateGraph built from scratch and no prebuilt agent constructors</li>
        <li><b>Structured classification</b> where a Pydantic schema drives deterministic and fully logged routing rules</li>
        <li><b>RAG with an escalation gate</b> so low retrieval confidence hands off to a human instead of answering ungrounded</li>
        <li><b>Three-tier memory</b> combining typed run state, thread checkpointing, and long-term cross-session memory in SQLAlchemy</li>
      </ul>
      <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
      <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
      <img src="https://img.shields.io/badge/Agentic%20RAG-1f2937?style=flat-square" />
      <img src="https://img.shields.io/badge/Supervisor%20Pattern-1f2937?style=flat-square" />
    </td>
    <td width="50%" valign="top">
      <h3>🚀 <a href="https://github.com/HelloJahid/CICDAgent">CICDAgent</a></h3>
      <p><i>From commit to cloud.</i></p>
      <p>
        Agents that cannot be deployed do not count. An end-to-end DevOps
        showcase, a fully automated GitHub Actions pipeline taking a
        containerised AI agent from a git push all the way to AWS.
      </p>
      <ul>
        <li><b>CI/CD pipeline design</b> covering build, unit and integration testing, and staged deployment through GitHub Actions</li>
        <li><b>Security scanning</b> baked into the pipeline so vulnerabilities are caught before they ship</li>
        <li><b>Keyless authentication</b> to AWS using OpenID Connect, with no long-lived credentials anywhere in the pipeline</li>
        <li><b>Containerisation</b> with Docker and serverless deployment to AWS Lambda</li>
      </ul>
      <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
      <img src="https://img.shields.io/badge/AWS%20Lambda-FF9900?style=flat-square&logo=awslambda&logoColor=white" />
      <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
      <img src="https://img.shields.io/badge/DevSecOps-1f2937?style=flat-square" />
    </td>
  </tr>
</table>

---

## 🎓 Agentic AI Credentials — Certified *and* Built

Frameworks are learned and fundamentals are built. Each credential below is paired with the
open-source work that demonstrates it in practice.

| Credential (Udacity Nanodegree) | Covers | Demonstrated in |
|---|---|---|
| **Agentic AI Engineer with LangChain & LangGraph** | LangGraph agent orchestration, RAG, human-in-the-loop workflows, multi-agent architecture | [UDA-Hub](https://github.com/HelloJahid/udahub_solution) |
| **Agentic AI** | Agent workflows and orchestration patterns, tool calling, state and memory management, multi-agent routing, agentic RAG with evaluation loops | [AgentProof](https://github.com/HelloJahid/AgentProof) |
| **Machine Learning DevOps Engineer** | Production ML pipelines, automated retraining, drift monitoring, CI/CD, API deployment (FastAPI, MLflow, GitHub Actions) | [CICDAgent](https://github.com/HelloJahid/CICDAgent) |
| **Data Scientist** | CRISP-DM, ML pipelines with NLP, recommendation systems, software engineering for data science | [PromptProof](https://github.com/HelloJahid/PromptProof) |

🔗 [Verifiy credentials →](https://www.linkedin.com/in/hellojahid/details/certifications/)

---

## 🧰 Tech Stack

**Agentic & LLM Engineering**

<p>
  <img src="https://img.shields.io/badge/Claude%20Agent%20SDK-191919?style=flat-square&logo=anthropic&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenAI%20SDK-412991?style=flat-square&logo=openai&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square&logo=langchain&logoColor=white" />
  <img src="https://img.shields.io/badge/MCP-1f2937?style=flat-square" />
  <img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat-square&logo=huggingface&logoColor=black" />
  <img src="https://img.shields.io/badge/Pydantic-E92063?style=flat-square&logo=pydantic&logoColor=white" />
  <img src="https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white" />
  <img src="https://img.shields.io/badge/Metaflow-4A6FA5?style=flat-square" />
  <img src="https://img.shields.io/badge/MLflow-0194E2?style=flat-square&logo=mlflow&logoColor=white" />
  <img src="https://img.shields.io/badge/DVC-13ADC7?style=flat-square&logo=dvc&logoColor=white" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" />
  <img src="https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white" />
</p>

**Deep Learning & Data**

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/SQL-4479A1?style=flat-square&logo=mysql&logoColor=white" />
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white" />
  <img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=flat-square&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Keras-D00000?style=flat-square&logo=keras&logoColor=white" />
  <img src="https://img.shields.io/badge/Scikit--learn-F7931E?style=flat-square&logo=scikitlearn&logoColor=white" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" />
  <img src="https://img.shields.io/badge/Pandas-150458?style=flat-square&logo=pandas&logoColor=white" />
  <img src="https://img.shields.io/badge/Weights%20%26%20Biases-FFBE00?style=flat-square&logo=weightsandbiases&logoColor=black" />
</p>

**Cloud & Scale**

<p>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonwebservices&logoColor=white" />
  <img src="https://img.shields.io/badge/Amazon%20SageMaker-1f2937?style=flat-square" />
  <img src="https://img.shields.io/badge/Amazon%20EMR-1f2937?style=flat-square" />
  <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=flat-square&logo=apachespark&logoColor=white" />
  <img src="https://img.shields.io/badge/Apache%20Sedona-8A2BE2?style=flat-square&logo=apache&logoColor=white" />
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" />
</p>

---

## ✍️ Writing

Blog writing when I get time, sharing hands-on projects and what I learn building them.
The build-in-public series is documented as it ships, published in **Towards AI** and
**Stackademic** on [Medium](https://medium.com/@hellojahid).

- **Clever Prompts Are Cheap Now. Reliable LLM Prompting Systems Are the Skill.** — the ideas behind dependable AI
- **Your LLM Lies Confidently. I Built an Engine That Doesn't.** — building the PromptProof engine
- **An Agent You Cannot Watch Is an Agent You Cannot Trust.** — the AgentProof flight recorder
- **Building an Agent Is Cheap Now. Proving It Works Is the Skill.** — grading recorded runs across four dimensions of quality
- **From Commit to Cloud: A Keyless CI/CD Pipeline that Ships an AI Agent to AWS** — the CICDAgent story
- **Git Tracks Your Code. Something Has to Track Your Data. Meet DVC** — hands-on data version control

📝 [Read the full series on Medium →](https://medium.com/@hellojahid)

---

## 🔬 Research Credibility

The engineering is backed by an applied AI research track record. I completed an
**industry-embedded PhD** (RMIT University × Carsales.com Ltd, awarded May 2026)
shipping production vision-language systems, and I currently work as a **Research Fellow
in Data Science & Geospatial Analytics** at RMIT, building cloud-native analytics
pipelines for the iMOVE Australia Advanced Air Mobility programme.

- 🏭 **CarDVLM**, an end-to-end vision-language model for automated vehicle damage
  assessment deployed in production, cutting assessment time from 20 minutes to 6
- 📐 **CarDamageEval**, a standardised benchmark for VLM-based damage assessment
  (*AusDM 2025*)
- 📖 **Systematic literature review** of AI vehicle damage detection in
  *WIREs Data Mining & Knowledge Discovery* (Q1, IF 11.7)
- 🧠 **SSPANet**, attention-based explainable deep learning for brain tumour
  classification in *Biomedical Signal Processing and Control* (Q1, IF 4.9)
- 🎯 **GroundingCarDD**, text-guided multimodal phrase grounding in *IEEE Access* (Q1)

📚 ~500 citations · h-index 12 · [Full list on Google Scholar](https://scholar.google.com/citations?user=7gQWnDMAAAAJ&hl)

---

## 📊 GitHub Stats

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=HelloJahid&show_icons=true&theme=default&hide_border=true&count_private=true" />
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=HelloJahid&layout=compact&hide_border=true&langs_count=8" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com/?user=HelloJahid&hide_border=true" />
</p>

---

<p align="center">
  <i>📍 Melbourne, Australia · Open to collaboration on agentic systems, multi-agent workflows, and applied AI research</i>
</p>
