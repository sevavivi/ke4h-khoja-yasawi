# Mausoleum of Khoja Ahmed Yasawi

## Knowledge Engineering for the Humanities

### Team
- Abdulazizova Sevara
- Kozmet Gulnara

### Topic
Mausoleum of Khoja Ahmed Yasawi

### Research Question
How can Wikidata for the Mausoleum of Khoja Ahmed Yasawi be enriched through RDF triples and knowledge graph modeling?

### Sections
- SPARQL Queries
- Knowledge Gaps
- LLM Evaluation
- RDF Enrichment
- Conclusion
- # Mausoleum of Khoja Ahmed Yasawi

...

### Sections

- SPARQL Queries
- Knowledge Gaps
- LLM Evaluation
- RDF Enrichment
- Conclusion

---

## Knowledge Gaps

The current Wikidata entry for the Mausoleum of Khoja Ahmed Yasawi contains basic historical and architectural information.

However, several important aspects are underrepresented:

- Connection with the Yasawiyya Sufi Order
- Role as a pilgrimage site
- Spiritual and religious significance
- Connections with related religious heritage sites in Kazakhstan

---

## LLM Evaluation

### Zero-shot Prompt

ChatGPT and Gemini were asked to generate RDF triples without examples.

Result:
Both models identified religious and pilgrimage-related knowledge gaps.

### Few-shot Prompt

Example RDF triples were provided before the task.

Result:
The generated triples became more structured and semantically consistent.

### Chain-of-Thought Prompt

Models were instructed to reason step-by-step before generating RDF triples.

Result:
Both models produced richer explanations and more detailed RDF triples.

---

## RDF Enrichment

```rdf
:Mausoleum_of_Khoja_Ahmed_Yasawi :associatedWith :Yasawiyya_Sufi_Order .
:Mausoleum_of_Khoja_Ahmed_Yasawi :hasFunction :Pilgrimage_Site .
:Mausoleum_of_Khoja_Ahmed_Yasawi :associatedWith :Sufism .
:Mausoleum_of_Khoja_Ahmed_Yasawi :relatedHeritageSite :Arystan_Bab_Mausoleum .
## Conclusion

This project explored how Large Language Models can support knowledge graph enrichment for cultural heritage.

By analyzing the Wikidata entry of the Mausoleum of Khoja Ahmed Yasawi, several knowledge gaps were identified, particularly regarding religious significance, pilgrimage practices, and connections with other heritage sites.

ChatGPT and Gemini were evaluated using Zero-shot, Few-shot, and Chain-of-Thought prompting strategies.

The generated RDF triples successfully represented missing information and improved the semantic richness of the knowledge graph.

Among the tested approaches, Chain-of-Thought prompting produced the most detailed and useful enrichment suggestions.

This demonstrates the potential of LLMs as tools for supporting cultural heritage knowledge engineering.
