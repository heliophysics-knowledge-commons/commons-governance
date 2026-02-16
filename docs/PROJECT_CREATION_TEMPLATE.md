# Heliophysics Knowledge Commons
GitHub Project Creation Template

---
## Purpose

This document defines the standard structure for creating new project repositories within the Heliophysics Knowledge Commons.

The goal is to ensure that all projects:
- Are legible to the community
- Clearly articulate scope and contribution
- Connect to existing efforts
- Track maturity and governance stage
- Support long-term interoperability

This template should be used whenever creating a new repository within the Knowledge Commons organization.

---
## 1. Repository Naming Convention

Use the following naming pattern:

`project-<short-descriptive-name>`


Examples:

`project-phenomena-ontology`

`project-spase-schemaorg-alignment`

`project-instrument-taxonomy`



If the repository is infrastructure-level:

`infra-<name>`


Examples:

`infra-network-map`

`infra-validation-tools`


Names should be concise, descriptive, and stable.

---
## 2. Required Files

Every new project repository must include:
```
README.md
commons.yaml
CONTRIBUTING.md
ROADMAP.md
LICENSE
```



Optional but encouraged:
```
docs/
data/
notebooks/
mappings/
examples/
```

---
## 3. README Template

Copy the following into README.md when creating a new project:
```
# Project Title

## Overview

This project is part of the Heliophysics Knowledge Commons.

Briefly describe:
- What this project does
- What problem it addresses
- What semantic or knowledge infrastructure it contributes to

---

## Relationship to the Heliophysics Knowledge Commons

This project contributes to stewarding:

- [ ] Meaning (glossaries, ontologies, vocabularies)
- [ ] Structure (data models, schemas, representations)
- [ ] Interoperability (crosswalks, mappings, alignment)

Primary intended pathway:

- [ ] Exploratory Project (Stage 0)
- [ ] Active Community Project (Stage 1)
- [ ] Foundation Candidate (Stage 2)
- [ ] Commons Foundation (Stage 3)

---

## Scope

Clearly define:

**In Scope**
- 

**Out of Scope**
- 

---

## Current Stage

- [ ] Stage 0 — Exploratory
- [ ] Stage 1 — Active Community Project
- [ ] Stage 2 — Foundation Candidate
- [ ] Stage 3 — Commons Foundation

(See commons-governance repository for definitions.)

---

## Leads & Contributors

Project Leads:
- Name (Affiliation)
- Name (Affiliation)

Contributors:
- 

---

## Dependencies & Connections

List related efforts inside and outside the commons:

- Internal projects:
- External standards:
- Related ontologies or schemas:
- Data systems:

---

## Deliverables

This project intends to produce:

- [ ] Ontology (OWL / SKOS / RDF)
- [ ] Data model or schema
- [ ] Crosswalk / mapping
- [ ] Knowledge graph
- [ ] API
- [ ] Documentation
- [ ] Integration with external systems
- [ ] Publication

---

## Roadmap

High-level milestones:

- Q1:
- Q2:
- Q3:
- Q4:

---

## Governance

This repository follows:

- Organization-level governance policies
- Interoperability guidance (if applicable)
- Foundation review processes (if applicable)

Major scope changes should be proposed via GitHub Issues.

---

## Citation

If applicable, include DOI, Zenodo link, or citation instructions.
```


---
## 4. commons.yaml (Machine-Readable Metadata)

Each project must include a `commons.yaml` file at the root of the repository.

This file enables:
```
Automated ecosystem mapping
Maturity tracking
Portfolio visualization
Governance transparency
```


```
Template:

name: Project Name
short_name: short-slug
type: project        # project | infra | foundation-candidate
stage: 0             # 0 | 1 | 2 | 3

leads:
  - name: Full Name
    affiliation: Institution
    email: optional

domains:
  - heliophysics

contributes_to:
  - meaning
  - structure
  - interoperability

connects_to:
  - SPASE
  - ADS
  - UAT
  - ODIS

external_standards:
  - schema.org
  - DataCite
  - DCAT

foundation_target: commons-foundations

status: active       # active | paused | completed

last_updated: YYYY-MM-DD
```

This file should be updated when:
```
Stage changes
Leads change
Status changes
Major scope revisions occur
```

---
## 5. CONTRIBUTING Template

Create a `CONTRIBUTING.md` file with the following structure:

```
# Contributing

Thank you for contributing to this project.

## Ways to Contribute

- Open Issues for discussion
- Submit Pull Requests
- Suggest mappings or model refinements
- Improve documentation
- Propose structural changes

## Review Expectations

- All changes should include rationale.
- Interoperability decisions must document assumptions.
- Significant model changes should reference related discussions.

For broader structural questions, consult organization governance policies.
```

---
## 6. ROADMAP Template

Create a `ROADMAP.md` file:

```
# Roadmap

## Phase 1 — Definition
- Define scope
- Gather stakeholders
- Identify dependencies

## Phase 2 — Implementation
- Develop ontology/model/mapping
- Release v0.x

## Phase 3 — Adoption
- Integrate with external systems
- Gather feedback

## Phase 4 — Stabilization
- Versioned release
- Consider promotion to Foundation (if appropriate)
```

---
## 7. Project Lifecycle Stages

Projects progress through the following stages:

- Stage 0 — Exploratory
  - Idea formation
  - Small working group
  - Early artifacts
- Stage 1 — Active Community Project
  - Public repository
  - Clear scope
  - Community contributors
  - Regular updates

- Stage 2 — Foundation Candidate
  - Broad adoption potential
  - Clear interoperability role
  - Documentation and governance maturity

- Stage 3 — Commons Foundation
  - Recognized structural role in the Knowledge Commons
  - Community-governed
  - Long-term stewardship commitment
  - Stage promotion requires community review.


---
## 8. Cultural Norms

This template is designed to:
- Encourage clarity before implementation
- Prevent duplication and fragmentation
- Make interoperability explicit
- Support ecosystem-level thinking
- Ensure transparency of intent and governance


Projects that do not maintain documentation, scope clarity, or governance alignment may not be promoted to higher stages.

---
## 9. Before Creating a New Project

Before opening a new repository, consider:
- Does this effort overlap with an existing project?
- Can this be implemented as a module within another repository?
- Does this require coordination with existing foundations?
- Is the scope clearly bounded?


If uncertain, open a discussion issue in the governance repository before creating the project.

---
## 10. Maintenance Expectations

Project leads are responsible for:
- Keeping commons.yaml up to date
- Updating roadmap status
- Responding to issues
- Communicating major changes


Inactive repositories may be archived after community review.

---
## Closing Note

The Heliophysics Knowledge Commons is an international, community-governed effort to steward the meaning, structure, and interoperability of Heliophysics knowledge.

Projects created using this template become part of a broader ecosystem. Clarity, transparency, and interoperability are shared responsibilities.
