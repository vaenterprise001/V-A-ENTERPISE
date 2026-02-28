
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VA Enterprise | Manpower & Security Services</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif}
body{background:#f4f7fb;color:#1f2937;overflow-x:hidden}

/* Welcome Screen */
#welcome{
position:fixed;
top:0;left:0;
width:100%;height:100%;
background:#0f172a;
color:white;
display:flex;
justify-content:center;
align-items:center;
flex-direction:column;
z-index:9999;
animation:fadeOut 1s ease 3s forwards;
}
#welcome h1{
font-size:40px;
letter-spacing:3px;
animation:zoomIn 1.5s ease;
}
#welcome p{
margin-top:10px;
opacity:0.8;
}

@keyframes zoomIn{
from{transform:scale(0.5);opacity:0}
to{transform:scale(1);opacity:1}
}
@keyframes fadeOut{
to{opacity:0;visibility:hidden}
}

.topbar{background:#0f172a;color:white;padding:10px 20px;display:flex;justify-content:space-between;flex-wrap:wrap;font-size:14px}
header{display:flex;justify-content:space-between;align-items:center;padding:20px 40px;background:white;box-shadow:0 4px 20px rgba(0,0,0,0.05)}
header h1{font-size:26px;font-weight:700;color:#0f172a}

.btn{background:#1d4ed8;color:white;padding:12px 24px;border-radius:30px;text-decoration:none;font-weight:500;transition:0.3s}
.btn:hover{background:#1e40af;transform:scale(1.05)}

.hero{padding:100px 40px;background:linear-gradient(to right,#ffffff,#e0ecff);display:flex;flex-wrap:wrap;align-items:center;justify-content:space-between}
.hero-text{flex:1;min-width:280px}
.hero-text h2{font-size:42px;margin-bottom:20px;color:#0f172a}
.hero-text p{font-size:18px;margin-bottom:30px;color:#374151}

.typing{border-right:3px solid #1d4ed8;white-space:nowrap;overflow:hidden;animation:typing 3s steps(40,end),blink .7s infinite}
@keyframes typing{from{width:0}to{width:100%}}
@keyframes blink{50%{border-color:transparent}}

.hero-box{flex:1;min-width:280px;background:white;padding:40px;border-radius:20px;box-shadow:0 20px 40px rgba(0,0,0,0.08);transition:0.5s}
.hero-box:hover{transform:translateY(-10px)}

.section{padding:80px 40px;text-align:center}
.section h3{font-size:36px;margin-bottom:50px;color:#0f172a}

.services{display:flex;flex-wrap:wrap;gap:30px;justify-content:center}
.card{background:white;padding:30px;border-radius:20px;box-shadow:0 10px 30px rgba(0,0,0,0.06);width:300px;transition:0.4s}
.card:hover{transform:translateY(-15px) scale(1.03)}
.card h4{margin-bottom:15px;color:#1d4ed8}

.contact{background:#0f172a;color:white;padding:60px 20px;text-align:center}
.contact p{margin:10px 0;font-size:18px}

footer{background:black;color:#aaa;text-align:center;padding:20px}

@media(max-width:768px){.hero{flex-direction:column;text-align:center}}
</style>
</head>
<body>

<!-- Welcome Animation -->
<div id="welcome">
<h1>WELCOME TO VA ENTERPRISE</h1>
<p>Professional Manpower & Security Services</p>
</div>

<div class="topbar">
<div>Professional Manpower & Security Solutions</div>
<div>📞 9737382651 | 9426428671 &nbsp; | &nbsp; ✉ pa509192@gmail.com</div>
</div>

<header>
<h1>VA ENTERPRISE</h1>
<a href="#contact" class="btn">Request Service</a>
</header>

<section class="hero">
<div class="hero-text">
<h2 class="typing">Trusted Security & Skilled Workforce Provider</h2>
<p>VA Enterprise delivers reliable security guard services and manpower solutions for industries, corporate offices and residential projects.</p>
<a href="#contact" class="btn">Get Free Consultation</a>
</div>

</section>

<section class="section">
<h3>Our Core Services</h3>
<div class="services">
<div class="card">
<h4>Security Guard Services</h4>
<p>Professional guards ensuring safety and surveillance for all types of properties.</p>
</div>
<div class="card">
<h4>Industrial Manpower</h4>
<p>Reliable workforce solutions for factories, warehouses and large-scale projects.</p>
</div>
<div class="card">
<h4>Corporate Staffing</h4>
<p>Efficient staffing solutions tailored for office and corporate environments.</p>
</div>
</div>
</section>

<section class="contact" id="contact">
<h3>Contact VA Enterprise</h3>
<p>📞 9737382651 / 9426428671</p>
<p>✉ pa509192@gmail.com</p>
<p>Serving Across Gujarat, India</p>
</section>

<footer>
© 2026 VA Enterprise. All Rights Reserved.
</footer>

</body>
</html>
