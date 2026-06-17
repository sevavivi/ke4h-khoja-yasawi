---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Conclusion | Mausoleum of Khoja Ahmet Yassawi</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{--dark:#170f0a;--brown:#4a2d17;--cream:#f8edd8;--light:#fffaf0;--gold:#d4af37;--blue:#0f4c81;--text:#2c2c2c}
*{box-sizing:border-box}
body{margin:0;font-family:Inter,sans-serif;background:var(--cream);color:var(--text);line-height:1.75}
nav{position:fixed;top:0;width:100%;z-index:1000;background:rgba(23,15,10,.9);padding:16px;text-align:center;border-bottom:1px solid rgba(212,175,55,.5)}
nav a{color:white;text-decoration:none;margin:0 10px;font-size:13px;font-weight:700;text-transform:uppercase}
nav a:hover{color:var(--gold)}
header{min-height:50vh;background:linear-gradient(rgba(23,15,10,.55),rgba(23,15,10,.82)),url("images/image1.png") center/cover;display:flex;justify-content:center;align-items:center;text-align:center;color:white;padding:100px 20px}
header div{background:rgba(23,15,10,.45);padding:40px;border:1px solid rgba(212,175,55,.7)}
h1{font-family:"Cormorant Garamond",serif;font-size:64px;margin:0}
main{max-width:1050px;margin:auto;padding:70px 24px}
section{background:white;padding:40px;margin-bottom:30px;border:1px solid rgba(212,175,55,.5);box-shadow:0 10px 30px rgba(0,0,0,.08)}
h2{font-family:"Cormorant Garamond",serif;font-size:42px;color:var(--brown);border-bottom:1px solid var(--gold);padding-bottom:10px}
footer{background:var(--dark);color:white;text-align:center;padding:35px;border-top:3px solid var(--gold)}
</style>
</head>

<body>

<nav>
<a href="index.html">Home</a>
<a href="topic.html">Topic</a>
<a href="methodology.html">Methodology</a>
<a href="sparql.html">SPARQL</a>
<a href="gaps.html">Gaps</a>
<a href="prompts.html">LLM Prompts</a>
<a href="rdf.html">RDF</a>
<a href="challenges.html">Challenges</a>
<a href="conclusion.html">Conclusion</a>
</nav>

<header>
<div>
<h1>Conclusion</h1>
</div>
</header>

<main>

<section>

<h2>Project Summary</h2>

<p>
This project explored how knowledge graph technologies can be used to enrich the representation of cultural heritage in Wikidata through the case of the Mausoleum of Khoja Ahmet Yassawi.
</p>

<p>
Using SPARQL queries, we investigated the existing Wikidata representation and identified several important knowledge gaps related to the Yasawiyya Sufi Order, pilgrimage functions, spiritual significance, and connections with related religious heritage sites.
</p>

<p>
To address these gaps, we evaluated the outputs of ChatGPT and Gemini using Zero-shot, Few-shot, and Chain-of-Thought prompting techniques. Based on the generated suggestions and our own analysis, we proposed RDF triples that could enrich the knowledge graph.
</p>

<p>
The results demonstrate that Large Language Models can support knowledge graph enrichment by generating useful semantic relationships. However, human evaluation remains essential to verify relevance, accuracy, and cultural appropriateness.
</p>

<p>
Overall, the project showed how SPARQL, RDF, Wikidata, and LLMs can be combined to improve the representation of cultural heritage knowledge in a structured and meaningful way.
</p>

</section>

</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
