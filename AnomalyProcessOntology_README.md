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
- T. Coleman ([TimTColeman](https://github.com/TimTColeman))

## License
Content License: [cco:ont00001743](https://www.commoncoreontologies.org/ontology/cco/cco.owl#ont00001743)  
Code License: [cco:ont00001759](https://www.commoncoreontologies.org/ontology/cco/cco.owl#ont00001759)  
Copyright: [cco:ont00001744](https://www.commoncoreontologies.org/ontology/cco/cco.owl#ont00001744)

## Citation
If using this ontology, please cite:

> J. Bittner, T. Coleman. *Anomaly Process Ontology: A Formal Representation of Anomaly Resolution in Dynamic Systems*. University at Buffalo, 2025. https://github.com/JJBittner/Anomaly-Ontologies

## Status
**Draft** – Open for community feedback and contributions.

---

For questions, suggestions, or contributions, please open an issue or contact the maintainers.

