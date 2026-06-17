---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Methodology | Mausoleum of Khoja Ahmet Yassawi</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{--dark:#170f0a;--brown:#4a2d17;--cream:#f8edd8;--light:#fffaf0;--gold:#d4af37;--blue:#0f4c81;--text:#2c2c2c}
*{box-sizing:border-box}
body{margin:0;font-family:Inter,sans-serif;background:var(--cream);color:var(--text);line-height:1.75}
nav{position:fixed;top:0;width:100%;z-index:1000;background:rgba(23,15,10,.9);backdrop-filter:blur(12px);padding:16px 20px;text-align:center;border-bottom:1px solid rgba(212,175,55,.55)}
nav a{color:white;text-decoration:none;margin:0 10px;font-size:13px;text-transform:uppercase;letter-spacing:1px;font-weight:700}
nav a:hover{color:var(--gold)}
header{min-height:55vh;background:linear-gradient(rgba(23,15,10,.55),rgba(23,15,10,.82)),url("images/IMG_8082.jpeg") center/cover;display:flex;align-items:center;justify-content:center;text-align:center;color:white;padding:110px 20px 70px}
header div{max-width:900px;padding:45px;background:rgba(23,15,10,.48);border:1px solid rgba(212,175,55,.75)}
h1{font-family:"Cormorant Garamond",serif;font-size:64px;line-height:1;margin:0;color:#fff7df}
header p{font-size:19px;color:#f7ead0}
main{max-width:1050px;margin:0 auto;padding:70px 24px}
section{background:var(--light);padding:45px;margin-bottom:35px;border:1px solid rgba(212,175,55,.55);box-shadow:0 12px 35px rgba(0,0,0,.10)}
h2{font-family:"Cormorant Garamond",serif;color:var(--brown);font-size:44px;margin:0 0 20px;border-bottom:1px solid var(--gold);padding-bottom:12px}
h3{color:var(--blue);font-size:24px}
.card{background:#fff4df;padding:22px;margin:18px 0;border-left:5px solid var(--gold)}
footer{background:var(--dark);color:white;text-align:center;padding:35px;border-top:3px solid var(--gold)}
@media(max-width:760px){nav{position:static}nav a{display:inline-block;margin:5px 7px}h1{font-size:44px}section{padding:28px}}
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
<h1>Methodology</h1>
<p>Research approach and knowledge graph enrichment process</p>
</div>
</header>

<main>

<section>
<h2>Methodology</h2>
<p>
To achieve our goal, we developed a step-by-step methodology for exploring and enriching the Wikidata representation of the Mausoleum of Khoja Ahmet Yassawi.
</p>

<div class="card">
<h3>1. Selecting the Topic</h3>
<p>
We selected the mausoleum because it is an important example of Islamic and Timurid architectural heritage in Kazakhstan.
</p>
</div>

<div class="card">
<h3>2. Exploring Wikidata</h3>
<p>
We started by examining the Wikidata entry of the Mausoleum of Khoja Ahmet Yassawi to understand what information was already available in the knowledge graph.
</p>
</div>

<div class="card">
<h3>3. Creating SPARQL Queries</h3>
<p>
We wrote SPARQL queries to retrieve information about the monument, including its properties, classifications, location, and related entities.
</p>
</div>

<div class="card">
<h3>4. Identifying Knowledge Gaps</h3>
<p>
We compared the retrieved data with the cultural and religious significance of the site. This allowed us to identify missing information connected with Sufism, pilgrimage, and the Yasawiyya tradition.
</p>
</div>

<div class="card">
<h3>5. Using LLMs</h3>
<p>
We used ChatGPT and Gemini to support the generation of possible RDF triples and to compare how different prompting strategies influenced the results.
</p>
</div>

<div class="card">
<h3>6. Proposing RDF Triples</h3>
<p>
Finally, we proposed RDF triples that could enrich the Wikidata representation with additional cultural, religious, and spiritual information related to the Mausoleum of Khoja Ahmet Yassawi.
</p>
</div>
</section>
<div class="card">
<h3>Tools Used</h3>
<p>
Wikidata, Wikidata Query Service (SPARQL), ChatGPT, Gemini, and GitHub Pages.
</p>
</div>
</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
