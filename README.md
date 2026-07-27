# AI Language Tutor POC

## Status

This repository is an **exploratory prototype specification and research-software foundation** for an AI-assisted English-learning intervention. It does not currently contain a developed, validated or deployed tutor, and it is not an autonomous assessment system.

No participant study is being conducted through this repository. Claims about pedagogical effectiveness, learner autonomy, functional English performance, GDPR compliance or longitudinal reproducibility require later implementation, institutional review, expert validation and pilot testing.

## Research purpose

The proposed intervention investigates whether strategically restricted Ukrainian- or Russian-mediated contrastive metalinguistic scaffolding can support learner autonomy and functional English performance among adult learners in Ukraine.

English is intended to remain the default interaction language. L1 support would be used selectively following repeated error, failed repair, comprehension breakdown, an explicit metalinguistic question or a learner request—not as routine translation.

## Proposed pedagogical architecture

The research instrument is intended to support:

- contrastive metalinguistic explanations;
- scaffold fading from fuller L1-mediated explanation to metalinguistic hints, L2-only elicitation and independent production;
- learner-initiated help and clarification;
- self-repair before direct correction;
- provisional modules addressing recurrent Ukrainian-/Russian-to-English difficulties;
- strict separation between instructional tutoring and standardized outcome assessment.

The initial linguistic targets are documented in [Fault_Line_Taxonomy.md](Fault_Line_Taxonomy.md). They are candidate modules subject to corpus evidence, expert linguistic review and pilot validation.

## Proposed research-data architecture

A future implementation is expected to record pseudonymous participant and session identifiers, target feature, feedback type, L1 use and function, learner- versus AI-initiated assistance, clarification requests, repair attempts and outcomes, learner-agency events, timestamps, and prompt/model/module/configuration versions.

Raw conversational data and derived analytical metadata should be logically separated. Automated classifications should be treated as candidate annotations and validated against human coding on a defined subset.

## Ethics and governance

[ETHICS_AND_PRIVACY.md](ETHICS_AND_PRIVACY.md) records design requirements for later institutional deployment. It does not certify that a GDPR-compliant environment, consent workflow, pseudonymization service, logging system or model-governance process has already been implemented.

## Planned development

1. Specify versioned instructional modules and trigger/fading rules.
2. Implement a minimal tutor and structured logging schema.
3. Add separate tutor and assessment modes.
4. Add prompt, model, module and configuration versioning.
5. Implement pseudonymization and separation of identity, consent and research data.
6. Complete provider, retention, data-location and subprocessor review.
7. Conduct expert linguistic review, pilot testing and human validation.
8. Seek the required University of Jyväskylä/TENK-aligned ethics and data-protection approvals before participant deployment.
