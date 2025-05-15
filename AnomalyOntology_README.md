# Anomaly Ontologies

This repository hosts the **Anomaly Ontologies**, a collection of formal, BFO- and CCO-aligned ontologies and artifacts that support semantic modeling of anomalies and their resolution lifecycle in data-driven systems.

Currently, the repository includes:

- The **Anomaly Ontology**, which formally represents anomalies as temporally bounded semantic entities.
- The accompanying **SHACL node shape file** for validating anomaly-related instance data.

This repository will also soon include:

- The **Anomaly Process Ontology (APO)**, which will define the resolution workflows, subprocesses, and decision points associated with anomaly handling.
- Additional artifacts such as usage examples, diagrams, and SPARQL query templates.

Together, these resources support rigorous, explainable, and machine-readable anomaly reasoning frameworks for use in cybersecurity, ISR, AI validation, and other high-assurance domains.

## Anomaly Ontology

Version: `anomaly-ontology.05132025.ttl`  
SHACL Shapes: `anomaly-ontology-node-shapes.ttl`  
License: CC-BY 4.0  
Maintainer: [JJBittner](https://github.com/JJBittner)

---

## Overview

Anomalies in this ontology are represented as **generically dependent continuants** that exist only during the epistemically bounded period between detection and understanding. The ontology supports intelligent anomaly processing systems by enabling explainable, validated, and semantically constrained reasoning.

## Key Features

- **Temporally Bounded Anomalies**: Models anomaly existence as time-constrained between initial observation and resolution.
- **Unresolved/Resolved Information Modeling**: Captures how anomalies are cognitively and computationally represented.
- **Observation-Driven Lifecycle**: Formal representation of observation acts as triggers of anomaly state.
- **SHACL Validation**: Includes node shape file for constraint checking and data validation.
- **Forward-Compatible**: Structured to integrate with the forthcoming *Anomaly Process Ontology (APO)*.

## Use Cases

- Cyber threat detection and triage
- Intelligence anomaly reporting
- Sensor data fusion and geospatial outlier analysis
- AI model auditability and epistemic transitions

---

## Ontology Files

| File | Description |
|------|-------------|
| `anomaly-ontology.05132025.ttl` | Main OWL/Turtle ontology file |
| `anomaly-ontology-node-shapes.ttl` | SHACL node shapes for validation |
| *(Planned)* `apo/` | Folder for Anomaly Process Ontology extensions |

---

## Key Concepts

| Class                         | Description |
|------------------------------|-------------|
| `Anomaly`                    | A generically dependent continuant that exists only while it is unresolved. |
| `Unresolved Anomaly Information` | ICE about the anomaly before understanding is achieved. |
| `Resolved Anomaly Information`   | ICE representing the understood resolution of the anomaly. |
| `Act of Anomaly Resolution`  | A process that transitions an anomaly from unresolved to resolved. |
| `Observation`                | The initiating event marking the anomaly’s epistemic beginning. |

---

## Recommended Tools

### Editors

- [Protégé](https://protege.stanford.edu/)
- [TopBraid Composer](https://www.topquadrant.com/products/topbraid-composer/)

### Reasoners

- [HermiT](http://www.hermit-reasoner.com/) — for expressive OWL DL reasoning
- [ELK](https://github.com/liveontologies/elk-reasoner) — for scalable classification
- [Jena SHACL](https://jena.apache.org/documentation/shacl/) — for validating SHACL shapes

---

## Design Principles

- **BFO 2020 Compliant** — top-level formal distinctions (continuant/occurrent)
- **CCO 2.0 Aligned** — leverages CCO modules (Information, Time, Quality)
- **OWL 2 DL Valid** — ensures compatibility with automated reasoning
- **SHACL-Enabled** — validates instance data conformance
- **Extensible** — designed for integration with APO and domain overlays

---

# Anomaly Ontology (AO)

This repository hosts the **Anomaly Ontology**, a formal BFO- and CCO-aligned ontology for modeling the semantic lifecycle of anomalies in data-driven systems. It provides a rigorous conceptual framework for representing anomalies from the moment of their detection to the point of their resolution.

**Version:** `anomaly-ontology.05132025.ttl`  
**Status:** Draft  
**License:** CC-BY 4.0  
**Maintainer:** [JJBittner](https://github.com/JJBittner)

---

## Overview

Anomalies in this ontology are represented as **generically dependent continuants** that exist only during the epistemically bounded period between detection and understanding. The ontology supports intelligent anomaly processing systems by enabling explainable, validated, and semantically constrained reasoning.

---

## Repository Structure

- `anomaly-ontology.05132025.ttl` – Main ontology
- `anomaly-ontology-node-shapes.ttl` – SHACL node shapes
- `anomaly-process-ontology/` *(planned)* – Anomaly Process Ontology for reasoning over resolution workflows
- `examples/` *(planned)* – Usage examples for anomaly modeling and validation
- `docs/` *(planned)* – Diagrams and documentation

---

## Use Cases

- Cyber threat detection and triage
- Intelligence anomaly reporting
- Sensor data fusion and geospatial outlier analysis
- AI model auditability and epistemic transitions

---

## Key Concepts

| Class                         | Description |
|------------------------------|-------------|
| `Anomaly`                    | A generically dependent continuant that exists only while it is unresolved. |
| `Unresolved Anomaly Information` | ICE about the anomaly before understanding is achieved. |
| `Resolved Anomaly Information`   | ICE representing the understood resolution of the anomaly. |
| `Act of Anomaly Resolution`  | A process that transitions an anomaly from unresolved to resolved. |
| `Observation`                | The initiating event marking the anomaly’s epistemic beginning. |

---

## Design Principles

- **BFO 2020 Compliant** – top-level formal distinctions (continuant/occurrent)
- **CCO 2.0 Aligned** – leverages CCO modules (Information, Time, Quality)
- **OWL 2 DL Valid** – ensures compatibility with automated reasoning
- **SHACL-Enabled** – validates instance data conformance
- **Extensible** – designed for integration with APO and domain overlays

---

## Editors

- [Protégé](https://protege.stanford.edu/)
- [TopBraid Composer](https://www.topquadrant.com/products/topbraid-composer/)

---

## Reasoners

- [HermiT](http://www.hermit-reasoner.com/) – for expressive OWL DL reasoning  
- [ELK](https://github.com/liveontologies/elk-reasoner) – for scalable classification  
- [Jena SHACL](https://jena.apache.org/documentation/shacl/) – for validating SHACL shapes

---

## Usage Instructions

### Loading in Protégé

- File > Open > Select `.ttl`
- Check for active reasoner: HermiT or ELK

### Validating with SHACL

Use Jena SHACL CLI or TopQuadrant SHACL API to test instances against shapes.

## Version and Status

**Version:** `anomaly-ontology.05132025.ttl`  
**Status:** Draft  
**License:** CC-BY 4.0  
**Maintainer:** [JJBittner](https://github.com/JJBittner)

---

## Repository Structure

- `anomaly-ontology.05132025.ttl` – Main ontology
- `anomaly-ontology-node-shapes.ttl` – SHACL node shapes
- `anomaly-process-ontology.05142025.ttl/` – Anomaly Process Ontology for reasoning over resolution workflows
- `examples/` *(planned)* – Usage examples for anomaly modeling and validation
- `docs/` *(planned)* – Diagrams and documentation

---

## Usage Instructions

### Loading in Protégé

- Open Protégé
- File > Open > Select `.ttl`
- Activate a reasoner such as HermiT or ELK

### Validating with SHACL

- Use the Jena SHACL CLI or TopQuadrant SHACL API
- Load your instance data and run it against `anomaly-ontology-node-shapes.ttl`

---

## Future Work / Roadmap

- Integration with Anomaly Process Ontology (APO)
- SPARQL query templates and validation scripts
- Formal alignment with OBO Foundry principles (optional)
- Examples for ISR, Cyber, and Environmental Safety domains

---

## Metadata (for ontology header)

```ttl
@prefix dcterms: <http://purl.org/dc/terms/> .
@prefix owl: <http://www.w3.org/2002/07/owl#> .

<https://github.com/JJBittner/anomaly-ontology>
    a owl:Ontology ;
    dcterms:title "Anomaly Ontology" ;
    dcterms:contributor "J. Bittner" ;
    dcterms:contributor "T. Coleman" ;
    dcterms:license <https://creativecommons.org/licenses/by/4.0/> ;
    dcterms:description "A BFO- and CCO-aligned ontology for representing anomalies and their resolution lifecycle." .

