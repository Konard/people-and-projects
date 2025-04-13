# Associative Data Models and "Links Theory" in Practice

This document summarizes key people, projects, articles, and systems aligned with the associative data model and "links theory" described in the [Habr article](https://habr.com/ru/articles/895896). This approach treats every piece of data as an atomic link and lets relationships (edges) link to other relationships—unlike traditional graph databases (which only allow edges between nodes), hypergraphs, or relational models.

> **Note:** The focus here is on solutions that allow **edge-to-edge (or link-to-link) associations** and not traditional graph models, hypergraphs, or conventional relational models.

## Table of Contents

- [Overview](#overview)
- [Pioneers and Key Figures](#pioneers-and-key-figures)
- [Projects and Systems](#projects-and-systems)
- [Related Articles and Academic Work](#related-articles-and-academic-work)
- [References](#references)

## Overview

**Associative Data Models / Links Theory** are based on the following principles:

- **Atomic Links:** All information is stored as atomic “links” (or sentences) with a subject–verb–object structure.
- **Edge-to-Edge Linking:** A link representing a relationship can itself participate as a subject or object in another link, enabling recursive and layered associations.
- **Uniform Representation:** There is no strict separation between data objects and their relationships; everything is handled uniformly as a link.
- **Flexibility:** This reduces schema complexity and allows for dynamic, evolving relationships.

These principles mirror the way human cognition forms associations and represent a significant departure from relational or standard graph models.

## Pioneers and Key Figures

### Simon Williams – *The Associative Model of Data*
- **Contribution:** Introduced an early associative model where data is stored as *Items* and *Links*. For example, a fact like “Mary is sister to William” is stored as a link connecting the items “Mary” and “William” through the relationship “sister.”
- **Key Feature:** Enables any link to be used as the subject or object of another link, supporting true recursive associations.
- **Reference:**  
  [LazySoft / Sentences DBMS](http://www.lazyssoft.com)  
  *(Historical details on Simon Williams’ work can be found via LazySoft’s resources.)*

### Athanassios Hatzis – R3DM/S3DM Framework
- **Contribution:** Developed the **R3DM/S3DM** framework that treats associations as first-class entities.
- **Key Project:** **TRIADB** is an analytical engine built on these principles, allowing data to be modeled as a hypergraph of associations without a strict node–edge separation.
- **Reference:**  
  [Athanassios Hatzis on GitHub](https://github.com/hatzis)  
  *(Search within his repositories for TRIADB or related projects.)*

### Konstantin Dyachenko & Ivan Glazunov – Deep.Foundation
- **Contribution:** Co-founders of Deep.Foundation, a modern platform implementing a fully associative data model using a single `Links` table.
- **Key Feature:** Every piece of data—be it an object or a relationship—is stored uniformly as a link, naturally supporting recursive associations.
- **Reference:**  
  [Deep.Foundation](https://deep.foundation)

> **Additional Note:** Researchers involved with Topic Maps (e.g., Steve Pepper and Lars Marius Garshol) have similarly emphasized making associations first-class entities. While their work is slightly different, it reinforces the merit of the associative approach.

## Projects and Systems

### LazySoft *Sentences*
- **Description:** An early database system that implemented the associative model introduced by Simon Williams.
- **Key Idea:** All data is captured as *Items* and *Links*, with links being reusable as subjects or objects in other links.
- **Reference:**  
  [LazySoft / Sentences DBMS](http://www.lazyssoft.com)

### TRIADB (R3DM/S3DM)
- **Description:** An analytical engine where data is modeled as a hypergraph of associations (with no strict separation between entities and relationships).
- **Key Idea:** Supports associating associations—i.e., links can point to other links, thus enabling deep recursive querying.
- **Reference:**  
  [Athanassios Hatzis on GitHub](https://github.com/hatzis)  
  *(Search for TRIADB within his repositories.)*

### Deep.Links (Deep.Foundation)
- **Description:** An open-source platform and runtime environment implementing a fully associative model with a single `Links` table.
- **Key Idea:** Everything is a link. The platform provides tools like **Deep.Case** for visual exploration of the data network, making schema evolution straightforward.
- **Reference:**  
  [Deep.Foundation](https://deep.foundation)

### Topic Maps
- **Description:** A knowledge representation standard (ISO/IEC 13250) where topics (subjects) and associations (relationships) are treated as first-class objects.
- **Key Idea:** Although Topic Maps traditionally do not allow complete edge-to-edge linking, they were instrumental in conceptualizing associations as objects with properties.
- **Reference:**  
  [Wikipedia: Topic Maps](https://en.wikipedia.org/wiki/Topic_maps)

### AtomicDB (X10SYS)
- **Description:** An experimental project aimed at creating a high-performance associative database system.
- **Key Idea:** Data was represented as atomic units linked together, enabling flexible relationships at a granular level.  
- **Reference:**  
  *Detailed online references for AtomicDB are limited and primarily exist in historical or academic literature.*

### Qlik’s Associative Engine
- **Description:** The engine behind QlikView and Qlik Sense, built around an in-memory associative model that automatically indexes data by co-occurrence.
- **Key Idea:** Facilitates intuitive, cross-dimensional data exploration without conventional join operations, albeit without explicit edge-to-edge linking.
- **Reference:**  
  [Qlik Sense](https://www.qlik.com/us/products/qlik-sense)

## Related Articles and Academic Work

- **Semantic Web Reification & RDF-Star**
  - **Concept:** RDF reification turns RDF triples into objects so that additional statements (metadata) can be made about them.  
  - **Modern Extension:** RDF-star extends this idea, allowing embedded triples (i.e., making statements about statements) which conceptually overlaps with edge-to-edge linking.
  - **Reference:**  
    [RDF-star Specification](https://www.w3.org/TR/rdf-star/)

- **Associative Data Modeling Demystified (Series)**
  - **Content:** A series of blog posts exploring the benefits of associative models over traditional relational or graph databases.
  - **Reference:**  
    *(Search for "Associative Data Modeling Demystified" on LinkedIn or Medium for detailed posts.)*

- **Academic Comparisons of Data Models**
  - **Overview:** Various academic papers compare associative models, relational databases, and graph-based systems, highlighting the strengths of supporting recursive associations.
  - **Reference:**  
    Look up academic references such as Simon Williams' publications on “The Associative Model of Data” for foundational theory.

## Summary

The associative data model and "links theory" propose representing every fact as an atomic link capable of linking to other links. This paradigm facilitates a flexible, evolving data architecture without the rigidity of tables or the limitations of standard graph edges. Projects like **LazySoft Sentences**, **TRIADB**, and **Deep.Foundation** illustrate practical applications of these ideas, while related approaches such as Topic Maps and RDF reification further validate the concept of making relationships first-class entities.

## References

- **Habr Article:**  
  [https://habr.com/ru/articles/895896](https://habr.com/ru/articles/895896)
- **LazySoft / Sentences DBMS:**  
  [http://www.lazyssoft.com](http://www.lazyssoft.com)
- **Athanassios Hatzis & TRIADB:**  
  [GitHub - Athanassios Hatzis](https://github.com/hatzis) *(Search for TRIADB within this repository)*
- **Deep.Foundation:**  
  [https://deep.foundation](https://deep.foundation)
- **Topic Maps:**  
  [https://en.wikipedia.org/wiki/Topic_maps](https://en.wikipedia.org/wiki/Topic_maps)
- **Qlik Sense (Associative Engine):**  
  [https://www.qlik.com/us/products/qlik-sense](https://www.qlik.com/us/products/qlik-sense)
- **RDF-star Specification:**  
  [https://www.w3.org/TR/rdf-star/](https://www.w3.org/TR/rdf-star/)
- **Associative Data Modeling Demystified:**  
  *(Search for related posts on LinkedIn or Medium for detailed discussions.)*
- **AtomicDB (X10SYS):**  
  *Historical/academic references are the primary sources for this experimental project.*

---

*This document provides an overview and reference guide for those interested in the associative data model and "links theory" as an alternative to traditional data modeling approaches.*
