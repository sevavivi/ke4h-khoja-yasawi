---
layout: default
title: Challenges
---
[Home](index.html) | [Topic](topic.html) | [Methodology](methodology.html) | [RDF Triples](rdf.html) | [SPARQL](sparql.html) | [Gaps](gaps.html) | [LLM Prompts](prompts.html) | [Challenges](challenges.html) | [Conclusion](conclusion.html)

---
<img src="images/IMG_8082.jpeg" width="100%">
# Challenges

During the development of this project, we encountered several technical and conceptual challenges.

Although the project focused on a single cultural heritage entity, working with knowledge graphs and semantic technologies required careful analysis and validation.

---

# Challenge 1 – Learning SPARQL

## Problem

At the beginning of the project, we had limited experience with SPARQL.

Understanding query structure, variables, filters, and relationships between entities required practice.

## Solution

We experimented with different query structures and gradually learned how to retrieve and analyze information from Wikidata.

---

# Challenge 2 – No Matching Records

## Problem

Several SPARQL queries returned no results.

For example, searches related to Yasawiyya and pilgrimage functions did not produce matching records.

## Solution

Rather than treating this as a failure, we interpreted these results as evidence of missing information within the knowledge graph.

These missing results helped us identify knowledge gaps.

---

# Challenge 3 – Identifying Real Gaps

## Problem

Some information was available in Wikipedia and other textual sources but not represented in Wikidata as structured semantic data.

This made it difficult to distinguish between missing information and missing semantic representation.

## Solution

We focused on structured data representation rather than textual availability.

Our analysis concentrated on what could be retrieved through semantic queries.

---

# Challenge 4 – Evaluating LLM Outputs

## Problem

ChatGPT and Gemini sometimes generated different RDF triples and explanations.

Some outputs were broader than our research question.

## Solution

We manually reviewed all generated RDF triples and selected only those that directly addressed the identified knowledge gaps.

Human evaluation remained an essential part of the process.

---

# Challenge 5 – Knowledge Graph Modeling

## Problem

Designing meaningful RDF triples required balancing historical accuracy and semantic clarity.

Not every relationship could be represented in a simple way.

## Solution

We focused on triples that were:

- understandable;
- semantically meaningful;
- directly connected to the identified gaps;
- useful for future knowledge graph enrichment.

---

# Lessons Learned

This project demonstrated that semantic technologies are powerful tools for cultural heritage representation.

However, effective knowledge graph enrichment requires a combination of:

- SPARQL exploration;
- domain knowledge;
- critical thinking;
- human validation;
- Large Language Models.
