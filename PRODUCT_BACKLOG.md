# Product Backlog

## Product goal

Develop an auditable research instrument for testing strategically restricted Ukrainian- or Russian-mediated metalinguistic scaffolding with adult English learners in Ukraine.

This is an ordered Scrum product backlog. Story points are relative estimates, not evidence of pedagogical effectiveness.

| Order | Product backlog item | Priority | Points | Acceptance criteria |
|---:|---|---|---:|---|
| 1 | Write the research-instrument specification | P0 | 8 | Tutor behaviour, comparison condition, outcomes, exclusions and limitations are documented. |
| 2 | Define the instructional state machine | P0 | 8 | Explanation → hint → L2 elicitation → independent production is explicit and testable. |
| 3 | Define L1-support triggers | P0 | 5 | L1 assistance occurs only after approved triggers such as failed repair or learner request. |
| 4 | Develop provisional language modules | P0 | 13 | Copula, article and tense-aspect modules contain researcher-approved multilingual explanations. |
| 5 | Conduct expert linguistic review | P0 | 8 | Specialists approve or revise each explanation before learner testing. |
| 6 | Implement the minimal tutor | P0 | 13 | A learner can complete a versioned module with English-default interaction and restricted L1 assistance. |
| 7 | Implement structured logging | P0 | 8 | Logs record triggers, feedback, L1 function, repair, agency events and timestamps. |
| 8 | Implement configuration versioning | P0 | 5 | Every session records model, prompt, module and system versions. |
| 9 | Separate raw and derived data | P0 | 8 | Conversations and analytical annotations are stored separately with access controls. |
| 10 | Implement pseudonymous identifiers | P0 | 5 | Participant and session IDs do not directly reveal identity. |
| 11 | Build human annotation tools | P0 | 13 | Researchers can validate feedback, repair, L1 use and learner-agency annotations. |
| 12 | Create tutor and assessment modes | P0 | 8 | Assessment mode disables L1 scaffolding, hints and corrective teaching feedback. |
| 13 | Develop standardized assessment tasks | P1 | 13 | Tasks have versioned administration procedures and independent rating criteria. |
| 14 | Select the autonomy instrument | P1 | 8 | A validated measure is selected, adapted where necessary and pilot-tested. |
| 15 | Implement consent and withdrawal workflows | P0 | 8 | Approved consent, withdrawal and deletion procedures are documented and testable. |
| 16 | Complete provider and GDPR assessment | P0 | 8 | Processing, retention, data location and subprocessors are documented. |
| 17 | Add model-drift monitoring | P1 | 8 | Defined tests detect changes in feedback, L1 use and instructional fidelity. |
| 18 | Build a pilot-validation dataset | P1 | 13 | Representative interactions are human-coded for quality, safety and annotation accuracy. |
| 19 | Conduct usability pilot testing | P1 | 13 | Target adult users complete modules without unsupported effectiveness claims. |
| 20 | Validate automated annotations | P1 | 8 | Candidate annotations are compared with human coding and reliability is reported. |
| 21 | Add intervention administration tools | P2 | 13 | Researchers can assign conditions, schedule sessions and monitor completion. |
| 22 | Add pseudonymous research exports | P2 | 5 | Process data exports retain version and provenance information. |
| 23 | Add automated testing and CI | P1 | 8 | Pedagogical rules, privacy boundaries, logging and mode separation are regression-tested. |
| 24 | Prepare pilot-release documentation | P1 | 8 | Deployment, ethics, module, coding and incident-response documentation is complete. |

## First functional POC

The minimum credible functional POC requires items 1–12, 15, 16 and 23. Completion permits the description **functional but unvalidated prototype**. It does not permit claims of effectiveness or status as a validated research instrument.

## Definition of done

An item is done only when:

- its acceptance criteria are satisfied;
- relevant tests pass;
- pedagogical and research assumptions are documented;
- model, prompt, module and configuration versions are recorded;
- privacy, ethics and participant-safety implications are reviewed;
- another researcher can reproduce or audit the result;
- the README distinguishes implemented and planned functionality accurately.

Software completion, linguistic validation, ethical approval and empirical validation are separate milestones.
## Research-plan synchronisation epic (v1.1)

These items are required by the current Jyväskylä research plan and join the pilot-release gate.

### ALT-21 — Matched L1-mediated and L2-only conditions
**Priority:** P0  
**Acceptance criteria:**
- Two versioned profiles implement `ai_l1_metalinguistic` and `ai_l2_only_comparison`.
- Modules, target forms, written tasks, scheduled time and non-L1 feedback opportunities are matched.
- Assigned and delivered condition, L1 exposure, fidelity status and deviations are logged.
- Automated tests demonstrate that L1 scaffolding cannot leak into the L2-only condition or assessment mode.

### ALT-22 — Participant language profile, allocation and dosage
**Priority:** P0  
**Acceptance criteria:**
- `principal_support_language`, reported multilingual background, support-language preference and dated changes replace a single essentialising L1 field.
- Language is never inferred from nationality, citizenship, residence or name.
- Allocation supports stratification by baseline A2–B1 proficiency and principal support language, plus a documented matched quasi-experimental fallback.
- Dose is configurable with a proposal default of two sessions weekly for 10–12 weeks; scheduled/completed sessions, duration, missed-session reasons and protocol deviations are exportable.

### ALT-23 — Standardised written assessment and blind rating
**Priority:** P0  
**Acceptance criteria:**
- Baseline/post tasks use parallel piloted written-task forms with fixed prompts and standardised administration metadata.
- Functional adequacy stores content, task requirements, comprehensibility and coherence using a versioned Kuiken–Vedder-aligned rubric.
- Independent pre-adjudication ratings retain rater ID, blinded status, scale version and reliability-ready data.
- Condition and time point are hidden from raters where feasible.

### ALT-24 — Autonomy-instrument adaptation and behaviour
**Priority:** P0  
**Acceptance criteria:**
- Nguyen and Habók remains a candidate pending construct-fit review for adult learners and the Ukrainian context.
- Ukrainian and Russian versions support forward/back translation, cognitive interviews and pilot records; invariance results are stored where sample size permits.
- Logs add persistence without assistance, voluntary scaffold reduction, optional scaffold uptake, independent completion and declared external help.
- Behavioural events are never emitted as validated autonomy scores.

### ALT-25 — Contamination, attrition and analysis populations
**Priority:** P0  
**Acceptance criteria:**
- Store external AI/help, cross-condition exposure and frequency without punitive labelling.
- Store withdrawal, attrition category, volunteered reason, missingness reason and analysis population.
- Preserve original assignment and support intention-to-treat and per-protocol exports.
- Produce a long-form mixed-effects-ready export with participant, task, time, condition, support language, baseline proficiency, dose, assessor, outcome dimensions and version fields.

### ALT-26 — Security and verified deletion
**Priority:** P0  
**Acceptance criteria:**
- Document encryption in transit/at rest, role-based access, audit logging and retention.
- Withdrawal/deletion propagates through transcripts, event logs and link tables as permitted by protocol and produces a verifiable audit result.
- Pilot release is blocked until condition, assessment, contamination, adherence, attrition and export fixtures pass.
