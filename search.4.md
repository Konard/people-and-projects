# Survey Note: Associative Data Models Supporting Edges Between Edges

This document summarizes research into open-source systems and projects that align with the associative data model, specifically those supporting edges between edges (links between links) at a single level. The focus is on English-language resources, prioritizing publicly available projects with less restrictive licensing. Excluded are graphs, hypergraphs (not allowing edges between edges), relational models with many tables, and n-order category theories requiring multiple levels.

## Background
The investigation was inspired by an article discussing links theory, which models everything as links without distinguishing vertices and edges. The goal was to identify similar but unmentioned systems where links can connect to other links at a single level, suitable for academic and industry applications.

## Methodology
Research involved web searches, academic papers, and database documentation, targeting terms like "associative data model," "links between links," and "open-source database edges between edges." Only open-source projects with permissive licensing were considered, ensuring alignment with the criteria.

## Findings

### 1. SurrealDB
- **Description**: A multi-model database supporting relational, document, and graph models. Its graph relations treat edges as records, enabling links between edges.
- **Key Features**:
  - Edges are records, allowing relationships between relationships.
  - Permissive open-source license.
  - Supports real-time collaboration and ACID transactions.
  - Actively maintained as of April 2025.
- **Use Cases**: Serverless apps, real-time systems, collaborative platforms.
- **Links**:
  - Website: [SurrealDB](https://surrealdb.com)
  - GitHub: [SurrealDB GitHub](https://github.com/surrealdb/surrealdb)

### 2. HyperGraphDB
- **Description**: A graph database using hypergraphs, designed for AI and semantic web projects, where edges can point to other edges.
- **Key Features**:
  - Atoms (nodes or edges) support higher-order relationships.
  - Open-source under Apache 2.0.
  - Java-based, using BerkeleyDB.
  - Active development with recent commits.
- **Use Cases**: AI, semantic web, knowledge representation.
- **Links**:
  - Website: [HyperGraphDB](http://hypergraphdb.org)
  - GitHub: [HyperGraphDB GitHub](https://github.com/hypergraphdb/hypergraphdb)

### 3. TypeDB
- **Description**: A knowledge graph database with a hypergraph model, allowing relationships to be entities for complex interconnections.
- **Key Features**:
  - Supports higher-order relationships via entity modeling.
  - Open-source under Apache 2.0.
  - Active community and industry use.
- **Use Cases**: Bioinformatics, financial systems, research.
- **Links**:
  - Website: [TypeDB](https://vaticle.com/typedb)
  - GitHub: [TypeDB GitHub](https://github.com/vaticle/typedb)

## Exclusions
- **Graphs/Hypergraphs**: Excluded (e.g., Neo4j, ArangoDB) as they do not natively support edges between edges without reification.
- **Relational Models**: Excluded due to reliance on many tables, not used associatively.
- **AtomicDB**: Not included due to unclear status and lack of recent updates.
- **Relavance**: Excluded as a commercial, non-open-source system.

## Academic and Community Context
- Academic papers, like "A COMPARISON OF THE RELATIONAL DATABASE MODEL AND THE ASSOCIATIVE DATABASE MODEL" ([ResearchGate](https://www.researchgate.net/publication/255670856_A_COMPARISON_OF_THE_RELATIONAL_DATABASE_MODEL_AND_THE_ASSOCIATIVE_DATABASE_MODEL)), highlight the flexibility of associative models.
- Community projects, such as HyperGraphDB’s OpenCog integration, show industry relevance, while SurrealDB and TypeDB have active open-source communities.

## Conclusion
SurrealDB, HyperGraphDB, and TypeDB are the most relevant open-source systems supporting edges between edges at a single level. They offer permissive licensing, active development, and applicability in academic and industry settings. Their repositories and documentation provide further exploration opportunities.

## References
- [SurrealDB](https://surrealdb.com)
- [HyperGraphDB](http://hypergraphdb.org)
- [TypeDB](https://vaticle.com/typedb)
- [SurrealDB GitHub](https://github.com/surrealdb/surrealdb)
- [HyperGraphDB GitHub](https://github.com/hypergraphdb/hypergraphdb)
- [TypeDB GitHub](https://github.com/vaticle/typedb)
- [A COMPARISON OF THE RELATIONAL DATABASE MODEL AND THE ASSOCIATIVE DATABASE MODEL](https://www.researchgate.net/publication/255670856_A_COMPARISON_OF_THE_RELATIONAL_DATABASE_MODEL_AND_THE_ASSOCIATIVE_DATABASE_MODEL)
- [Associative Data Modeling Demystified](https://www.datasciencecentral.com/associative-data-modeling-demystified-part1/)
