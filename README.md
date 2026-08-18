# AI Language Tutor — Proof of Concept & Research Specification

This repository contains the exploratory architecture, technical specifications, and data logging protocols for a doctoral intervention study at the University of Jyväskylä.

## Research Overview
* **Project Title:** AI-Assisted Metalinguistic Instruction and Learner Autonomy in Adult English Learning in Ukraine
* **Primary Objective:** To investigate whether an AI tutor using strategically restricted L1 mediation and contrastive metalinguistic scaffolding supports learner autonomy and functional L2 performance.
* **Target Audience:** Adult English learners in Ukraine.

## Key Architectural Principles
* **English-Default Policy:** The tutor interacts in English by default, using Ukrainian/Russian L1 support only when triggered by repeated errors, failed repair, or explicit learner requests (`/config/tutor_mode.json`).
* **Scaffold Fading:** Systematically steps down assistance from full contrastive explanations to metalinguistic hints, L2 elicitations, and independent production.
* **Separation of Modes:** Distinguishes instructional teaching mode (`/config/tutor_mode.json`) from unassisted outcome assessment mode (`/config/assessment_mode.json`).
* **Auditability & Version Control:** All model releases, prompts, system configurations, and module checkpoints are strictly versioned to safeguard against third-party API model drift.

## Data Governance & Ethics Compliance
* **GDPR & TENK Compliance:** Personal participant identities are strictly separated from interaction logs. All sessions are logged using pseudonymous user IDs.
* **Human Validation:** Automated process classifications (e.g., self-repair or learner autonomy events) are logged as candidate annotations (`/schema/interaction_log.json`) and validated against human coding.
