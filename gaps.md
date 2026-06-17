---
layout: default
title: Identifying Gaps
---
[Home](index.html) | [Topic](topic.html) | [Methodology](methodology.html) | [RDF Triples](rdf.html) | [SPARQL](sparql.html) | [Gaps](gaps.html) | [LLM Prompts](prompts.html) | [Challenges](challenges.html) | [Conclusion](conclusion.html)

---
# Identifying Gaps

After exploring the Wikidata representation of the Mausoleum of Khoja Ahmed Yasawi through SPARQL queries, we identified several important gaps in the knowledge graph.

Although Wikidata contains historical, geographical, and architectural information, important cultural and religious aspects remain underrepresented.

These missing elements limit the ability of the knowledge graph to fully represent the significance of the monument.

---

# Gap 1 – Missing Connection with the Yasawiyya Sufi Order

## Observation

The mausoleum was built around the tomb of Khoja Ahmed Yasawi, founder of the Yasawiyya Sufi tradition.

However, our SPARQL exploration did not reveal an explicit semantic connection between the monument and the Yasawiyya Order.

## Why It Matters

The Yasawiyya Order played a fundamental role in the spread of Islam throughout Central Asia.

Without this connection, the knowledge graph cannot properly represent the religious importance of the site.

---

# Gap 2 – Missing Representation as a Pilgrimage Site

## Observation

The mausoleum is widely recognized as a place of pilgrimage.

However, this role is not clearly represented through structured semantic relations in Wikidata.

## Why It Matters

Pilgrimage is one of the monument's most important social and religious functions.

Its absence reduces the cultural richness of the knowledge graph.

---

# Gap 3 – Missing Spiritual and Religious Significance

## Observation

The Wikidata entry contains historical and architectural information but provides very limited information regarding spiritual significance.

## Why It Matters

The mausoleum is an important symbol of Islamic spirituality and Sufi heritage.

Representing only physical characteristics fails to capture its broader cultural meaning.

---

# Gap 4 – Missing Links with Related Religious Heritage Sites

## Observation

No explicit semantic links were found between the mausoleum and other important religious heritage sites in Kazakhstan.

One example is the Arystan Bab Mausoleum.

## Why It Matters

Religious heritage sites often form cultural and historical networks.

Representing these relationships would improve navigation and contextual understanding within the knowledge graph.

---

# Summary of Identified Gaps

| Gap | Description |
|------|-------------|
| Gap 1 | Missing connection with the Yasawiyya Sufi Order |
| Gap 2 | Missing representation as a pilgrimage site |
| Gap 3 | Missing spiritual and religious significance |
| Gap 4 | Missing links with related religious heritage sites |

---

# From Gaps to RDF Enrichment

The identified gaps became the basis for the next phase of the project.

We used ChatGPT and Gemini to generate RDF triples that could enrich the Wikidata representation of the Mausoleum of Khoja Ahmed Yasawi and address the missing information discovered during our SPARQL exploration.
