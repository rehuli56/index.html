<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ultimate Mensuration Learning Hub</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">
<style>
body{font-family:'Poppins',sans-serif;margin:0;background:#eef2f7;color:#222}
header{background:linear-gradient(135deg,#1e3c72,#2a5298);color:white;padding:30px;text-align:center}
nav{background:#142850;padding:12px;text-align:center}
nav a{color:white;margin:12px;text-decoration:none;font-weight:500}
section{padding:30px}
.card{background:white;padding:20px;margin:20px 0;border-radius:15px;box-shadow:0 5px 15px rgba(0,0,0,0.1)}
h2{color:#1e3c72}
button{padding:10px 15px;border:none;border-radius:8px;background:#1e3c72;color:white;cursor:pointer;margin:5px}
button:hover{background:#16325c}
input{padding:8px;margin:5px}
footer{background:#142850;color:white;text-align:center;padding:15px}
.quiz-score{font-weight:bold;margin-top:10px}
svg{margin-top:15px}
</style>
</head>
<body>

<header>
<h1>Ultimate Mensuration Learning Hub</h1>
<p>Complete Notes | Diagrams | Practice | Full Tests | Downloadable Material</p>
</header>

<nav>
<a href="#notes">Notes</a>
<a href="#formulas">Formulas</a>
<a href="#diagrams">Diagrams</a>
<a href="#practice">Practice</a>
<a href="#test">Full Test</a>
<a href="#download">Download</a>
</nav>

<section id="notes">
<h2>Complete Chapter Notes (ICSE/CBSE)</h2>
<div class="card">
<h3>2D Shapes</h3>
<p>Rectangle → Area = l × b | Perimeter = 2(l + b)</p>
<p>Square → Area = a² | Perimeter = 4a</p>
<p>Triangle → Area = 1/2 × base × height</p>
<p>Circle → Area = πr² | Circumference = 2πr</p>
</div>
<div class="card">
<h3>3D Solids</h3>
<p>Cube → Volume = a³ | TSA = 6a²</p>
<p>Cuboid → Volume = lbh | TSA = 2(lb + bh + hl)</p>
<p>Cylinder → Volume = πr²h | TSA = 2πr(h+r)</p>
<p>Sphere → Volume = 4/3 πr³ | Surface Area = 4πr²</p>
<p>Cone → Volume = 1/3 πr²h | CSA = πrl</p>
</div>
</section>

<section id="formulas">
<h2>Quick Formula Sheet</h2>
<div class="card">
<p>π = 22/7 or 3.14</p>
<p>Diagonal of Cube = a√3</p>
<p>Diagonal of Cuboid = √(l² + b² + h²)</p>
<p>Slant Height of Cone = √(r² + h²)</p>
</div>
</section>

<section id="diagrams">
<h2>Shape Diagrams</h2>
<div class="card">
<h3>Rectangle</h3>
<svg width="200" height="120">
<rect x="20" y="20" width="150" height="80" stroke="black" fill="lightblue"/>
</svg>
<h3>Circle</h3>
<svg width="200" height="150">
<circle cx="100" cy="75" r="50" stroke="black" fill="lightgreen"/>
</svg>
<h3>Cylinder</h3>
<svg width="200" height="200">
<ellipse cx="100" cy="40" rx="60" ry="20" fill="lightgray" stroke="black"/>
<rect x="40" y="40" width="120" height="100" fill="lightgray" stroke="black"/>
<ellipse cx="100" cy="140" rx="60" ry="20" fill="lightgray" stroke="black"/>
</svg>
</div>
</section>

<section id="practice">
<h2>Practice Questions</h2>
<div class="card">
<p>1. Find area of rectangle (l=12 cm, b=8 cm).</p>
<p>2. Find circumference of circle (r=14 cm).</p>
<p>3. Find volume of cylinder (r=7 cm, h=10 cm).</p>
<p>4. Find TSA of cube (a=5 cm).</p>
<p>5. A sphere has radius 7 cm. Find surface area.</p>
</div>
</section>

<section id="test">
<h2>Interactive Full Test</h2>
<div class="card">
<p>1. Area of square (side=9 cm):</p>
<button onclick="answer(1,81)">81</button>
<button onclick="answer(1,72)">72</button>

<p>2. Volume of cube (side=3 cm):</p>
<button onclick="answer(2,27)">27</button>
<button onclick="answer(2,18)">18</button>

<p>3. Circumference of circle (r=7, π=22/7):</p>
<button onclick="answer(3,44)">44</button>
<button onclick="answer(3,49)">49</button>

<div class="quiz-score" id="score"></div>
</div>
</section>

<section id="download">
<h2>Download Notes</h2>
<div class="card">
<p>Click below to download printable Mensuration Notes (PDF ready).</p>
<button onclick="downloadNotes()">Download PDF</button>
</div>
</section>

<footer>
<p>© 2026 Ultimate Mensuration Learning Hub | Built for Complete Mastery</p>
</footer>

<script>
let totalScore = 0;
function answer(q, correct){
if((q==1 && correct==81) || (q==2 && correct==27) || (q==3 && correct==44)){
totalScore++;
document.getElementById('score').innerHTML = "Correct! Current Score: " + totalScore;
}else{
document.getElementById('score').innerHTML = "Wrong! Current Score: " + totalScore;
}
}

function downloadNotes(){
alert("PDF Download feature can be connected using backend or file link.");
}
</script>

</body>
</html>
