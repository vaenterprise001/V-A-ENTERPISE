<!DOCTYPE html>
<html>
<head>
  <title>VA Enterprise | Professional Manpower & Security Services</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: #0f172a;
      color: white;
      overflow-x: hidden;
    }

    header {
      position: fixed;
      width: 100%;
      top: 0;
      background: rgba(0,0,0,0.7);
      padding: 20px 50px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      backdrop-filter: blur(10px);
      z-index: 1000;
    }

    header h1 {
      color: gold;
      letter-spacing: 2px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin-left: 25px;
      transition: 0.3s;
    }

    nav a:hover {
      color: gold;
    }

    .hero {
      height: 100vh;
      background: linear-gradient(to right, #000428, #004e92);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 20px;
      animation: fadeIn 2s ease-in-out;
    }

    .hero h2 {
      font-size: 50px;
      margin-bottom: 20px;
      animation: slideDown 1.5s ease;
    }

    .hero p {
      max-width: 600px;
      margin-bottom: 30px;
      opacity: 0.9;
    }

    .btn {
      padding: 15px 35px;
      border: none;
      border-radius: 30px;
      background: gold;
      color: black;
      font-weight: bold;
      cursor: pointer;
      transition: 0.4s;
    }

    .btn:hover {
      transform: scale(1.1);
      background: orange;
    }

    section {
      padding: 100px 20px;
      text-align: center;
    }

    .services {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
      margin-top: 50px;
    }

    .card {
      background: #1e293b;
      padding: 30px;
      width: 300px;
      border-radius: 15px;
      transition: 0.4s;
      box-shadow: 0 0 20px rgba(255,215,0,0.2);
      opacity: 0;
      transform: translateY(50px);
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 0 30px gold;
    }

    footer {
      background: black;
      padding: 30px;
      text-align: center;
      color: gray;
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }

    @keyframes slideDown {
      from {transform: translateY(-50px); opacity: 0;}
      to {transform: translateY(0); opacity: 1;}
    }
  </style>
</head>

<body>

<header>
  <h1>VA ENTERPRISE</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#contact">Contact</a>
  </nav>
</header>

<div class="hero">
  <h2>Professional Manpower & Security Solutions</h2>
  <p>VA Enterprise provides highly trained security guards and professional manpower services to ensure safety, reliability, and excellence.</p>
  <button class="btn" onclick="showMessage()">Request Service</button>
</div>

<section id="about">
  <h2>About VA Enterprise</h2>
  <p style="max-width:700px;margin:20px auto;">
    We are committed to delivering trusted manpower and top-tier security services for corporate offices, residential societies, industries, and events.
  </p>
</section>

<section id="services">
  <h2>Our Services</h2>

  <div class="services">
    <div class="card">
      <h3>Security Guards</h3>
      <p>Highly trained and disciplined guards ensuring complete protection.</p>
    </div>

    <div class="card">
      <h3>Corporate Manpower</h3>
      <p>Professional staff solutions tailored to business needs.</p>
    </div>

    <div class="card">
      <h3>Event Security</h3>
      <p>Reliable event management security with full monitoring.</p>
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
  function showMessage() {
    alert("Thank you for choosing VA Enterprise. Our team will contact you soon.");
  }

  // Scroll animation
  window.addEventListener("scroll", function() {
    const cards = document.querySelectorAll(".card");
    cards.forEach(card => {
      const position = card.getBoundingClientRect().top;
      const screenHeight = window.innerHeight;
      if(position < screenHeight - 100){
        card.style.opacity = "1";
        card.style.transform = "translateY(0)";
        card.style.transition = "1s";
      }
    });
  });
</script>

</body>
</html>
