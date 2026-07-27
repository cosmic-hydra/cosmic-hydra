<div align="center">

<picture>
  <source media="(max-width: 700px)" srcset="./assets/readme/hero-mobile.svg">
  <img
    src="./assets/readme/hero.svg"
    width="100%"
    alt="Advaith Vaithianathan — software engineer and founder building verifiable AI systems, quantitative infrastructure, and scientific tools."
  >
</picture>

<br>

<a href="https://www.linkedin.com/in/advaithvaithianathan">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="https://orcid.org/0009-0000-2076-3011">
  <img src="https://img.shields.io/badge/ORCID-A6CE39?style=flat&logo=orcid&logoColor=white" alt="ORCID">
</a>
<a href="mailto:advaithv.av7@gmail.com">
  <img src="https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white" alt="Email">
</a>
<a href="https://github.com/cosmic-hydra">
  <img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white" alt="GitHub">
</a>

</div>

<br>

```text
╔══════════════════════════════════════════════════════════════════════╗
║                                                                      ║
║   ██████╗ ██████╗ ███████╗███╗   ███╗██╗ ██████╗    ██╗  ██╗   ██╗   ║
║  ██╔════╝██╔═══██╗██╔════╝████╗ ████║██║██╔════╝    ██║  ╚██╗ ██╔╝   ║
║  ██║     ██║   ██║███████╗██╔████╔██║██║██║         ███████╗╚████╔╝    ║
║  ██║     ██║   ██║╚════██║██║╚██╔╝██║██║██║         ██╔══██║ ╚██╔╝     ║
║  ╚██████╗╚██████╔╝███████║██║ ╚═╝ ██║██║╚██████╗    ██║  ██║  ██║      ║
║   ╚═════╝ ╚═════╝ ╚══════╝╚═╝     ╚═╝╚═╝ ╚═════╝    ╚═╝  ╚═╝  ╚═╝      ║
║                                                                      ║
║  software engineer · founder · bengaluru                             ║
║  applied AI · quantitative systems · scientific computing            ║
║                                                                      ║
╚══════════════════════════════════════════════════════════════════════╝
```

```text
  about
  ─────
  I build at the intersection of applied AI, quantitative systems,
  scientific computing, and product engineering.

  The projects here share a consistent thesis: that the most impactful
  systems in AI, science, and finance benefit from determinism where it
  matters, rigorous evaluation, clean interfaces, and composable
  primitives over monolithic frameworks.
```

<br>

```text
  ecosystem
  ─────────
```

```mermaid
%%{init: {'theme': 'base', 'themeVariables': { 'primaryColor': '#0a1a18', 'primaryTextColor': '#e0e0e0', 'primaryBorderColor': '#2a5a50', 'lineColor': '#3a8a78', 'secondaryColor': '#0f2420', 'tertiaryColor': '#06120f', 'fontSize': '14px' }}}%%
graph TB
    subgraph core["ai & memory"]
        zeroH["zeroH<br/>grounded agents"] -->|"powers"| zane
        zeroH -->|"informs"| concepts
    end
    subgraph science["science & pharma"]
        zane["ZANE<br/>molecular engineering"]
    end
    subgraph infra["infrastructure"]
        vecomp["vecomp<br/>vector index"]
        tetra["Tetra Quant<br/>quant research"]
    end
    subgraph platform["platform"]
        hf["Hydra Fund<br/>investment OS"]
    end
    zane -->|"feeds into"| hf
    tetra -->|"feeds into"| hf
    vecomp -->|"supports"| zeroH
    style core fill:#0a1a18,stroke:#2a5a50,color:#e0e0e0
    style science fill:#0a1a18,stroke:#2a5a50,color:#e0e0e0
    style infra fill:#0a1a18,stroke:#2a5a50,color:#e0e0e0
    style platform fill:#0a1a18,stroke:#2a5a50,color:#e0e0e0
    style zeroH fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    style zane fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    style vecomp fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    style tetra fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    style hf fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    style concepts fill:#0f2420,stroke:#3a8a78,color:#e0e0e0
    linkStyle default stroke:#3a8a78,stroke-width:1px
```

<br>

```text
  projects
  ────────
```

<br>

<!-- zeroH -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <a href="https://github.com/cosmic-hydra/zeroH">
        <img src="https://img.shields.io/badge/zeroH-000000?style=for-the-badge&logo=python&logoColor=white" alt="zeroH">
      </a>
      <br><br>
      <sub><em>Zero Hallucination for AI agents</em></sub>
      <br><br>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
      <br>
      <img src="https://img.shields.io/badge/SQLite-003B57?style=flat&logo=sqlite&logoColor=white" alt="SQLite">
    </td>
    <td valign="top">
      <br>
      A standard-library-first Python layer for grounded memory, retrieval, claim verification, citations, and abstention. Bring your own LLM — any API or local provider — and zeroH wraps it with a deterministic <strong>verify-reask-abstain</strong> loop that pushes hallucination rates toward zero.
      <br><br>
      Durable SQLite-backed memory, sentence-aware chunking, confidence scoring, and citation emission — all pure Python with zero heavyweight ML dependencies.
      <br><br>
      <details>
        <summary>architecture</summary>
        <br>
        <pre>
query ──► retrieve ──► augment ──► [LLM] ──► verify ──► answer
                          ▲                    │
                          └──── re-ask ─────────┘
                               or abstain
        </pre>
      </details>
    </td>
  </tr>
</table>

<br>

<!-- ZANE -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <a href="https://github.com/cosmic-hydra/zane">
        <img src="https://img.shields.io/badge/ZANE-000000?style=for-the-badge&logo=python&logoColor=white" alt="ZANE">
      </a>
      <br><br>
      <sub><em>Pharma OS for Autonomous Molecular Engineering</em></sub>
      <br><br>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
      <br>
      <img src="https://img.shields.io/badge/AMD-ED760E?style=flat&logo=amd&logoColor=white" alt="AMD">
      <img src="https://img.shields.io/badge/NVIDIA-76B900?style=flat&logo=nvidia&logoColor=white" alt="NVIDIA">
    </td>
    <td valign="top">
      <br>
      AI-native pharmaceutical operating system unifying target intelligence, molecule generation, free-energy physics, preclinical safety triage, compliance telemetry, and lab execution interfaces into a single orchestration-grade runtime.
      <br><br>
      Funded by <strong>AMD</strong> and <strong>NVIDIA</strong>. Every molecular decision is generated, stress-tested, and cryptographically auditable through governed decision gates.
    </td>
  </tr>
</table>

<br>

<!-- vecomp -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <a href="https://github.com/cosmic-hydra/vecomp">
        <img src="https://img.shields.io/badge/vecomp-000000?style=for-the-badge&logo=rust&logoColor=white" alt="vecomp">
      </a>
      <br><br>
      <sub><em>Vector compression via TurboQuant</em></sub>
      <br><br>
      <img src="https://img.shields.io/badge/Rust-000000?style=flat&logo=rust&logoColor=white" alt="Rust">
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
    </td>
    <td valign="top">
      <br>
      A vector index written in <strong>Rust</strong> with Python bindings that shrinks high-dimensional embedding footprints to roughly <strong>2GB</strong> for practical-scale corpora. Exploration into quantization-aware retrieval for resource-constrained deployment.
    </td>
  </tr>
</table>

<br>

<!-- Tetra Quant -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <a href="https://github.com/cosmic-hydra/tetra-quant">
        <img src="https://img.shields.io/badge/Tetra%20Quant-000000?style=for-the-badge&logo=python&logoColor=white" alt="Tetra Quant">
      </a>
      <br><br>
      <sub><em>Quantitative trading research infrastructure</em></sub>
      <br><br>
      <img src="https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
    </td>
    <td valign="top">
      <br>
      Pipeline-driven data ingestion, strategy backtesting, and signal analysis built on the <strong>OpenBB</strong> platform for systematic research.
    </td>
  </tr>
</table>

<br>

<!-- Concepts -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <a href="https://github.com/cosmic-hydra/Concepts">
        <img src="https://img.shields.io/badge/Concepts-000000?style=for-the-badge&logo=markdown&logoColor=white" alt="Concepts">
      </a>
      <br><br>
      <sub><em>AI-native note-taking with PNAS-backed retrieval</em></sub>
      <br><br>
      <img src="https://img.shields.io/badge/Markdown-000000?style=flat&logo=markdown&logoColor=white" alt="Markdown">
    </td>
    <td valign="top">
      <br>
      Personal knowledge management that applies grounding and verification primitives from agentic systems to daily notes and ideas.
    </td>
  </tr>
</table>

<br>

<!-- Hydra Fund -->
<table>
  <tr>
    <td width="200" align="center" valign="top">
      <br>
      <img src="https://img.shields.io/badge/Hydra%20Fund-000000?style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIyNCIgaGVpZ2h0PSIyNCIgdmlld0JveD0iMCAwIDI0IDI0IiBmaWxsPSJub25lIiBzdHJva2U9IndoaXRlIiBzdHJva2Utd2lkdGg9IjIiIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIgc3Ryb2tlLWxpbmVqb2luPSJyb3VuZCI+PHBvbHlsaW5lIHBvaW50cz0iMjIgMTIgMTggMTIgMTUgMjEgOSAzIDYgMTIgMiAxMiIvPjwvc3ZnPg==" alt="Hydra Fund">
      <br><br>
      <sub><em>AI-native investment platform</em></sub>
    </td>
    <td valign="top">
      <br>
      Software and research infrastructure for an AI-native investment and venture platform. Portfolio analytics, market data pipelines, and the research stack underpinning systematic decision-making.
    </td>
  </tr>
</table>

<br>

```text
  toolbox
  ───────
```

<br>

<div align="center">

<a href="#">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white" alt="Swift">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go">
</a>

<br><br>

<a href="#">
  <img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" alt="React">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=next.js&logoColor=white" alt="Next.js">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/OpenBB-0081CB?style=for-the-badge&logoColor=white" alt="OpenBB">
</a>

<br><br>

<a href="#">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/SQLite-003B57?style=for-the-badge&logo=sqlite&logoColor=white" alt="SQLite">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker">
</a>
<a href="#">
  <img src="https://img.shields.io/badge/AWS-FF9900?style=for-the-badge&logo=amazonwebservices&logoColor=white" alt="AWS">
</a>

</div>

<br>

```text
  operating principles
  ────────────────────
```

<br>

```text
  ┌─────────────────────────────────────────────────────────────────┐
  │  determinism over heuristics                                    │
  │  stochasticity is a tool, not a default                         │
  │  ── especially in evaluation, retrieval, and agent behavior     │
  ├─────────────────────────────────────────────────────────────────┤
  │  composable over monolithic                                     │
  │  small, standard-library-first primitives                       │
  │  ── inspired by the Unix philosphy applied to AI systems        │
  ├─────────────────────────────────────────────────────────────────┤
  │  evaluate honestly                                              │
  │  benchmarks that measure what matters                           │
  │  ── citation-grounding verification, abstention rates, gaps     │
  ├─────────────────────────────────────────────────────────────────┤
  │  ship real things                                               │
  │  applied research that produces software people can use         │
  │  ── not papers that produce more papers                         │
  └─────────────────────────────────────────────────────────────────┘
```

<br>

```text
  activity
  ────────
```

<br>

<div align="center">

<a href="https://github.com/cosmic-hydra">
  <img src="https://github-readme-stats.vercel.app/api?username=cosmic-hydra&show_icons=true&count_private=true&hide_border=true&bg_color=0d1117&title_color=3a8a78&icon_color=3a8a78&text_color=c9d1d9" width="49%" alt="GitHub stats">
</a>
<a href="https://github.com/cosmic-hydra">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=cosmic-hydra&layout=compact&hide_border=true&bg_color=0d1117&title_color=3a8a78&text_color=c9d1d9" width="49%" alt="Top languages">
</a>

</div>

<br>

```text
  connect
  ───────
```

<br>

<div align="center">

<a href="https://www.linkedin.com/in/advaithvaithianathan">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn">
</a>
<a href="mailto:advaithv.av7@gmail.com">
  <img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email">
</a>
<a href="https://github.com/cosmic-hydra">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub">
</a>

<br><br>

<sub>last updated 2026 · cosmic-hydra</sub>

</div>
