# DIKWP HepatoScholar OS

**DIKWP HepatoScholar OS** is an offline-first, GitHub-ready research system for liver disease academic material aggregation, semantic organization, evidence ledgering, and research-gap mining.

It is designed for hepatology researchers, graduate students, evidence synthesis teams, translational medicine groups, and DIKWP ecosystem pilots. It helps transform messy academic materials into a DIKWP research ledger: **Data, Information, Knowledge, Wisdom, Purpose, Reliability**.

## What it is

- A literature corpus organizer for liver disease research.
- A DIKWP semantic ledger for papers, claims, disease entities, biomarkers, interventions, outcomes, and evidence gaps.
- A 3NO SemanticClosure engine for incomplete, imprecise, and inconsistent research materials.
- A research mining assistant for identifying evidence clusters, weak claims, hidden denominators, population gaps, and follow-up hypotheses.

## What it is not

This package is **not** a medical diagnostic tool, treatment recommendation system, prescription system, triage system, or substitute for clinicians, ethics review, regulatory review, or formal systematic-review methods.

## Quick start

```bash
pip install -e .
hepatoscholar analyze examples/sample_liver_research_corpus.json --out outputs/demo
hepatoscholar static-audit src --out outputs/demo/static_boundary_audit_report.json
```

## Main outputs

- `hepatoscholar_report.json`
- `dikwp_literature_ledger.json`
- `evidence_matrix.csv`
- `claim_cards.csv`
- `research_gap_report.md`
- `query_strategy_pack.md`
- `semantic_closure_report.json`
- `static_boundary_audit_report.json`

## Core idea

Liver disease literature is not only a pile of abstracts. Each record must be transformed into:

```text
C = (D, I, K, W, P, R)
D: source data and metadata
I: relations, terms, populations, exposures, endpoints
K: mechanisms, study designs, effect claims, disease knowledge
W: evidence quality, clinical risk boundary, translational caution
P: research purpose, review question, hypothesis, follow-up plan
R: reliability, missingness, inconsistency, residual, kill conditions
```

## Strategic value

This repository can become a DIKWP open-source sample for biomedical knowledge organization. The open-source core attracts researchers; official DIKWP templates, registry, review reports, and training can remain value-added layers.
