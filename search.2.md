# Associative Data Models and "Links Theory" in Practice

This document summarizes people, projects, articles, and systems that align with the associative data model and links theory described in the [Habr article](https://habr.com/ru/articles/895896). This model emphasizes *associative linking*, where relationships (edges) are first-class citizens capable of linking to other relationships—unlike traditional graph databases (which disallow edge-to-edge links), hypergraphs, or relational models.

## Overview of Associative Data Modeling & Links Theory

The **associative data model** (or "links theory") is based on the following principles:

- **Atomic Links:** All information is represented as atomic “links” (or sentences) with a subject–verb–object structure.
- **Edge-to-Edge Linking:** Any link, representing an association, can itself be linked to other links—allowing recursive or layered relationships.
- **Uniform Representation:** Everything—data objects, relationships, relationship types— is stored uniformly as links.
- **Flexibility & Evolution:** This model reduces schema complexity; any change is simply new links rather than refactoring tables.

These ideas mirror how human cognition associates concepts and have been proposed as an advance beyond both relational models and traditional graph databases.

## Pioneers and Key Figures

### Simon Williams – The Associative Model of Data
- **Overview:** Introduced an early associative model where data is stored as *Items* and *Links*. A fact, e.g., “Mary is sister to William,” becomes a link associating the items “Mary” and “William” through the relationship “sister.”
- **Key Features:** Links can themselves be the subject or object of further links, allowing rich recursive associations.
- **References:** [Williams’ writings and Sentences DBMS](#).

### Athanassios Hatzis – R3DM/S3DM Framework
- **Overview:** Developed the R3DM/S3DM framework, which treats associations as first-class entities. His work shows how an associative model can support link-to-link relationships.
- **Key Project:** TRIADB, an analytical engine built on this concept.
- **Key Features:** Data is modeled as a hypergraph where nodes and edges have no strict separation.
- **References:** [Hatzis’ publications on associative data modeling](#).

### Konstantin Dyachenko & Ivan Glazunov – Deep.Foundation
- **Overview:** Deep.Foundation is a modern project that implements an associative data model using a single `Links` table.
- **Key Features:** 
  - Every piece of data is stored as a link, allowing associations to refer to any other association.
  - Includes tools like **Deep.Case** for visual exploration.
  - Emphasizes “data-driven development” with flexible, schema-agnostic design.
- **References:** [Deep.Foundation documentation and Medium articles](#).

> **Note:** Other pioneers linked to Topic Maps (e.g., Steve Pepper and Lars Marius Garshol) have also contributed to first-class relationship modeling, further reinforcing the validity of associative approaches.

## Projects and Systems Implementing Associative Models

### 1. LazySoft *Sentences*
- **Description:** An early DBMS system that implemented the associative model as described by Simon Williams.
- **Key Idea:** Stored all data as *Items* and *Links*, where links could be reused as subjects/objects in further associations.

### 2. TRIADB (R3DM/S3DM)
- **Description:** An analytical engine that models data as a hypergraph of associations.
- **Key Idea:** Allows deep associative querying without the rigidities of traditional SQL joins.

### 3. Deep.Links (Deep.Foundation)
- **Description:** An open-source environment implementing a fully associative runtime.
- **Key Idea:** A single `Links` table holds every data entity and relationship. This provides native support for linking relationships to relationships, hence enabling recursive associations.

### 4. Topic Maps
- **Description:** A knowledge modeling standard (ISO/IEC 13250) where topics and associations are both first-class objects.
- **Key Idea:** Associations are explicitly treated as objects that can have properties and roles. While not allowing full edge-to-edge linkage as in associative models, the philosophy is closely aligned.

### 5. AtomicDB (X10SYS)
- **Description:** A lesser-known project aimed at building a high-performance associative database system.
- **Key Idea:** Data was conceptualized as atomic units linked together, enabling flexible linking across otherwise isolated records.

### 6. Qlik’s Associative Engine
- **Description:** Powers QlikView/Qlik Sense, creating an in-memory index of data values that are automatically associated based on co-occurrence.
- **Key Idea:** This associative design facilitates instant, cross-dimensional data filtering, though it doesn’t support direct edge-to-edge linking.
  
> **Additional Note:**  
> Research in the semantic web space (e.g., **RDF reification** and **RDF-star**) also acknowledges the need for making statements about statements (a kind of associative linking). Although RDF-star extends graph-based models, it supports nested associations, confirming the broader appeal of the idea.

## Related Articles and Academic Work

- **Semantic Web Reification & RDF-Star:**  
  Discusses how to treat triples (or statements) as subjects/objects in further triples, conceptually similar to links theory.
  
- **"Associative Data Modeling Demystified":**  
  A series of blog posts exploring how associative models compare and can improve upon traditional relational and graph-based approaches.
  
- **Academic Comparisons of Data Models:**  
  Papers that compare graph databases, topic maps, and associative data models, highlighting the unique strengths of edge-to-edge linking.

## Summary

In essence, the associative data model as described by the Habr article has inspired a range of projects and systems that see data as a network of relationships that can be as dynamic and multi-dimensional as the associations in human thought. Key implementations such as **Sentences**, **TRIADB**, and **Deep.Foundation** demonstrate the practical benefits: reduced schema complexity, inherent flexibility, and truly recursive relationships. This approach offers a promising alternative that pushes beyond the limitations of both traditional relational databases and conventional graph databases.

---

*This document aims to serve as an introductory summary of the associative data model and "links theory." For further reading, please refer to the listed primary sources and project documentations.*
