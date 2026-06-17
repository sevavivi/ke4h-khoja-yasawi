---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>SPARQL | Mausoleum of Khoja Ahmet Yassawi</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{--dark:#170f0a;--brown:#4a2d17;--cream:#f8edd8;--light:#fffaf0;--gold:#d4af37;--blue:#0f4c81;--text:#2c2c2c}
*{box-sizing:border-box}
body{margin:0;font-family:Inter,sans-serif;background:var(--cream);color:var(--text);line-height:1.75}
nav{position:fixed;top:0;width:100%;z-index:1000;background:rgba(23,15,10,.9);backdrop-filter:blur(12px);padding:16px 20px;text-align:center;border-bottom:1px solid rgba(212,175,55,.55)}
nav a{color:white;text-decoration:none;margin:0 10px;font-size:13px;text-transform:uppercase;letter-spacing:1px;font-weight:700}
nav a:hover{color:var(--gold)}
header{min-height:55vh;background:linear-gradient(rgba(23,15,10,.55),rgba(23,15,10,.82)),url("images/image1.png") center/cover;display:flex;align-items:center;justify-content:center;text-align:center;color:white;padding:110px 20px 70px}
header div{max-width:900px;padding:45px;background:rgba(23,15,10,.48);border:1px solid rgba(212,175,55,.75)}
h1{font-family:"Cormorant Garamond",serif;font-size:64px;line-height:1;margin:0;color:#fff7df}
header p{font-size:19px;color:#f7ead0}
main{max-width:1050px;margin:0 auto;padding:70px 24px}
section{background:var(--light);padding:45px;margin-bottom:35px;border:1px solid rgba(212,175,55,.55);box-shadow:0 12px 35px rgba(0,0,0,.10)}
h2{font-family:"Cormorant Garamond",serif;color:var(--brown);font-size:44px;margin:0 0 20px;border-bottom:1px solid var(--gold);padding-bottom:12px}
h3{color:var(--blue);font-size:24px}
pre{background:#170f0a;color:#fff7df;padding:22px;overflow:auto;border-left:5px solid var(--gold);font-size:14px;line-height:1.6}
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
<h1>SPARQL Queries</h1>
<p>Exploring the Wikidata representation of the mausoleum</p>
</div>
</header>

<main>

<section>
<h2>SPARQL Investigation</h2>
<p>
This section presents the SPARQL queries used to investigate the Wikidata representation of the Mausoleum of Khoja Ahmet Yassawi and identify missing information.
</p>
</section>

<section>
<h2>Query 1 — Basic Information</h2>
<h3>Purpose</h3>
<p>Retrieve the basic properties associated with the Mausoleum of Khoja Ahmet Yassawi.</p>

<pre>SELECT ?propertyLabel ?valueLabel
WHERE {
  wd:Q46069 ?p ?value .
  ?property wikibase:directClaim ?p .

  FILTER(?property != wd:P18)

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?property rdfs:label ?propertyLabel .
    ?value rdfs:label ?valueLabel .
  }
}
LIMIT 20</pre>

<div class="card">
<strong>Result:</strong> The query returned information such as country, location, architectural style, material, UNESCO World Heritage status, and historical identifiers.
</div>
</section>

<section>
<h2>Query 2 — Ordered Properties</h2>
<h3>Purpose</h3>
<p>Retrieve a clearer ordered list of properties and values from Wikidata.</p>

<pre>SELECT ?propertyLabel ?valueLabel
WHERE {
  wd:Q46069 ?p ?value .
  ?property wikibase:directClaim ?p .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?property rdfs:label ?propertyLabel .
    ?value rdfs:label ?valueLabel .
  }
}
ORDER BY ?propertyLabel
LIMIT 15</pre>

<div class="card">
<strong>Result:</strong> The query showed structured data such as Commons category, World Heritage Site ID, World Heritage criteria, Wikikids ID, and other external identifiers.
</div>
</section>

<section>
<h2>Query 3 — Architect Information</h2>
<h3>Purpose</h3>
<p>Check whether Wikidata contains an architect relation for the mausoleum.</p>

<pre>SELECT ?itemLabel ?architectLabel
WHERE {
  VALUES ?item { wd:Q46069 }

  OPTIONAL { ?item wdt:P84 ?architect . }

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
  }
}</pre>

<div class="card">
<strong>Result:</strong> The query returned the mausoleum, but the architect field was empty. This shows that the architect information is not clearly represented.
</div>
</section>

<section>
<h2>Query 4 — Heritage Designation</h2>
<h3>Purpose</h3>
<p>Identify the heritage designation connected to the mausoleum.</p>

<pre>SELECT DISTINCT ?heritageLabel
WHERE {
  wd:Q46069 wdt:P1435 ?heritage .
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?heritage rdfs:label ?heritageLabel .
  }
}</pre>

<div class="card">
<strong>Result:</strong> The query returned World Heritage Site and Q4343708, confirming that Wikidata represents the monument as a heritage site.
</div>
</section>

<section>
<h2>Query 5 — Extended Properties</h2>
<h3>Purpose</h3>
<p>Retrieve a broader set of properties to identify what is present and what is missing.</p>

<pre>SELECT ?propertyLabel ?valueLabel
WHERE {
  wd:Q46069 ?p ?value .
  ?property wikibase:directClaim ?p .

  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?property rdfs:label ?propertyLabel .
    ?value rdfs:label ?valueLabel .
  }
}
LIMIT 50</pre>

<div class="card">
<strong>Result:</strong> The query returned 32 results, including country, image, instance of, commissioned by Timur, location, architectural style, material, coordinates, heritage designation, and World Heritage criteria.
</div>
</section>

<section>
<h2>Summary</h2>
<p>
The SPARQL investigation demonstrated that Wikidata provides useful historical, geographical, and architectural information about the Mausoleum of Khoja Ahmet Yassawi.
</p>
<p>
However, important religious, spiritual, and pilgrimage-related aspects remain underrepresented. These findings motivated the RDF enrichment phase of the project.
</p>
</section>

</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
