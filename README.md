# Service Ontology

This repository contains **Service Ontology**, an OWL/RDF ontology for goal-driven service-package creation, service execution, service orchestration, reusable-resource management, and evaluation through Key Values (KVs), Key Value Indicators (KVIs), and Key Performance Indicators (KPIs).

## Repository files

- [`service_ontology.ttl`](./service_ontology.ttl): the ontology in Turtle syntax.
- [`index.html`](./index.html): the interactive ontology directory and RDF visualization.
- [`README.md`](./README.md): repository documentation.
- [`.nojekyll`](./.nojekyll): ensures GitHub Pages serves the static files directly.

## Ontology version

- **Ontology name:** Service Ontology
- **Current version:** Version 1.0
- **Canonical ontology file:** `service_ontology.ttl`
- **Ontology IRI:** `https://lemontologist-syed.github.io/service_ontology/`
- **Namespace:** `https://lemontologist-syed.github.io/service_ontology/#`
- **Prefix:** `so:`

The version is stored as ontology metadata through `owl:versionInfo` and `rdfs:comment`. It is intentionally not included in class names, property names, the ontology IRI, the namespace, or the canonical filename.

Example:

```turtle
@prefix so: <https://lemontologist-syed.github.io/service_ontology/#> .

so:AIAgent
    a owl:Class ;
    rdfs:label "AI agent"@en .
```

## Main classes

The ontology has four top-level classes:

- `so:Goal`
- `so:Resource`
- `so:ServiceExecutingAgent`
- `so:ServicePackage`

`so:ServiceExecutingAgent` has no subclasses. It is described using:

- `so:serviceExecutingAgentRole`: `service execution` or `orchestration`
- `so:serviceExecutingAgentType`: `technical service execution agent` or `human agent`

## Ontology statistics

| Ontology element | Count |
|---|---:|
| Named classes | 28 |
| Object properties | 14 |
| Datatype properties | 39 |
| OWL restrictions | 24 |
| RDF triples | 546 |

The ontology uses the standard annotation properties `rdfs:label` and `rdfs:comment`.

## Interactive ontology directory

After GitHub Pages is enabled, the ontology directory will be available at:

**https://lemontologist-syed.github.io/service_ontology/**

The webpage contains definitions, classes, subclasses, object properties, datatype properties, annotation properties, OWL restrictions, and an interactive RDF visualization whose nodes and edges use ontology labels.

## Opening the ontology

The Turtle file can be opened in tools such as:

- Protégé
- RDFLib
- Apache Jena
- TopBraid Composer

## Versioning approach

Keep `service_ontology.ttl` as the stable canonical file. For later releases, update `owl:versionInfo` in the ontology and create a GitHub release such as `v1.1` or `v2.0`. A versioned copy may be attached to the release without changing the canonical ontology URL.

## Citation

A formal citation can be added after publication, for example:

```text
Author(s). (Year). Service Ontology (Version 1.0). GitHub repository. https://lemontologist-syed.github.io/service_ontology/
```
