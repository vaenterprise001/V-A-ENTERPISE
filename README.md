<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VA Enterprise | Manpower & Security Services</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family: 'Segoe UI', sans-serif;
}

body{
    background:#0f172a;
    color:white;
    scroll-behavior:smooth;
}

header{
    background:#111827;
    padding:20px 0;
    position:fixed;
    width:100%;
    top:0;
    z-index:1000;
}

nav{
    display:flex;
    justify-content:center;
    gap:40px;
}

nav a{
    color:white;
    text-decoration:none;
    font-weight:bold;
    transition:0.3s;
}

nav a:hover{
    color:#38bdf8;
}

section{
    padding:100px 20px;
    text-align:center;
}

.hero{
    background:linear-gradient(rgba(0,0,0,0.6), rgba(0,0,0,0.8)),
    url('https://images.unsplash.com/photo-1581090700227-4c4d2f5c4b3c');
    background-size:cover;
    background-position:center;
    height:100vh;
    display:flex;
    flex-direction:column;
    justify-content:center;
    align-items:center;
}

.hero h1{
    font-size:50px;
}

.hero p{
    margin:20px 0;
    font-size:20px;
}

.btn{
    background:#38bdf8;
    padding:12px 25px;
    border-radius:30px;
    text-decoration:none;
    color:black;
    font-weight:bold;
    transition:0.3s;
}

.btn:hover{
    background:white;
}

.services{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:30px;
    margin-top:40px;
}

.card{
    background:#1e293b;
    padding:30px;
    width:280px;
    border-radius:15px;
    transition:0.3s;
}

.card:hover{
    transform:translateY(-10px);
}

footer{
    background:#111827;
    padding:20px;
    text-align:center;
}
</style>
</head>

<body>

<header>
<nav>
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#services">Services</a>
<a href="#contact">Contact</a>
</nav>
</header>

<section class="hero" id="home">
<h1>VA ENTERPRISE</h1>
<p>Professional Manpower & Security Guard Services</p>
<a href="#contact" class="btn">Get Free Quote</a>
</section>

<section id="about">
<h2>About Us</h2>
<p style="margin-top:20px; max-width:700px; margin-left:auto; margin-right:auto;">
VA Enterprise provides highly trained security guards and reliable manpower 
for industries, offices, apartments, hospitals, and events. 
We ensure safety, discipline, and professionalism in every assignment.
</p>
</section>

<section id="services">
<h2>Our Services</h2>
<div class="services">

<div class="card">
<h3>Security Guards</h3>
<p>Professional trained guards for residential and commercial security.</p>
</div>

<div class="card">
<h3>Industrial Manpower</h3>
<p>Skilled & unskilled manpower for factories and corporate offices.</p>
</div>

<div class="card">
<h3>Event Security</h3>
<p>Complete security arrangements for events and public gatherings.</p>
</div>

</div>
</section>

<section id="contact">
<h2>Contact Us</h2>
<p style="margin-top:20px;">
📞 Phone: <a href="tel:9737382651" style="color:#38bdf8;">9737382651</a>
</p>
<p>
📧 Email: <a href="mailto:vaentreprise@gmail.com" style="color:#38bdf8;">vaentreprise@gmail.com</a>
</p>
</section>

<footer>
<p>© 2026 VA Enterprise | All Rights Reserved</p>
</footer>

</body>
</html>
