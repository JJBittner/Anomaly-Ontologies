# Anomaly Continuant Ontology (ACO)

## Overview
The Anomaly Continuant Ontology (ACO) provides a formal, BFO- and CCO-aligned framework for modeling anomalies as generically dependent continuants that exist only during a bounded epistemic interval. It supports intelligent anomaly processing systems by enabling explainable, validated, and semantically constrained reasoning over unresolved and resolved anomaly states.

## Key Features

- **Temporally Bounded Anomalies**: Models anomaly existence as time-constrained between initial observation and resolution.
- **Unresolved/Resolved Information Modeling**: Captures how anomalies are cognitively and computationally represented.
- **Observation-Driven Lifecycle**: Formal representation of observation acts as triggers of anomaly state.
- **SHACL Validation**: Includes node shape file for constraint checking and data validation.
- **Forward-Compatible**: Structured to integrate with the Anomaly Process Ontology (APO).

## Use Cases

- Cyber threat detection and triage
- Intelligence anomaly reporting
- Sensor data fusion and geospatial outlier analysis
- AI model auditability and epistemic transitions

## Key Concepts

| Class                         | Description |
|------------------------------|-------------|
| `Anomaly`                    | A generically dependent continuant that exists only while it is unresolved. |
| `Unresolved Anomaly Information` | ICE about the anomaly before understanding is achieved. |
| `Resolved Anomaly Information`   | ICE representing the understood resolution of the anomaly. |
| `Act of Anomaly Resolution`  | A process that transitions an anomaly from unresolved to resolved. |
| `Observation`                | The initiating event marking the anomaly’s epistemic beginning. |

## Ontology Files

| File | Description |
|------|-------------|
| `anomaly-ontology.05132025.ttl` | Main OWL/Turtle ontology file |
| `anomaly-ontology-node-shapes.ttl` | SHACL node shapes for validation |

## Repository Structure

- `anomaly-ontology.05132025.ttl` – Main ontology
- `anomaly-ontology-node-shapes.ttl` – SHACL node shapes
- `anomaly-process-ontology.05142025.ttl/` – APO extension for resolution workflows
- `examples/` *(planned)* – Usage examples
- `docs/` *(planned)* – Diagrams and documentation

## Design Principles

- **BFO 2020 Compliant** – formal continuant/occurrent distinctions
- **CCO 2.0 Aligned** – uses Information, Time, and Quality modules
- **OWL 2 DL Valid** – fully reasoner-compatible
- **SHACL-Enabled** – validates instance-level conformance

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
- Use Jena SHACL CLI or TopQuadrant SHACL API to validate instances

## Version and Status

**Version:** `anomaly-ontology.05132025.ttl`  
**Status:** Draft  
**License:** CC-BY 4.0  
**Maintainer:** [JJBittner](https://github.com/JJBittner)

## Authors
- J. Bittner ([JJBittner](https://github.com/JJBittner))  
- T. Coleman ([TimothyWColeman](https://github.com/TimothyWColeman))

## Citation
If using this ontology, please cite:

> J. Bittner, T. Coleman. *Anomaly Continuant Ontology: A Formal Semantic Representation of Temporally Bounded Anomalies. https://github.com/JJBittner/Anomaly-Ontologies
