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
