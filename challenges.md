---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Challenges | Mausoleum of Khoja Ahmet Yassawi</title>
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
h3{color:var(--blue)}
.card{background:#fff4df;padding:20px;margin:20px 0;border-left:5px solid var(--gold)}
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
<h1>Challenges</h1>
<p>Technical and conceptual difficulties faced during the project</p>
</div>
</header>

<main>

<section>
<h2>Challenges Faced</h2>

<div class="card">
<h3>1. Learning SPARQL</h3>
<p>
At the beginning of the project, writing SPARQL queries was difficult because we had to understand variables, properties, entity identifiers, filters, and query structure.
</p>
</div>

<div class="card">
<h3>2. No Matching Records</h3>
<p>
Some queries returned no results. Instead of treating this as a failure, we interpreted it as evidence that certain cultural and religious relationships are missing from Wikidata.
</p>
</div>

<div class="card">
<h3>3. Distinguishing Textual Information from Structured Data</h3>
<p>
Some information exists in Wikipedia or other textual sources, but it is not represented as structured data in Wikidata. This difference was important for identifying real knowledge gaps.
</p>
</div>

<div class="card">
<h3>4. Evaluating LLM Outputs</h3>
<p>
ChatGPT and Gemini sometimes produced different RDF triples. We had to manually compare the outputs and select only the triples that were relevant, accurate, and useful for knowledge graph enrichment.
</p>
</div>

<div class="card">
<h3>5. Modeling Cultural and Religious Meaning</h3>
<p>
Religious significance, pilgrimage practices, and spiritual heritage are difficult to represent through simple RDF triples. Human interpretation was necessary to avoid oversimplification.
</p>
</div>

</section>

<section>
<h2>Lessons Learned</h2>
<p>
This project showed that knowledge graph enrichment requires both technical skills and cultural interpretation. SPARQL helped us identify what is already represented, while LLMs helped generate possible enrichment ideas. However, human validation remained essential throughout the process.
</p>
</section>

</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
