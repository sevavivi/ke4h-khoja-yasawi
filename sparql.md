---
layout: default
title: SPARQL Queries
---
[Home](index.html) | [Topic](topic.html) | [Methodology](methodology.html) | [RDF Triples](rdf.html) | [SPARQL](sparql.html) | [Gaps](gaps.html) | [LLM Prompts](prompts.html) | [Challenges](challenges.html) | [Conclusion](conclusion.html)

---
# SPARQL Queries

This section presents the SPARQL queries used to investigate the Wikidata representation of the Mausoleum of Khoja Ahmed Yasawi and identify missing information.

---

# Query 1 – Basic Information

## Purpose

Retrieve the basic properties associated with the Mausoleum of Khoja Ahmed Yasawi.

```sparql
SELECT ?property ?propertyLabel ?value ?valueLabel
WHERE {
  wd:Q46069 ?property ?value .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}
LIMIT 50
```

## Results

The query returned information about:

- Location
- Country
- UNESCO World Heritage status
- Architectural style
- Historical period

### Proof of Execution

Insert screenshot of query results here.

---

# Query 2 – Religious Associations

## Purpose

Investigate whether the mausoleum is directly linked to religious organizations or traditions.

```sparql
SELECT ?item ?itemLabel
WHERE {
  wd:Q46069 ?p ?item .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}
LIMIT 50
```

## Results

No explicit connection with the Yasawiyya Sufi Order was found.

### Proof of Execution

Insert screenshot of query results here.

---

# Query 3 – Pilgrimage Function

## Purpose

Check whether the mausoleum is represented as a pilgrimage site.

```sparql
SELECT ?type ?typeLabel
WHERE {
  wd:Q46069 wdt:P31 ?type .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}
```

## Results

The query did not reveal a direct representation of pilgrimage-related functions.

### Proof of Execution

Insert screenshot of query results here.

---

# Query 4 – Related Heritage Sites

## Purpose

Identify heritage sites located in Kazakhstan that could be semantically connected to the mausoleum.

```sparql
SELECT ?site ?siteLabel
WHERE {
  ?site wdt:P17 wd:Q232 .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}
LIMIT 50
```

## Results

Several cultural heritage sites were retrieved, but no explicit semantic links with the mausoleum were identified.

### Proof of Execution

Insert screenshot of query results here.

---

# Query 5 – Cultural and Religious Context

## Purpose

Explore entities connected with Khoja Ahmed Yasawi and his cultural influence.

```sparql
SELECT ?related ?relatedLabel
WHERE {
  ?related ?p wd:Q46069 .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}
LIMIT 50
```

## Results

The query revealed only limited contextual information and highlighted missing cultural relationships.

### Proof of Execution

Insert screenshot of query results here.

---

# Summary

The SPARQL investigation demonstrated that Wikidata provides rich historical and architectural information about the Mausoleum of Khoja Ahmed Yasawi.

However, important religious, spiritual, and pilgrimage-related aspects remain underrepresented. These findings motivated the RDF enrichment phase of the project.
