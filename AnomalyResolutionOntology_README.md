# Anomaly Resolution Ontology (ARO)

## Overview
The Anomaly Resolution Ontology (ARO) provides a formal framework for modeling anomalies, their bounded epistemic existence, and the semantic processes involved in their resolution. Built on BFO 2020 and aligned with the Common Core Ontologies (CCO 2.0), the ARO integrates and extends concepts originally drafted in the Anomaly Continuant Ontology (ACO) and the Anomaly Process Ontology (APO). It supports anomaly lifecycle modeling, enabling AI systems and analysts to represent and reason over states of uncertainty, cognitive transitions, and formal resolution processes.

## Key Features

- **Continuant–Occurrent Integration**: Combines anomaly state modeling with process-driven resolution workflows.
- **Temporally Bounded Anomalies**: Captures anomalies as generically dependent continuants that exist during bounded epistemic intervals.
- **Resolution Lifecycle Semantics**: Represents observations, unresolved information states, and epistemic closure via acts of resolution.
- **Epistemic Enlightenment**: Supports the terminal classification of anomalies through concretizing events.
- **SHACL Validation**: Includes node shape constraints for instance-level validation.

## Key Classes

| Class                          | Description |
|-------------------------------|-------------|
| `Anomaly`                     | A GDC that exists only while unresolved. |
| `Unresolved Anomaly Information` | ICE about the anomaly before resolution. |
| `Resolved Anomaly Information`   | ICE representing the understood outcome. |
| `Act of Observation`          | Initiates the epistemic existence of an anomaly. |
| `Act of Anomaly Resolution`   | Transitions an anomaly from unresolved to resolved. |
| `Epistemic Enlightenment Event` | A terminal act that marks an epistemic shift to resolution. |
| `Bounded Temporality Interval` | A temporal region capturing the start and end of an anomaly’s existence. |
| `Bounded Temporality`         | A quality or condition representing the temporally scoped existence of an anomaly. |
| `Epistemic State`             | A cognitive state associated with an anomaly's recognition, uncertainty, or resolution. |

## Object Properties Used
- `bfo:has_participant`
- `cco:has_input`
- `cco:has_output`
- `cco:is_about`
- `bfo:concretizes`
- `has bounded temporality interval`
- `marks start of bounded temporality interval`
- `marks end of bounded temporality interval`

## Use Cases
- Cyber threat triage and explanation
- ISR and sensor data anomaly reporting
- AI auditability and epistemic traceability
- Healthcare diagnostics and scientific anomaly resolution

## Ontology Files

| File | Description |
|------|-------------|
| `anomaly-resolution-ontology.05202025.ttl` | Turtle ontology file |
| `anomaly-ontology-node-shapes.ttl`        | SHACL node shapes for validation |

## Repository Structure
- `anomaly-resolution-ontology.05202025.ttl` – Main ontology
- `anomaly-ontology-node-shapes.ttl` – SHACL validation
- `examples/` *(planned)* – Usage walkthroughs
- `docs/` *(planned)* – Reference documentation and diagrams

## Design Principles
- **BFO 2020 Compliant** – Continuant/occurrent distinctions
- **CCO 2.0 Aligned** – Integrates Act, Agent, and Information modules
- **OWL 2 DL Valid** – Reasoner compatible
- **SHACL-Enabled** – Supports constraint checking

## Editors
- [Protégé](https://protege.stanford.edu/)
- [TopBraid Composer](https://www.topquadrant.com/products/topbraid-composer/)

## Reasoners
- [HermiT](http://www.hermit-reasoner.com/)
- [ELK](https://github.com/liveontologies/elk-reasoner)
- [Jena SHACL](https://jena.apache.org/documentation/shacl/)

## Usage Instructions

### Loading in Protégé
- File > Open > Select `.ttl`
- Activate reasoner: HermiT or ELK

### Validating with SHACL
- Use Jena SHACL CLI or TopQuadrant SHACL API

## Version and Status
**Version:** `anomaly-resolution-ontology.05202025.ttl`  
**Status:** Draft  
**License:** CC-BY 4.0  
**Maintainer:** [JJBittner](https://github.com/JJBittner)

## Authors
- J. Bittner ([JJBittner](https://github.com/JJBittner))  
- T. Coleman ([TimothyWColeman](https://github.com/TimothyWColeman))

## Citation
If using this ontology, please cite:

> J. Bittner, T. Coleman. *Anomaly Resolution Ontology: Semantic Modeling of Temporally Bounded Anomalies and Their Resolution Lifecycles.* https://github.com/JJBittner/Anomaly-Ontologies
