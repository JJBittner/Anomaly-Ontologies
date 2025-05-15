# Anomaly Process Ontology (APO)

## Overview
The Anomaly Process Ontology (APO) provides a structured representation of the semantic processes involved in identifying, analyzing, and resolving anomalies. It is designed as a formal extension of the Anomaly Continuant Ontology (ACO), capturing dynamic activities that occur over time, such as the recognition of epistemic uncertainty, the processing of unresolved information, and the resolution of anomalies through acts of information processing. 

This ontology aligns with the **Basic Formal Ontology (BFO 2020)** and the **Common Core Ontologies (CCO 2.0)** and is intended for use in domains where explainability, formal traceability, and epistemic transitions are critical, including ISR, cybersecurity, healthcare diagnostics, and scientific inference.

## Scope and Purpose
The APO models:
- The **lifecycle of anomaly resolution**, including discovery, evaluation, and resolution.
- The transition from **unresolved anomaly information** to **resolved information**.
- The formal representation of **epistemic shifts**, including events such as the *Epistemic Enlightenment Event*.
- The **temporal boundaries** of anomaly existence, i.e., bounded temporality.
- The role of AI systems, sensor observations, and agents in anomaly interpretation and resolution.

## Key Classes
- **Bounded Temporality**: A representation of temporally-scoped existence constraints tied to epistemic conditions.
- **Bounded Temporality Interval**: A subclass of `bfo:temporal region` denoting the start and end bounds of an anomaly's recognized duration.
- **Act of Anomaly Resolution**: A subclass of `cco:ActOfResolution` representing the process by which an anomaly is resolved.
- **Unresolved Anomaly Information**: A subclass of `Unresolved Information`, representing information content entities about anomalies not yet resolved.
- **Resolved Anomaly Information**: A subclass of `Resolved Information`, representing the resolved state of a formerly anomalous entity.
- **Epistemic Enlightenment Event**: A terminal act that concretizes a change in understanding, marking the resolution of the anomaly.

## Object Properties Used
- `bfo:has_participant`
- `cco:has_input`
- `cco:has_output`
- `cco:is_about`
- `apo:APO_0000053` – marks start of bounded temporality interval
- `apo:APO_0000054` – marks end of bounded temporality interval

## Dependencies
- [Anomaly Continuant Ontology (ACO)](../Anomaly-Ontology)
- [Basic Formal Ontology (BFO 2020)](https://github.com/BFO-ontology/BFO-2020)
- [Common Core Ontologies (CCO 2.0)](https://github.com/CommonCoreOntology/CommonCoreOntologies)

## Authors
- J. Bittner ([JJBittner](https://github.com/JJBittner))  
- T. Coleman ([TimothyWColeman](https://github.com/TimothyWColeman))

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



