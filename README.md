<html>
<head>
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>VA Enterprise | Elite Security & Manpower</title>

<style>
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
  font-family:Arial, Helvetica, sans-serif;
}

body{
  background:#0a0f1c;
  color:white;
  overflow-x:hidden;
}

/* ===== NAVBAR ===== */
.navbar{
  position:fixed;
  width:100%;
  top:0;
  display:flex;
  justify-content:space-between;
  align-items:center;
  padding:20px 60px;
  background:rgba(0,0,0,0.85);
  backdrop-filter:blur(12px);
  z-index:1000;
}

.logo{
  font-size:26px;
  font-weight:bold;
  color:#FFD700;
  letter-spacing:2px;
}

.navbar a{
  color:white;
  text-decoration:none;
  margin-left:30px;
  transition:0.3s;
}

.navbar a:hover{
  color:#FFD700;
}

/* ===== HERO ===== */
.hero{
  height:100vh;
  display:flex;
  justify-content:center;
  align-items:center;
  flex-direction:column;
  text-align:center;
  background:linear-gradient(135deg,#000000,#1c1f2f,#002b5c);
  padding:20px;
}

.hero h1{
  font-size:55px;
  margin-bottom:20px;
  animation:fadeUp 1.5s ease;
}

.hero p{
  max-width:700px;
  margin-bottom:30px;
  opacity:0.85;
}

.btn{
  padding:15px 40px;
  border:none;
  border-radius:40px;
  background:#FFD700;
  color:black;
  font-weight:bold;
  cursor:pointer;
  transition:0.4s;
}

.btn:hover{
  transform:scale(1.15);
  background:#ffae00;
}

/* ===== SERVICES ===== */
.section{
  padding:120px 20px;
  text-align:center;
}

.cards{
  display:flex;
  justify-content:center;
  gap:40px;
  flex-wrap:wrap;
  margin-top:60px;
}

.card{
  background:rgba(255,255,255,0.05);
  padding:40px;
  width:300px;
  border-radius:20px;
  backdrop-filter:blur(10px);
  box-shadow:0 0 25px rgba(255,215,0,0.15);
  transition:0.5s;
  opacity:0;
  transform:translateY(80px);
}

.card:hover{
  transform:translateY(-15px);
  box-shadow:0 0 40px rgba(255,215,0,0.5);
}

/* ===== CONTACT ===== */
.contact-box{
  margin-top:40px;
  font-size:18px;
  line-height:30px;
}

/* ===== FOOTER ===== */
footer{
  background:black;
  padding:30px;
  text-align:center;
  color:gray;
}

/* ===== ANIMATION ===== */
@keyframes fadeUp{
  from{opacity:0; transform:translateY(60px);}
  to{opacity:1; transform:translateY(0);}
}

@media(max-width:768px){
  .navbar{
    flex-direction:column;
  }
}
</style>
</head>

<body>

<div class="navbar">
  <div class="logo">VA ENTERPRISE</div>
  <div>
    <a href="#home">Home</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </div>
</div>

<div class="hero" id="home">
  <h1>Elite Security & Professional Manpower</h1>
  <p>Providing disciplined, trained and verified security guards and manpower solutions for corporate offices, residential societies, industries and major events.</p>
  <button class="btn" onclick="showMessage()">Hire Now</button>
</div>

<div class="section" id="services">
  <h2>Our Premium Services</h2>
  <div class="cards">
    <div class="card">
      <h3>Armed & Unarmed Guards</h3>
      <p>Highly trained guards ensuring 24/7 protection and safety.</p>
    </div>

    <div class="card">
      <h3>Corporate Staffing</h3>
      <p>Professional manpower solutions tailored for business needs.</p>
    </div>

    <div class="card">
      <h3>Event & Industrial Security</h3>
      <p>Complete surveillance and crowd management services.</p>
    </div>
  </div>
</div>

<div class="section" id="contact">
  <h2>Contact VA Enterprise</h2>
  <div class="contact-box">
    📞 9426428671 <br>
    📞 9737382651 <br>
    📧 emailpa509192@gmail.com
  </div>
</div>

<footer>
  © 2026 VA Enterprise | All Rights Reserved
</footer>

<script>
function showMessage(){
  alert("Thank you for choosing VA Enterprise. Our team will contact you immediately.");
}

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
