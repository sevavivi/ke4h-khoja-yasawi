# Mausoleum of Khoja Ahmed Yasawi

## Knowledge Engineering for the Humanities

### Team

- Gulnara Kozmet
- Abdulazizova Sevara

### Topic

Mausoleum of Khoja Ahmed Yasawi

### Research Question

How can Wikidata for the Mausoleum of Khoja Ahmed Yasawi be enriched through RDF triples and knowledge graph modeling?

---

## Knowledge Gaps

The current Wikidata entry for the Mausoleum of Khoja Ahmed Yasawi contains basic historical and architectural information.

However, several important aspects are underrepresented:

- Connection with the Yasawiyya Sufi Order
- Role as a pilgrimage site
- Spiritual and religious significance
- Connections with related religious heritage sites in Kazakhstan

These gaps limit the representation of the monument within a broader cultural and religious knowledge graph.

---

## SPARQL Queries

### Query 1: Basic Information

```sparql
SELECT ?item ?itemLabel WHERE {
  wd:Q485523 ?p ?item .
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
LIMIT 20
```

Result: Information about the Mausoleum of Khoja Ahmed Yasawi and related entities retrieved from Wikidata.

### Query 2: Related Heritage Sites

```sparql
SELECT ?site ?siteLabel WHERE {
  ?site wdt:P31 wd:Q839954 .
  SERVICE wikibase:label { bd:serviceParam wikibase:language "en". }
}
LIMIT 20
```

Result: Related cultural and heritage sites.

---

## LLM Evaluation

### Zero-shot Prompt

ChatGPT and Gemini were asked to generate RDF triples without examples.

**Result:** Both models identified religious and pilgrimage-related knowledge gaps.

### Few-shot Prompt

Example RDF triples were provided before the task.

**Result:** The generated triples became more structured and semantically consistent.

### Chain-of-Thought Prompt

Models were instructed to reason step-by-step before generating RDF triples.

**Result:** Both models produced richer explanations and more detailed RDF triples.

---

## Human Assessment

ChatGPT and Gemini produced useful RDF triples for all prompting strategies.

ChatGPT generally generated more concise and focused triples directly related to the research question.

Gemini often provided longer explanations and additional contextual information.

For Zero-shot prompting, both models successfully identified major knowledge gaps.

For Few-shot prompting, the quality of RDF triples improved due to the provided examples.

For Chain-of-Thought prompting, both models generated more detailed reasoning, but ChatGPT produced the most focused output for knowledge graph enrichment.

Overall, Chain-of-Thought prompting achieved the best results.

---

## RDF Enrichment

```rdf
:Mausoleum_of_Khoja_Ahmed_Yasawi :associatedWith :Yasawiyya_Sufi_Order .

:Mausoleum_of_Khoja_Ahmed_Yasawi :hasFunction :Pilgrimage_Site .

:Mausoleum_of_Khoja_Ahmed_Yasawi :associatedWith :Sufism .

:Mausoleum_of_Khoja_Ahmed_Yasawi :relatedHeritageSite :Arystan_Bab_Mausoleum .
```

These triples enrich Wikidata by representing religious traditions, pilgrimage practices, spiritual significance, and connections with other heritage sites.

---

## Conclusion

This project explored how Large Language Models can support knowledge graph enrichment for cultural heritage.

By analyzing the Wikidata entry of the Mausoleum of Khoja Ahmed Yasawi, several knowledge gaps were identified, particularly regarding religious significance, pilgrimage practices, and connections with other heritage sites.

ChatGPT and Gemini were evaluated using Zero-shot, Few-shot, and Chain-of-Thought prompting strategies.

The generated RDF triples successfully represented missing information and improved the semantic richness of the knowledge graph.

Among the tested approaches, Chain-of-Thought prompting produced the most detailed and useful enrichment suggestions.

This demonstrates the potential of LLMs as tools for supporting cultural heritage knowledge engineering.
