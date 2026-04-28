<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Smart Uro</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif;}
body{background:#0f172a;color:#fff;}
header{display:flex;justify-content:space-between;align-items:center;padding:20px 50px;}
header h1{color:#38bdf8;}
nav a{color:#fff;margin-left:20px;text-decoration:none;}
.hero{height:90vh;display:flex;flex-direction:column;justify-content:center;align-items:center;text-align:center;padding:20px;}
.hero h2{font-size:3rem;max-width:800px;}
.hero p{margin:20px 0;opacity:0.8;}
.btn{padding:12px 25px;background:#38bdf8;border:none;border-radius:30px;color:#000;font-weight:600;cursor:pointer;transition:0.3s;}
.btn:hover{transform:scale(1.05);}
.section{padding:80px 20px;text-align:center;}
.cards{display:grid;grid-template-columns:repeat(auto-fit,minmax(220px,1fr));gap:20px;margin-top:40px;}
.card{background:#1e293b;padding:20px;border-radius:15px;transition:0.3s;}
.card:hover{transform:translateY(-10px);}
.fade{opacity:0;transform:translateY(40px);transition:1s;}
.fade.show{opacity:1;transform:translateY(0);}
footer{padding:30px;text-align:center;background:#020617;margin-top:50px;}
</style>
</head>
<body>

<header>
<h1>Smart Uro</h1>
<nav>
<a href="#">Home</a>
<a href="#features">Features</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero">
<h2 class="fade">Smarter Care for Those Who Need It Most</h2>
<p class="fade">Real-time urinary health monitoring for elderly and bedridden patients</p>
<button class="btn fade">Book a Demo</button>
</section>

<section class="section fade">
<h2>The Problem</h2>
<p>Caregivers often miss early signs of urinary issues, leading to infections and complications.</p>
</section>

<section id="features" class="section fade">
<h2>Why Smart Uro?</h2>
<div class="cards">
<div class="card">24/7 Monitoring</div>
<div class="card">Real-Time Alerts</div>
<div class="card">Reduce Caregiver Stress</div>
<div class="card">Improve Patient Safety</div>
</div>
</section>

<section class="section fade">
<h2>How It Works</h2>
<p>Smart sensors track urinary patterns and send instant alerts to caregivers.</p>
</section>

<section id="contact" class="section fade">
<h2>Get Started</h2>
<p>Email: smarturo@gmail.com</p>
<p>Phone: +91-XXXXXXXXXX</p>
<button class="btn">Contact Us</button>
</section>

<footer>
<p>© 2026 Smart Uro</p>
</footer>

<script>
const fades = document.querySelectorAll('.fade');
window.addEventListener('scroll', () => {
  fades.forEach(f => {
    const top = f.getBoundingClientRect().top;
    if(top < window.innerHeight - 100){
      f.classList.add('show');
    }
  });
});
</script>

</body>
</html>
