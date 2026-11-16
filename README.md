# PaceMind---SCSE3103-Group02
SCSE3103 Cognitive Computing Prototype
<div align="center">

### Explainable Academic Workload & Burnout Risk Advisor

![Course](https://img.shields.io/badge/Course-SCSE3103_Cognitive_Computing-1a365d?style=for-the-badge)
![University](https://img.shields.io/badge/UTM-Faculty_of_Computing-800000?style=for-the-badge)
![Session](https://img.shields.io/badge/Session-2026%2F2027_Sem_1-2b6cb0?style=for-the-badge)

![Python](https://img.shields.io/badge/Python-3.11-3776AB?style=flat-square&logo=python&logoColor=white)
![Fuzzy Logic](https://img.shields.io/badge/Engine-Mamdani_Fuzzy_Logic-008080?style=flat-square)
![Rule Engine](https://img.shields.io/badge/Reasoning-YAML_Production_Rules-6B46C1?style=flat-square)
![Streamlit](https://img.shields.io/badge/UI-Streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=white)
![Status](https://img.shields.io/badge/Phase_1-Proposal_Submitted-2F855A?style=flat-square)

*An interpretable cognitive decision-support prototype that models imprecise student workload indicators and generates transparent, actionable study and recovery advice.*

</div>

---

## Project Overview

University students frequently face overlapping deadlines, irregular sleep schedules, and fluctuating stress levels. Traditional tracking apps rely on rigid binary cutoffs (e.g., hard `if-else` thresholds) that fail near boundary values and offer little explanation.

**PaceMind** bridges this gap using a hybrid **Cognitive Computing** architecture:
* 🟦 **Mamdani Fuzzy Inference System (`scikit-fuzzy`):** Evaluates four continuous inputs (*weekly study hours, nightly sleep, upcoming 14-day deadlines, and self-rated stress*) anchored to MQA[cite: 40] and National Sleep Foundation guidelines to compute a smooth **Burnout Risk Score (0–100)**.
* 🟪 **Transparent Rule-Based Engine (`YAML` + Python):** Maps fuzzy risk levels and student context into tailored, human-readable study pacing and recovery recommendations.
* 🟩 **Explainable & Interactive UI (`Streamlit` + `Matplotlib`):** Visualizes active fuzzy membership degrees, fired `IF-THEN` rules, and an interactive **"What-If" simulator** so students can test schedule adjustments safely.

---

## Team Roster & Role Allocation — Group `[XX]`

| Member Name | Matric No. | Primary Role | Key Responsibilities |
| :--- | :--- | :--- | :--- |
| **[FATIMA YOUSRA]** | `A24CS0011` | **Project Management & Architecture** | Timeline governance, GitHub workflow, system integration, and report compilation |
| **[Member 2 Name]** | `A2XECXXXX` | **Knowledge & Fuzzy Engineering** | Membership functions (MQA/sleep anchors), Mamdani controller, and sensitivity analysis |
| **[Member 3 Name]** | `A2XECXXXX` | **Rule Engine & UI Implementation** | YAML production rules, Streamlit dashboard, Matplotlib plots, and input validation |
| **[Member 4 Name]** | `A2XECXXXX` | **Testing, Evaluation & Ethics** | Synthetic profiles (40+ cases), crisp-baseline comparison (`pytest`), and Responsible AI checks |

---

## 🗂️ Repository Structure

```text
SCSE3103-GroupXX-LoadSense/
├── src/            # Core Mamdani fuzzy scorer, rule engine, and Streamlit app
├── rules/          # Version-controlled YAML IF-THEN recommendation rule base
├── data/           # Non-PII synthetic student profiles for baseline evaluation
├── tests/          # Automated pytest suites (normal, boundary, and invalid cases)
├── docs/           # Project Proposal, Design Report, and contribution logs
└── requirements.txt
