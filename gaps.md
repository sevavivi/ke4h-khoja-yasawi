---
layout: null
---

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Knowledge Gaps | Mausoleum of Khoja Ahmed Yasawi</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@600;700&family=Inter:wght@400;500;700&display=swap" rel="stylesheet">

<style>
:root{
--dark:#170f0a;
--brown:#4a2d17;
--cream:#f8edd8;
--light:#fffaf0;
--gold:#d4af37;
--blue:#0f4c81;
--text:#2c2c2c;
}
*{box-sizing:border-box}
body{
margin:0;
font-family:Inter,sans-serif;
background:var(--cream);
color:var(--text);
line-height:1.75;
}
nav{
position:fixed;
top:0;
width:100%;
z-index:1000;
background:rgba(23,15,10,.9);
padding:16px;
text-align:center;
border-bottom:1px solid rgba(212,175,55,.5);
}
nav a{
color:white;
text-decoration:none;
margin:0 10px;
font-size:13px;
font-weight:700;
text-transform:uppercase;
}
nav a:hover{
color:var(--gold);
}
header{
min-height:50vh;
background:linear-gradient(rgba(23,15,10,.55),rgba(23,15,10,.82)),
url("images/IMG_8082.jpeg") center/cover;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
color:white;
padding:100px 20px;
}
header div{
background:rgba(23,15,10,.45);
padding:40px;
border:1px solid rgba(212,175,55,.7);
}
h1{
font-family:"Cormorant Garamond",serif;
font-size:64px;
margin:0;
}
main{
max-width:1050px;
margin:auto;
padding:70px 24px;
}
section{
background:white;
padding:40px;
margin-bottom:30px;
border:1px solid rgba(212,175,55,.5);
box-shadow:0 10px 30px rgba(0,0,0,.08);
}
h2{
font-family:"Cormorant Garamond",serif;
font-size:42px;
color:var(--brown);
border-bottom:1px solid var(--gold);
padding-bottom:10px;
}
.card{
background:#fff4df;
padding:20px;
margin:20px 0;
border-left:5px solid var(--gold);
}
footer{
background:var(--dark);
color:white;
text-align:center;
padding:35px;
border-top:3px solid var(--gold);
}
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
<h1>Knowledge Gaps</h1>
<p>Missing information identified through SPARQL analysis</p>
</div>
</header>

<main>

<section>

<h2>Identified Knowledge Gaps</h2>

<p>
The SPARQL investigation showed that Wikidata contains rich architectural and historical information about the Mausoleum of Khoja Ahmed Yasawi. However, several culturally significant aspects are missing or insufficiently represented.
</p>

<div class="card">
<h3>Missing Connection to the Yasawiyya Sufi Order</h3>
<p>
The mausoleum is strongly associated with the Yasawiyya Sufi tradition, but this relationship is not explicitly represented in Wikidata.
</p>
</div>

<div class="card">
<h3>Missing Pilgrimage Function</h3>
<p>
The site is an important pilgrimage destination in Central Asia, yet no direct statement identifies it as a pilgrimage site.
</p>
</div>

<div class="card">
<h3>Missing Spiritual Significance</h3>
<p>
The religious and spiritual importance of Khoja Ahmed Yasawi and his influence on Islamic culture are not adequately reflected.
</p>
</div>

<div class="card">
<h3>Limited Links to Related Heritage Sites</h3>
<p>
Connections between the mausoleum and other religious heritage sites in Kazakhstan are largely absent.
</p>
</div>

<div class="card">
<h3>Lack of Semantic Religious Context</h3>
<p>
Most existing information focuses on architecture and heritage status rather than religious meaning and cultural influence.
</p>
</div>

</section>

</main>

<footer>
Knowledge Engineering for the Humanities • University of Bologna • 2026
</footer>

</body>
</html>
