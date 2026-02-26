<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VA Enterprise | Professional Manpower & Security</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family: 'Segoe UI', sans-serif;
  scroll-behavior:smooth;
}

body{
  background:#0f172a;
  color:white;
}

/* ===== HEADER ===== */
header{
  position:fixed;
  top:0;
  width:100%;
  background:rgba(0,0,0,0.85);
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:20px 50px;
  z-index:1000;
}

header h1{
  color:gold;
  letter-spacing:2px;
}

nav a{
  color:white;
  text-decoration:none;
  margin-left:25px;
  transition:0.3s;
  font-weight:500;
}

nav a:hover{
  color:gold;
}

/* ===== HERO ===== */
.hero{
  min-height:100vh;
  padding-top:140px;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  background:linear-gradient(to right,#000428,#004e92);
}

.hero h2{
  font-size:48px;
  margin-bottom:20px;
  animation:fadeDown 1.5s ease;
}

.hero p{
  max-width:650px;
  margin-bottom:30px;
  opacity:0.9;
}

.btn{
  padding:15px 40px;
  border:none;
  border-radius:30px;
  background:gold;
  color:black;
  font-weight:bold;
  cursor:pointer;
  transition:0.4s;
}

.btn:hover{
  transform:scale(1.1);
  background:orange;
}

/* ===== SECTIONS ===== */
section{
  padding:100px 20px;
  text-align:center;
}

.services{
  display:flex;
  flex-wrap:wrap;
  justify-content:center;
  gap:30px;
  margin-top:50px;
}

.card{
  background:#1e293b;
  padding:30px;
  width:300px;
  border-radius:15px;
  transition:0.6s;
  box-shadow:0 0 20px rgba(255,215,0,0.2);
  opacity:0;
  transform:translateY(60px);
}

.card:hover{
  transform:translateY(-10px);
  box-shadow:0 0 30px gold;
}

/* ===== FOOTER ===== */
footer{
  background:black;
  padding:30px;
  text-align:center;
  color:gray;
}

/* ===== ANIMATIONS ===== */
@keyframes fadeDown{
  from{opacity:0; transform:translateY(-50px);}
  to{opacity:1; transform:translateY(0);}
}

/* ===== RESPONSIVE ===== */
@media(max-width:768px){
  header{
    flex-direction:column;
  }
  nav{
    margin-top:10px;
  }
}
</style>
</head>

<body>

<header>
  <h1>VA ENTERPRISE</h1>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero" id="home">
  <h2>Professional Manpower & Security Solutions</h2>
  <p>We provide highly trained security guards and trusted manpower services for corporate offices, residential societies, industries and events.</p>
  <button class="btn" onclick="showMessage()">Request Service</button>
</div>

<section id="about">
  <h2>About VA Enterprise</h2>
  <p style="max-width:700px;margin:20px auto;">
    VA Enterprise is committed to delivering disciplined manpower and top-tier security services with professionalism, reliability and excellence.
  </p>
</section>

<section id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div class="card">
      <h3>Security Guards</h3>
      <p>Certified and trained guards ensuring complete protection.</p>
    </div>

    <div class="card">
      <h3>Corporate Manpower</h3>
      <p>Professional staffing solutions tailored for industries.</p>
    </div>

    <div class="card">
      <h3>Event Security</h3>
      <p>Reliable event monitoring and crowd management services.</p>
    </div>
  </div>
</section>

<section id="contact">
  <h2>Contact Us</h2>
  <p>Email: info@vaenterprise.com</p>
  <p>Phone: +91 9876543210</p>
</section>

<footer>
  © 2026 VA Enterprise | All Rights Reserved
</footer>

<script>
function showMessage(){
  alert("Thank you for choosing VA Enterprise. Our team will contact you soon.");
}

/* Scroll Animation */
window.addEventListener("scroll",function(){
  const cards=document.querySelectorAll(".card");
  cards.forEach(card=>{
    const position=card.getBoundingClientRect().top;
    const screenHeight=window.innerHeight;
    if(position < screenHeight-100){
      card.style.opacity="1";
      card.style.transform="translateY(0)";
    }
  });
});
</script>

</body>
</html>
