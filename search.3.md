# Survey Note: Exploring Associative Data Models and Link-Based Theories

This document compiles projects, articles, and systems related to associative data models and link-based theories, inspired by the concepts in the article ["The Links Theory 0.0.2"](https://habr.com/ru/articles/895896). The focus is on English-language resources that support relationships between relationships, excluding traditional graphs, relational models, and hypergraphs, as they do not meet the criteria of allowing edges between edges in the desired way.

## Background and Context

The referenced article introduces the "Links Theory," defining links as n-tuples of references to other links, with implementations like "Deep" and "LinksPlatform." It contrasts this with relational, associative, and graph models, emphasizing the ability to model complex relationships. This survey seeks similar projects, systems, or theoretical works that align with this associative paradigm, specifically those supporting higher-order relationships.

## Methodology

The search involved analyzing the article's concepts, focusing on terms like "associative data model," "links theory," and "relationships between relationships." Web searches and document reviews identified open-source database systems, theoretical papers, and related tools, all in English, that fit the criteria.

## Findings

### Database Systems Supporting Associative Models

The following open-source systems support complex relationship modeling, with varying degrees of alignment to the associative model:

- **TypeDB**: A knowledge graph database that inherently supports relationships between relationships using its TypeQL schema language. Ideal for knowledge representation.
  - Link: [https://typedb.com/](https://typedb.com/)
- **ConceptBase**: A deductive database with object-oriented modeling, supporting higher-order logic for complex relationships through meta-modeling.
  - Link: [http://conceptbase.sourceforge.net/](http://conceptbase.sourceforge.net/)
- **Apache Jena**: A semantic web framework supporting RDF and reification, allowing statements about statements (e.g., "Alice says Bob likes Charlie").
  - Link: [https://jena.apache.org/](https://jena.apache.org/)
- **Blazegraph**: A graph database supporting RDF and SPARQL, previously used by Wikidata, with reification for higher-order relationships.
  - Link: [https://blazegraph.com/](https://blazegraph.com/)
- **Neo4j**: A graph database where higher-order relationships can be modeled by reifying edges as nodes, adaptable for associative structures.
  - Link: [https://neo4j.com/](https://neo4j.com/)
- **OrientDB**: A multi-model database with graph capabilities, supporting complex relationships through edge reification.
  - Link: [https://orientdb.org/](https://orientdb.org/)
- **ArangoDB**: A multi-model database with graph support, capable of modeling higher-order relationships with appropriate schema design.
  - Link: [https://www.arangodb.com/](https://www.arangodb.com/)

### Articles and Theoretical Papers

These resources provide theoretical foundations for associative data models and link-based theories:

- **"The Associative Model of Data" by Simon Williams**: A book detailing the associative model implemented in the Sentences database, where links can connect to other links.
  - Link: [https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011](https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011)
- **Higher-Order Entity-Relationship Model (HERM) by Bernhard Thalheim**: Papers extending ER models to handle relationships between relationships, used for conceptual design.
  - Example Link: [https://link.springer.com/chapter/10.1007/3-540-51251-9_25](https://link.springer.com/chapter/10.1007/3-540-51251-9_25)
- **"Simplicial Databases" by David I. Spivak**: A category-theoretic approach using simplicial sets for database schemas, supporting complex relationship modeling.
  - Link: [https://arxiv.org/abs/0904.2012](https://arxiv.org/abs/0904.2012)

### Tools for Personal Knowledge Management

These tools apply associative principles for individual use, potentially inspiring database designs:

- **Logseq**: An open-source note-taking app with bidirectional links for associative organization of blocks.
  - Link: [https://logseq.com/](https://logseq.com/)
- **TiddlyWiki**: An open-source personal wiki using linked tiddlers for flexible, associative content management.
  - Link: [https://tiddlywiki.com/](https://tiddlywiki.com/)

## Summary Table

| Category                  | Name                           | Description                                                                 | Link                                                                 |
|---------------------------|--------------------------------|-----------------------------------------------------------------------------|----------------------------------------------------------------------|
| Database Systems          | TypeDB                        | Knowledge graph with direct support for relationships between relationships | [https://typedb.com/](https://typedb.com/)                           |
| Database Systems          | ConceptBase                   | Deductive database with higher-order logic for complex relationships        | [http://conceptbase.sourceforge.net/](http://conceptbase.sourceforge.net/) |
| Database Systems          | Apache Jena                   | Semantic web framework with RDF reification for higher-order statements     | [https://jena.apache.org/](https://jena.apache.org/)                 |
| Database Systems          | Blazegraph                    | RDF/SPARQL graph database with reification, used by Wikidata               | [https://blazegraph.com/](https://blazegraph.com/)                   |
| Database Systems          | Neo4j                         | Graph database modeling higher-order relationships via edge reification     | [https://neo4j.com/](https://neo4j.com/)                             |
| Database Systems          | OrientDB                      | Multi-model database with graph support for complex relationships           | [https://orientdb.org/](https://orientdb.org/)                       |
| Database Systems          | ArangoDB                      | Multi-model database with graph capabilities for relationship modeling      | [https://www.arangodb.com/](https://www.arangodb.com/)               |
| Articles and Papers       | The Associative Model of Data | Book on associative model with links between links                         | [https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011](https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011) |
| Articles and Papers       | HERM by Thalheim              | Extends ER model for relationships between relationships                    | [https://link.springer.com/chapter/10.1007/3-540-51251-9_25](https://link.springer.com/chapter/10.1007/3-540-51251-9_25) |
| Articles and Papers       | Simplicial Databases          | Category-theoretic database schemas for complex relationships               | [https://arxiv.org/abs/0904.2012](https://arxiv.org/abs/0904.2012)   |
| Tools                     | Logseq                        | Note-taking app with bidirectional links for associative thinking           | [https://logseq.com/](https://logseq.com/)                           |
| Tools                     | TiddlyWiki                    | Personal wiki with linked tiddlers for associative organization             | [https://tiddlywiki.com/](https://tiddlywiki.com/)                   |

## Conclusion

This survey identifies a range of open-source systems, theoretical papers, and tools aligned with associative data models and link-based theories. TypeDB and ConceptBase offer direct support for relationships between relationships, while Neo4j, Apache Jena, and others provide flexibility through reification. Theoretical works by Williams, Thalheim, and Spivak provide foundational insights, and tools like Logseq and TiddlyWiki demonstrate practical applications. These resources offer a starting point for exploring and building upon associative paradigms.

## Key Citations

- TypeDB: [https://typedb.com/](https://typedb.com/)
- ConceptBase: [http://conceptbase.sourceforge.net/](http://conceptbase.sourceforge.net/)
- Apache Jena: [https://jena.apache.org/](https://jena.apache.org/)
- Blazegraph: [https://blazegraph.com/](https://blazegraph.com/)
- Neo4j: [https://neo4j.com/](https://neo4j.com/)
- OrientDB: [https://orientdb.org/](https://orientdb.org/)
- ArangoDB: [https://www.arangodb.com/](https://www.arangodb.com/)
- The Associative Model of Data: [https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011](https://www.amazon.com/associative-model-data-Simon-Williams/dp/1903453011)
- HERM by Thalheim: [https://link.springer.com/chapter/10.1007/3-540-51251-9_25](https://link.springer.com/chapter/10.1007/3-540-51251-9_25)
- Simplicial Databases: [https://arxiv.org/abs/0904.2012](https://arxiv.org/abs/0904.2012)
- Logseq: [https://logseq.com/](https://logseq.com/)
- TiddlyWiki: [https://tiddlywiki.com/](https://tiddlywiki.com/)
