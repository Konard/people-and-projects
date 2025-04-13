# Associative Data Models: Summary of Findings

This document summarizes the context from the article ["The Links Theory 0.0.2"](https://habr.com/ru/articles/895896) and identifies related projects and articles on associative data models, excluding standard graphs (no edges between edges) and relational models (typically too many tables). The findings focus on projects and resources not mentioned in the original article, suitable for researchers and developers exploring associative data structures for AI and beyond.

## Context from "The Links Theory 0.0.2"

The article, published on Habr, introduces "The Links Theory 0.0.2," a framework for a unified informational theory inspired by human associative memory, aimed at future AI data storage. Key points include:

- **Purpose**: Develop a simpler data model using set theory (\`L \to L^2\`), with doublet-links (2-tuples) and triplet-links (3-tuples) for efficient data representation and deduplication.
- **Comparison**: Outperforms relational algebra and graph theory, with implementations like Deep (PostgreSQL-based) and plans for LinksPlatform (Rust, offering 200x write, 1000x read improvements).
- **Features**: Includes visual tools (link blueprint designer, H-tree fractal demo) and future plans for self-projection and comparisons with set theory, type theory, etc.
- **Resources**: References Wikipedia ([Associative Model Archive](https://web.archive.org/web/20210814063207/https://en.wikipedia.org/wiki/Associative_model_of_data)), GitHub repositories, and community channels (Telegram, Deep.Foundation blog).

The associative model stores entities as items and relationships as links, supporting higher-order connections (links to links), unlike graphs or multi-table relational databases.

## Identified Projects

Below are projects aligned with associative data models, not mentioned in the article:

| Project       | Description                                                                 | Relevance                                                  | URL                                                                 |
|---------------|-----------------------------------------------------------------------------|------------------------------------------------------------|---------------------------------------------------------------------|
| **CQL**       | Open-source tool using category theory for data integration and querying.   | Mathematical approach to relationships, akin to set theory. | [CQL Website](https://categoricaldata.net/)                         |
| **HyperGraphDB** | Open-source hypergraph database for AI and semantic web applications.     | Supports edges connecting edges, fitting associative needs. | [HyperGraphDB Website](https://hypergraphdb.org/)                   |
| **TypeDB**    | Open-source hypergraph database for knowledge representation.               | Models complex relationships beyond standard graphs.        | [TypeDB Website](https://vaticle.com/typedb)                       |
| **Graphbrain**| Semantic hypergraph database for natural language processing.               | Handles recursive, n-ary connections like associative links.| [Graphbrain Docs](https://graphbrain.net/overview/hypergraph.html) |
| **AtomicDB**  | Associative database storing unique instances with managed associations.    | Directly implements associative model (possibly inactive).  | [AtomicDBOnline](https://www.atomicdbonline.com/)                   |
| **Qlikview**  | BI tool with associative data model for dynamic data exploration.           | Links data for analysis, though focused on BI, not storage. | [Qlik Community](https://community.qlik.com/t5/QlikView-App-Dev/QlikView-Associative-Model-Explained-A-perspective-on-R3DM/td-p/1256548) |

## Related Articles

These articles provide theoretical and practical insights into associative models, not referenced in the original:

- **"Associative Data Modeling Demystified" Series**: Explores associative technology in databases like AtomicDB, comparing with graph and document models.  
  - [Part 1](https://www.datasciencecentral.com/associative-data-modeling-demystified-part1/)
- **"The associative data model"**: Compares associative and relational models, highlighting business-database alignment.  
  - [ResearchGate](https://www.researchgate.net/publication/234779362_The_associative_data_model)
- **"Categorical Data Integration for Computational Science"**: Discusses CQL's functorial data migration for data integrity.  
  - [arXiv](https://arxiv.org/abs/1903.10579)

## Notes

- **Criteria**: Projects and articles were selected for supporting higher-order relationships, excluding standard graphs (no edge-to-edge connections) and relational models (avoiding excessive tables).
- **Activity**: Most projects (CQL, HyperGraphDB, TypeDB, Graphbrain) are active; AtomicDB’s status is unclear but conceptually relevant.
- **Date**: Findings are current as of April 13, 2025, ensuring relevance.

This summary provides a starting point for exploring associative data models, with links for further investigation.

## Citations

- ["The Links Theory 0.0.2"](https://habr.com/ru/articles/895896)
- [Wikipedia Archive: Associative Model of Data](https://web.archive.org/web/20210814063207/https://en.wikipedia.org/wiki/Associative_model_of_data)
- [CQL Website](https://categoricaldata.net/)
- [HyperGraphDB Website](https://hypergraphdb.org/)
- [TypeDB Website](https://vaticle.com/typedb)
- [Graphbrain Documentation](https://graphbrain.net/overview/hypergraph.html)
- [AtomicDBOnline](https://www.atomicdbonline.com/)
- [Qlik Community: QlikView Associative Model](https://community.qlik.com/t5/QlikView-App-Dev/QlikView-Associative-Model-Explained-A-perspective-on-R3DM/td-p/1256548)
- [Associative Data Modeling Demystified Part 1](https://www.datasciencecentral.com/associative-data-modeling-demystified-part1/)
- [ResearchGate: The Associative Data Model](https://www.researchgate.net/publication/234779362_The_associative_data_model)
- [arXiv: Categorical Data Integration](https://arxiv.org/abs/1903.10579)
