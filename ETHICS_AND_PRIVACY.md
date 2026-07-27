# Planned Research Ethics and Privacy Requirements

This document specifies safeguards for a **future research instrument and intervention**. It does not certify that the present repository is a GDPR-compliant deployment environment or that the listed technical controls have already been implemented.

## Required approvals and governance

Before participant deployment, the study should:

- obtain the applicable University of Jyväskylä ethical and data-protection approvals;
- follow Finnish Research Integrity (TENK) guidance and applicable GDPR requirements;
- document the AI provider, processing purposes, retention arrangements, data location and subprocessors;
- define lawful basis, controller/processor responsibilities, access controls, retention periods and deletion procedures;
- conduct a data-protection impact assessment if required by the final design.

## Participant protection

Participation should be voluntary and based on documented informed consent, with an unconditional right to withdraw in accordance with the approved protocol. Recruitment and study procedures should account for war, displacement and instability without inferring trauma or other protected characteristics from AI interactions.

Consent and contact records should be stored separately from research data. Information should be provided in an accessible language, including Ukrainian or Russian where required by the approved recruitment and consent procedure.

## Data minimization and separation

A future implementation should:

- assign pseudonymous participant and session identifiers;
- keep identity, contact and consent records separate from intervention data;
- separate raw conversational data from derived analytical metadata;
- avoid sending unnecessary demographic information to the language model;
- restrict access according to documented research roles;
- avoid public release of raw conversations unless separately justified ethically and legally;
- publish only anonymized, aggregated or otherwise non-identifying outputs where permitted.

## AI-specific safeguards

The final instrument should address inaccurate explanations, bias, model drift, provider changes and measurement contamination through:

- researcher-approved instructional modules wherever feasible;
- expert linguistic review and pilot testing;
- versioned prompts, models, modules and system configurations;
- structured logging of every intervention session;
- monitoring against predefined pedagogical-fidelity criteria;
- human validation of automated behavioral annotations;
- separate instructional and standardized assessment modes;
- independent outcome measurement.

Pinned model snapshots or securely hosted open-weights models may be considered, subject to institutional security, feasibility and data-protection review. No architecture should be described as guaranteeing absolute longitudinal reproducibility.

## Current repository limitation

The present repository documents these requirements only. It does not yet implement participant onboarding, consent management, pseudonymization, secure storage, automated logging, drift monitoring or a university-approved API environment.
