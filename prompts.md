---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>LLM Prompts | Mausoleum of Khoja Ahmet Yassawi</title>
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
table{width:100%;border-collapse:collapse;background:white;margin-top:20px}
th,td{border:1px solid #d4af37;padding:14px;text-align:left;vertical-align:top}
th{background:#0f4c81;color:white}
.btn{display:inline-block;margin-top:20px;padding:13px 24px;background:var(--gold);color:#170f0a;text-decoration:none;font-weight:700;border:1px solid #f7ead0;text-transform:uppercase;letter-spacing:1px;font-size:13px}
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
<h1>LLM Prompts</h1>
<p>Comparison of ChatGPT and Gemini</p>
</div>
</header>

<main>

<section>
<h2>Use of Large Language Models</h2>
<p>
After identifying knowledge gaps in Wikidata, we used Large Language Models to generate possible RDF triples for enriching the representation of the Mausoleum of Khoja Ahmet Yassawi.
</p>
<p>
The goal was not to automatically insert information into Wikidata, but to evaluate whether LLMs could support knowledge graph enrichment.
</p>
</section>

<section>
<h2>Models Compared</h2>
<div class="card">
<h3>ChatGPT</h3>
<p>
ChatGPT produced focused and structured RDF suggestions that were closely aligned with the project research question.
</p>
</div>

<div class="card">
<h3>Gemini</h3>
<p>
Gemini provided broader contextual explanations and additional enrichment ideas, but its output sometimes required more filtering.
</p>
</div>
</section>

<section>
<h2>Prompting Techniques</h2>

<div class="card">
<h3>Zero-shot Prompting</h3>
<p>
The model was asked to generate RDF triples without examples. This helped test its basic understanding of the task.
</p>
</div>

<div class="card">
<h3>Few-shot Prompting</h3>
<p>
The model was given examples of RDF triples before generating new triples for the mausoleum.
</p>
</div>

<div class="card">
<h3>Chain-of-Thought Prompting</h3>
<p>
The model was asked to reason step by step before proposing final RDF triples.
</p>
</div>
</section>

<section>
<h2>Comparison of Models</h2>

<table>
<tr>
<th>Prompt Type</th>
<th>ChatGPT</th>
<th>Gemini</th>
<th>Assessment</th>
</tr>
<tr>
<td>Zero-shot</td>
<td>Focused and concise</td>
<td>Detailed and contextual</td>
<td>Both models were useful</td>
</tr>
<tr>
<td>Few-shot</td>
<td>Structured output</td>
<td>Strong adaptation to examples</td>
<td>Few-shot improved consistency</td>
</tr>
<tr>
<td>Chain-of-Thought</td>
<td>Most consistent</td>
<td>Most exploratory</td>
<td>Best results for enrichment ideas</td>
</tr>
</table>

<a class="btn" href="https://liveunibo-my.sharepoint.com/:x:/g/personal/sevara_abdulazizova_studio_unibo_it/IQAvce5I0pJ1R7a_eZSGPOm2Ad68NTYWqlaEer0eWgfFtm4?e=0bYS9I" target="_blank">
Open LLM Comparison Spreadsheet
</a>
</section>

<section>
<h2>Overall Evaluation</h2>
<p>
Both models were useful for supporting knowledge graph enrichment. However, ChatGPT produced the most focused RDF triples for the specific research question, while Gemini provided additional contextual information that could inspire future enrichment work.
</p>
<p>
The outputs generated by both models served as the basis for the RDF triples proposed in the next stage of the project.
</p>
</section>
<section>
<h2>External Comparison Spreadsheet</h2>

<p>
The complete comparison between ChatGPT and Gemini outputs can be accessed using the spreadsheet below:
</p>

<p>
<a href="https://liveunibo-my.sharepoint.com/:x:/g/personal/sevara_abdulazizova_studio_unibo_it/IQAvce5I0pJ1R7a_eZSGPOm2Ad68NTYWqlaEer0eWgfFtm4?e=0bYS9I" target="_blank">
Open LLM Comparison Spreadsheet
</a>
</p>

</section>
</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
