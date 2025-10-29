<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Advocate Sapana Nalegavkar | Pune Session Court</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@700&family=Roboto:wght@400;300&display=swap" rel="stylesheet">
  <style>
    /* Reset and fonts */
    body, h1, h2, h3, h4, ul, p {margin:0; padding:0;}
    body {font-family:'Roboto', Arial, sans-serif; background: #f5f7fa; color: #222;}
    a {text-decoration: none; color: inherit;}
    ul {list-style: none;}
    /* Navbar */
    nav {
      position: sticky; top: 0; left: 0; z-index: 1000;
      background: rgba(34,87,126,0.98);
      display: flex; justify-content: center; align-items: center;
      box-shadow: 0 2px 8px #0002;
    }
    nav ul {display: flex;}
    nav li {margin: 0 22px;}
    nav a {
      font-family: 'Montserrat', Arial, sans-serif;
      color: #FFD700; font-weight: 700; font-size: 1.08em;
      padding: 16px 0; display: block;
      transition: color 0.2s;
    }
    nav a:hover {color: #fff;}
    /* Hero section */
    .hero {
      min-height: 62vh;
      background: linear-gradient(110deg, rgba(34,87,126,.8) 60%, rgba(255,215,0,.7)), url('https://images.unsplash.com/photo-1506744038136-46273834b3fb?auto=format&fit=crop&w=1200&q=80') center/cover no-repeat;
      color: #fff; display: flex; flex-direction: column; align-items: center; justify-content: center;
      text-align: center; position: relative;
    }
    .hero-logo {
      width: 120px; border-radius: 60px; border: 5px solid #FFD700; margin-bottom: 20px; box-shadow: 0 4px 25px #0002;
    }
    .hero h1 {font-family:'Montserrat',Arial,sans-serif;font-size:2.7em;margin-bottom:6px;}
    .hero .tagline {font-size:1.4em;margin-bottom:18px;}
    .hero .cta-btn {
      background: #FFD700; color: #22577E; font-weight: 700; font-size: 1.12em;
      padding: 13px 40px; border-radius: 40px; box-shadow: 0 2px 8px #0002;
      transition: background 0.2s, color 0.2s;
      margin-top: 30px;
      display: inline-block;
      border: none; cursor: pointer;
    }
    .hero .cta-btn:hover {background: #ffed85; color: #1a5276;}
    /* Sections */
    section {max-width: 1100px; margin: 48px auto 0 auto; background: white; border-radius: 20px; box-shadow: 0 4px 28px #0001; padding: 54px 36px;}
    .about {display: flex; flex-wrap: wrap; gap: 42px; align-items: center;}
    .about-img {
      min-width: 240px; width: 240px; height: 240px; border-radius: 20px; object-fit: cover; box-shadow: 0 2px 12px #0002;
    }
    .about-text {flex:1;}
    .about-text h2 {font-family:'Montserrat',Arial,sans-serif;font-size:2em;}
    .about-text ul {margin-top: 12px;}
    .about-text li {margin-bottom:8px;font-size:1.08em;}
    /* Services */
    .services-title {text-align:center;}
    .services-grid {
      display: grid; grid-template-columns: repeat(auto-fit, minmax(250px,1fr)); gap: 32px; margin-top: 28px;
    }
    .service-card {
      background: linear-gradient(120deg,#eaf6fb 80%,#fff 100%);
      border-radius: 16px; box-shadow: 0 2px 10px #0001;
      padding: 32px 18px; text-align: center; transition: transform 0.18s;
      position: relative; overflow: hidden;
      animation: fadeInUp 1s;
    }
    .service-card:hover {transform:translateY(-5px) scale(1.04);}
    .service-card img {width:56px;margin-bottom:16px;}
    .service-card h3 {font-family:'Montserrat';font-size:1.28em;margin-bottom:9px;}
    @keyframes fadeInUp {from{opacity:0;transform:translateY(24px);}to{opacity:1;transform:translateY(0);}}
    /* Testimonials */
    .testimonials-title {text-align: center;}
    .testimonials-grid {
      display: grid; grid-template-columns: repeat(auto-fit,minmax(300px,1fr)); gap: 28px; margin-top: 30px;
    }
    .testimonial-card {
      background: #22577E; color: #fff; border-radius: 14px;
      padding: 32px 22px; box-shadow: 0 2px 10px #0002;
      position: relative; font-size: 1.13em; font-style: italic;
      animation: fadeInUp 1.2s;
    }
    .testimonial-card .client {margin-top:16px;font-weight:700;color:#FFD700;}
    /* Contact */
    .contact-title {text-align: center;}
    .contact-content {display: flex; flex-wrap: wrap; gap: 44px;}
    .contact-form {flex:1; min-width: 320px;}
    .contact-form input, .contact-form textarea {
      width: 100%; padding: 14px; margin-bottom:16px;
      border:1px solid #ccd; border-radius: 10px; font-size:1.08em;
      background: #f7fafd;
    }
    .contact-form button {
      background: #22577E; color: #FFD700; padding: 13px 32px;
      border:none; border-radius:10px; font-size:1.12em; cursor:pointer;
      font-family:'Montserrat';
      transition: background .2s, color .2s;
    }
    .contact-form button:hover {background:#FFD700;color:#22577E;}
    .contact-details {flex:1; min-width: 280px; font-size:1.12em;}
    .contact-details strong {display:block;margin-bottom:6px;}
    .contact-map {
      width:100%;height:180px;border-radius:10px;box-shadow:0 2px 8px #0001;margin-top:18px;
      border: 1px solid #ccd;
    }
    /* Footer */
    footer {
      background: #22577E; color: #fff; text-align: center; padding: 32px 16px; margin-top: 64px;
      border-top: 4px solid #FFD700; font-size: 1.03em;
    }
    .social-icons img {width: 30px; margin: 0 10px; vertical-align: middle; transition: transform .2s;}
    .social-icons img:hover {transform: scale(1.12);}
    /* Responsive */
    @media(max-width:900px){
      section{padding:34px 10px;}
      .about{flex-direction:column;align-items:flex-start;}
      .contact-content{flex-direction:column;}
    }
    @media(max-width:600px){
      nav ul{flex-direction:column;}
      nav li{margin:10px 0;}
      .hero{padding:32px 8px;}
      .about-img{width:100%;height:180px;}
    }
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav>
    <ul>
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#testimonials">Testimonials</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
  <!-- Hero -->
  <div class="hero" id="home">
    <img class="hero-logo" src="https://images.unsplash.com/photo-1517841905240-472988babdf9?auto=format&fit=facearea&w=256&h=256" alt="Advocate Sapana Nalegavkar Logo">
    <h1>Advocate Sapana Nalegavkar</h1>
    <div class="tagline">Justice. Integrity. Excellence.<br>LLB, LLM | Pune Session Court</div>
    <a href="#contact" class="cta-btn">Request Consultation</a>
  </div>
  <!-- About Section -->
  <section id="about">
    <div class="about">
      <img class="about-img" src="https://images.unsplash.com/photo-1523292562811-5c5b8c1a8f5c?auto=format&fit=crop&w=400&q=80" alt="Professional Image">
      <div class="about-text">
        <h2>About Advocate Sapana Nalegavkar</h2>
        <p>Advocate Sapana Nalegavkar is a leading legal professional in Pune, specializing in civil, criminal, family, corporate, and property law. With a reputation for integrity and client-first advocacy, Sapana combines deep expertise, modern legal strategies, and personal attention to deliver exceptional results.</p>
        <ul>
          <li>LLB, LLM – Premier Indian Universities</li>
          <li>Practice at Pune Session Court</li>
          <li>Member, Maharashtra Bar Council</li>
          <li>Fluent in Marathi, Hindi, and English</li>
        </ul>
      </div>
    </div>
  </section>
  <!-- Services Section -->
  <section id="services">
    <h2 class="services-title">Legal Services</h2>
    <div class="services-grid">
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/2936/2936901.png" alt="Civil Litigation">
        <h3>Civil Litigation</h3>
        <p>Expert representation in civil disputes, contracts, torts, and property matters. Solutions tailored for individuals and businesses.</p>
      </div>
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/1041/1041916.png" alt="Criminal Defense">
        <h3>Criminal Defense</h3>
        <p>Strong defense in criminal cases, ensuring rights are protected with strategic, compassionate advocacy.</p>
      </div>
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/1077/1077012.png" alt="Family Law">
        <h3>Family Law</h3>
        <p>Support for divorce, custody, and alimony matters, delivered with empathy and results-driven focus.</p>
      </div>
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/1828/1828884.png" alt="Property Disputes">
        <h3>Property Disputes</h3>
        <p>Resolving land and title conflicts and documentation for smooth, transparent transactions.</p>
      </div>
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/3135/3135715.png" alt="Corporate Law">
        <h3>Corporate Law</h3>
        <p>Guidance for business formation, contracts, compliance, and dispute resolution for startups and established firms.</p>
      </div>
      <div class="service-card">
        <img src="https://cdn-icons-png.flaticon.com/512/1157/1157002.png" alt="Consultations">
        <h3>Consultations & Advice</h3>
        <p>Personalized legal advice to help you make informed decisions and protect your interests.</p>
      </div>
    </div>
  </section>
  <!-- Testimonials Section -->
  <section id="testimonials">
    <h2 class="testimonials-title">What Clients Say</h2>
    <div class="testimonials-grid">
      <div class="testimonial-card">
        "Sapana Nalegavkar is exceptionally skilled and truly cares about her clients' success."
        <div class="client">– Rajesh P.</div>
      </div>
      <div class="testimonial-card">
        "Professional, reliable, and trustworthy. Helped me navigate a complex property dispute with confidence."
        <div class="client">– Priya S.</div>
      </div>
      <div class="testimonial-card">
        "Highly recommend for family law matters. Sapana's approach is both compassionate and effective."
        <div class="client">– Amit D.</div>
      </div>
      <div class="testimonial-card">
        "Her expertise in corporate law was crucial for our startup’s success!"
        <div class="client">– Kiran M.</div>
      </div>
    </div>
  </section>
  <!-- Contact Section -->
  <section id="contact">
    <h2 class="contact-title">Contact Advocate Sapana Nalegavkar</h2>
    <div class="contact-content">
      <form class="contact-form" action="mailto:sapana.nalegavkar@example.com" method="POST" enctype="text/plain">
        <input type="text" name="name" placeholder="Your Name" required>
        <input type="email" name="email" placeholder="Your Email" required>
        <textarea name="message" rows="4" placeholder="Your Message" required></textarea>
        <button type="submit">Send Message</button>
      </form>
      <div class="contact-details">
        <strong>Office Address:</strong> Pune Session Court, Pune, Maharashtra<br>
        <strong>Email:</strong> sapana.nalegavkar@example.com<br>
        <strong>Phone:</strong> +91-XXXXXXXXXX<br>
        <strong>Hours:</strong> Mon–Sat, 9:30am–6:00pm
        <div class="contact-map">
          <iframe src="https://www.openstreetmap.org/export/embed.html?bbox=73.850%2C18.520%2C73.870%2C18.540&amp;layer=mapnik" style="border:0;width:100%;height:100%;" allowfullscreen="" loading="lazy"></iframe>
        </div>
      </div>
    </div>
  </section>
  <!-- Footer -->
  <footer>
    <div class="social-icons">
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/174/174857.png" alt="Facebook"></a>
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/174/174855.png" alt="Instagram"></a>
      <a href="#"><img src="https://cdn-icons-png.flaticon.com/512/174/174876.png" alt="LinkedIn"></a>
    </div>
    <div style="margin-top:10px;">
      &copy; 2025 Advocate Sapana Nalegavkar | Designed for Excellence
    </div>
    <div style="font-size:0.9em;margin-top:10px;">
      Disclaimer: This website is for informational purposes only and does not constitute legal advice. For specific legal concerns, please contact directly.
    </div>
  </footer>
  <script>
    // Smooth scroll for nav links
    document.querySelectorAll('nav a').forEach(link=>{
      link.addEventListener('click',function(e){
        const href=this.getAttribute('href');
        if(href.startsWith('#')){
          e.preventDefault();
          document.querySelector(href).scrollIntoView({behavior:'smooth'});
        }
      });
    });
  </script>
</body>
</html>
