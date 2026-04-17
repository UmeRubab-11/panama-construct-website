[index.html](https://github.com/user-attachments/files/26823614/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
  <title>Panama Construct | Premium Construction & Engineering</title>
  <meta name="description" content="Leading construction company in Panama: residential, commercial, and industrial projects. Expert engineering, modern design, and reliable delivery.">
  <!-- Google Fonts + Font Awesome -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,400;14..32,500;14..32,600;14..32,700;14..32,800&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #0B1120;
      font-family: 'Inter', sans-serif;
      color: #F0F3FA;
      scroll-behavior: smooth;
    }

    .container {
      max-width: 1280px;
      margin: 0 auto;
      padding: 2rem 1.5rem;
    }

    /* Navbar */
    .navbar {
      background: #0B1120cc;
      backdrop-filter: blur(12px);
      position: sticky;
      top: 0;
      z-index: 100;
      border-bottom: 1px solid #253153;
      padding: 1rem 1.5rem;
    }
    .nav-container {
      max-width: 1280px;
      margin: 0 auto;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 1rem;
    }
    .logo {
      font-size: 1.8rem;
      font-weight: 800;
      background: linear-gradient(130deg, #F7D44A, #D4AF37);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }
    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
      flex-wrap: wrap;
    }
    .nav-links a {
      text-decoration: none;
      color: #F0F3FA;
      font-weight: 600;
      transition: 0.2s;
      font-size: 1rem;
    }
    .nav-links a:hover {
      color: #F7D44A;
    }
    .nav-buttons {
      display: flex;
      gap: 0.8rem;
    }
    .btn-nav {
      background: #F5D74220;
      border: 1px solid #E5B83C;
      padding: 0.5rem 1.2rem;
      border-radius: 40px;
      text-decoration: none;
      color: #F3CD65;
      font-weight: 600;
      transition: 0.2s;
    }
    .btn-nav:hover {
      background: #E5B83C;
      color: #0B1120;
    }

    /* Headings */
    h1 {
      font-size: 3rem;
      background: linear-gradient(130deg, #F7D44A, #D4AF37);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      line-height: 1.2;
      margin-bottom: 1rem;
    }
    h2 {
      font-size: 2rem;
      margin: 2rem 0 1rem;
      border-left: 5px solid #E5B83C;
      padding-left: 1rem;
    }
    .subhead {
      color: #B9C8FF;
      margin-bottom: 2rem;
      font-size: 1.1rem;
    }

    /* Hero Section */
    .hero {
      background: linear-gradient(135deg, #0B1120 0%, #0f172f 100%);
      position: relative;
      border-bottom: 1px solid #253153;
      padding: 3rem 0;
    }
    .hero-grid {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 2rem;
    }
    .hero-text {
      flex: 1;
    }
    .hero-image {
      flex: 1;
      border-radius: 32px;
      overflow: hidden;
      box-shadow: 0 20px 35px -10px rgba(0,0,0,0.5);
    }
    .hero-image img {
      width: 100%;
      height: auto;
      display: block;
    }
    .btn-group {
      display: flex;
      gap: 1rem;
      margin-top: 2rem;
      flex-wrap: wrap;
    }
    .btn-primary {
      background: #E5B83C;
      border: none;
      padding: 0.9rem 2rem;
      border-radius: 40px;
      font-weight: 700;
      color: #0B1120;
      cursor: pointer;
      transition: 0.2s;
      font-size: 1rem;
    }
    .btn-primary:hover {
      background: #F7D44A;
      transform: translateY(-2px);
    }
    .btn-outline {
      background: transparent;
      border: 1.5px solid #E5B83C;
      padding: 0.9rem 2rem;
      border-radius: 40px;
      font-weight: 700;
      color: #F3CD65;
      cursor: pointer;
      transition: 0.2s;
    }
    .btn-outline:hover {
      background: #E5B83C20;
      transform: translateY(-2px);
    }

    /* Cards Grid (Services / Projects) */
    .card-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
      gap: 2rem;
      margin-top: 1rem;
    }
    .service-card, .project-card {
      background: #121A2C;
      border-radius: 28px;
      overflow: hidden;
      border: 1px solid #253153;
      transition: 0.25s;
    }
    .service-card:hover, .project-card:hover {
      transform: translateY(-6px);
      box-shadow: 0 20px 30px -12px rgba(212,175,55,0.2);
      border-color: #E5B83C;
    }
    .card-img {
      width: 100%;
      height: 220px;
      object-fit: cover;
    }
    .card-content {
      padding: 1.5rem;
    }
    .card-title {
      font-size: 1.5rem;
      font-weight: 700;
      color: #F3CD65;
      margin-bottom: 0.5rem;
    }
    .card-desc {
      color: #CFDEF5;
      line-height: 1.4;
      margin: 0.5rem 0;
    }
    .tag {
      background: #1D2A44;
      display: inline-block;
      padding: 0.2rem 1rem;
      border-radius: 20px;
      font-size: 0.7rem;
      margin-bottom: 0.8rem;
      color: #F7D44A;
    }

    /* Stats Section */
    .stats {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 2rem;
      background: #0E1626;
      border-radius: 2rem;
      padding: 2rem;
      margin: 2rem 0;
      text-align: center;
    }
    .stat-item h3 {
      font-size: 2rem;
      color: #F7D44A;
    }

    /* Contact Form */
    .contact-wrapper {
      background: #121A2C;
      border-radius: 2rem;
      padding: 2rem;
      border: 1px solid #253153;
      display: flex;
      flex-wrap: wrap;
      gap: 2rem;
    }
    .contact-info {
      flex: 1;
    }
    .contact-form {
      flex: 1;
    }
    input, textarea {
      width: 100%;
      padding: 12px 16px;
      background: #0B1120;
      border: 1px solid #253153;
      border-radius: 24px;
      color: white;
      font-family: inherit;
      margin-bottom: 1rem;
    }
    input:focus, textarea:focus {
      outline: none;
      border-color: #E5B83C;
    }
    .error {
      color: #ff8a7a;
      font-size: 0.75rem;
      margin-top: -0.5rem;
      margin-bottom: 0.5rem;
    }
    .success-msg {
      background: #2b4f2b;
      padding: 0.7rem;
      border-radius: 2rem;
      text-align: center;
    }

    /* Footer */
    .footer {
      text-align: center;
      margin-top: 3rem;
      padding: 2rem;
      border-top: 1px solid #1F2A48;
    }

    /* Responsive */
    @media (max-width: 768px) {
      .nav-container { flex-direction: column; }
      .nav-links { justify-content: center; }
      h1 { font-size: 2rem; }
      h2 { font-size: 1.6rem; }
    }
  </style>
</head>
<body>

<!-- Navigation Bar (fully clickable & working) -->
<nav class="navbar">
  <div class="nav-container">
    <div class="logo"><i class="fas fa-hard-hat"></i> Panama Construct</div>
    <ul class="nav-links">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div class="nav-buttons">
      <a href="#contact" class="btn-nav"><i class="fas fa-phone-alt"></i> Get Quote</a>
    </div>
  </div>
</nav>

<!-- Hero Section -->
<section id="home" class="hero">
  <div class="container hero-grid">
    <div class="hero-text">
      <h1>Building Panama’s Future<br>With Precision & Excellence</h1>
      <div class="subhead">Over 25 years of engineering marvels — from high-rise towers to sustainable residential communities.</div>
      <div class="btn-group">
        <button class="btn-primary" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Start Your Project <i class="fas fa-arrow-right"></i></button>
        <button class="btn-outline" onclick="document.getElementById('projects').scrollIntoView({behavior:'smooth'})">View Our Work</button>
      </div>
    </div>
    <div class="hero-image">
      <img src="https://images.unsplash.com/photo-1541888946425-d81bb19240f5?w=700&auto=format" alt="Modern construction site Panama">
    </div>
  </div>
</section>

<!-- About Section -->
<section id="about">
  <div class="container">
    <h2>About Panama Construct</h2>
    <div class="subhead">Leader in infrastructure, design & project management across Central America</div>
    <div style="display: flex; flex-wrap: wrap; gap: 2rem; align-items: center;">
      <div style="flex:1; border-radius: 28px; overflow: hidden;">
        <img src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?w=600&auto=format" alt="Engineers team" style="width:100%; border-radius: 24px;">
      </div>
      <div style="flex:1">
        <p style="margin-bottom: 1rem; line-height: 1.5;">We combine Panamanian expertise with global engineering standards. Our team has delivered over 150+ projects — from the financial district of Panama City to eco-resorts in the Pearl Islands. We specialize in turnkey construction, sustainable materials, and AI-driven project monitoring.</p>
        <p style="margin-bottom: 1.5rem;"><i class="fas fa-check-circle" style="color:#F7D44A;"></i> ISO 9001:2025 certified &nbsp;|&nbsp; <i class="fas fa-trophy" style="color:#F7D44A;"></i> 35+ industry awards</p>
        <button class="btn-primary" onclick="alert('📄 Company brochure will be sent to your email. Contact us!')">Download Brochure</button>
      </div>
    </div>
  </div>
</section>

<!-- Services Section (Card Grid) -->
<section id="services">
  <div class="container">
    <h2>Our Core Services</h2>
    <div class="subhead">Comprehensive construction solutions tailored to Panama’s unique landscape</div>
    <div class="card-grid">
      <div class="service-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1581092160607-ee22731e0b6b?w=600&auto=format" alt="Engineering">
        <div class="card-content">
          <div class="tag">Expertise</div>
          <div class="card-title">Structural Engineering</div>
          <div class="card-desc">Seismic-resistant design, high-rise foundations, and advanced material testing for Panama’s growing skyline.</div>
        </div>
      </div>
      <div class="service-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1504307651254-35680f356dfd?w=600&auto=format" alt="Construction">
        <div class="card-content">
          <div class="tag">Execution</div>
          <div class="card-title">General Contracting</div>
          <div class="card-desc">Full project management from ground breaking to handover. On time, within budget, zero compromise.</div>
        </div>
      </div>
      <div class="service-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1616486338812-3badae4b4b6e?w=600&auto=format" alt="Interior">
        <div class="card-content">
          <div class="tag">Design</div>
          <div class="card-title">Interior & Architecture</div>
          <div class="card-desc">Modern luxury interiors, biophilic design, and smart home integration for residential and commercial spaces.</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Projects Section -->
<section id="projects">
  <div class="container">
    <h2>Featured Projects</h2>
    <div class="subhead">Landmarks that define modern Panama — built by our expert teams</div>
    <div class="card-grid" id="projectsGrid">
      <!-- Dynamic projects will be shown but we also use static with JS for interaction? We'll create static cards with working filter? Let's keep static but clickable details -->
      <div class="project-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1486406146926-c627a92ad1ab?w=600&auto=format" alt="Oceana Tower">
        <div class="card-content">
          <div class="card-title">Oceana Financial Tower</div>
          <div class="card-desc">45-story commercial skyscraper in Panama City with LEED Gold certification.</div>
          <button class="btn-outline" style="margin-top: 12px; padding: 0.4rem 1rem; font-size:0.8rem;" onclick="alert('Case study: Completed 2025, 220,000 sq ft of premium offices.')">View Details</button>
        </div>
      </div>
      <div class="project-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1560518883-ce09059eeffa?w=600&auto=format" alt="Residential">
        <div class="card-content">
          <div class="card-title">Costa Verde Residences</div>
          <div class="card-desc">Luxury beachfront apartments in Coronado, featuring smart home automation & sustainable energy.</div>
          <button class="btn-outline" style="margin-top: 12px; padding: 0.4rem 1rem;" onclick="alert('70 units delivered in 2024, 98% occupancy rate.')">Learn More</button>
        </div>
      </div>
      <div class="project-card">
        <img class="card-img" src="https://images.unsplash.com/photo-1497366216548-37526070297c?w=600&auto=format" alt="Logistics Hub">
        <div class="card-content">
          <div class="card-title">Colón Free Zone Logistics Hub</div>
          <div class="card-desc">Industrial warehouse with AI-driven inventory systems, boosting trade efficiency.</div>
          <button class="btn-outline" style="margin-top: 12px; padding: 0.4rem 1rem;" onclick="alert('350,000 sq ft, completed Q1 2025.')">Project Brief</button>
        </div>
      </div>
    </div>
    <div style="text-align: center; margin-top: 2rem;">
      <button class="btn-primary" onclick="alert('More projects available upon request. Contact our team.')">See All Projects <i class="fas fa-chevron-right"></i></button>
    </div>
  </div>
</section>

<!-- Stats & Trust Badges -->
<div class="container">
  <div class="stats">
    <div class="stat-item"><h3>150+</h3><p>Completed Projects</p></div>
    <div class="stat-item"><h3>12</h3><p>Years in Panama</p></div>
    <div class="stat-item"><h3>98%</h3><p>Client Satisfaction</p></div>
    <div class="stat-item"><h3>24/7</h3><p>Project Support</p></div>
  </div>
</div>

<!-- Contact Section with Validation -->
<section id="contact">
  <div class="container">
    <h2>Contact Us</h2>
    <div class="subhead">Let’s discuss your next construction project — free consultation & quote</div>
    <div class="contact-wrapper">
      <div class="contact-info">
        <i class="fas fa-map-marker-alt" style="font-size: 2rem; color: #F7D44A;"></i>
        <h3 style="margin: 0.5rem 0;">Panama Headquarters</h3>
        <p>Torre Global, 28th floor, Calle 50, Panama City</p>
        <i class="fas fa-phone-alt" style="font-size: 2rem; margin-top: 1rem; color: #F7D44A;"></i>
        <h3>Call / WhatsApp</h3>
        <p>+507 6789-1234</p>
        <i class="fas fa-envelope" style="font-size: 2rem; margin-top: 1rem; color: #F7D44A;"></i>
        <h3>Email</h3>
        <p>hello@panamaconstruct.com</p>
        <div style="margin-top: 2rem;"><i class="fab fa-facebook-f"></i> &nbsp; <i class="fab fa-instagram"></i> &nbsp; <i class="fab fa-linkedin-in"></i></div>
      </div>
      <div class="contact-form">
        <form id="contactForm">
          <input type="text" id="fullname" placeholder="Full Name *">
          <div class="error" id="nameError"></div>
          <input type="email" id="email" placeholder="Email Address *">
          <div class="error" id="emailError"></div>
          <input type="tel" id="phone" placeholder="Phone Number">
          <textarea rows="4" id="message" placeholder="Tell us about your construction project *"></textarea>
          <div class="error" id="msgError"></div>
          <button type="submit" class="btn-primary" style="width:100%;"><i class="fas fa-paper-plane"></i> Send Message</button>
          <div id="formStatus"></div>
        </form>
      </div>
    </div>
  </div>
</section>

<!-- Footer -->
<div class="footer">
  <a href="#" class="btn-nav" style="margin-bottom: 1rem; display: inline-block;">🏗️ Panama Construct © 2026</a>
  <p style="margin-top: 1rem;">Leading construction & engineering firm — building a smarter Panama.</p>
  <p><i class="fas fa-hard-hat"></i> Licensed & Insured | Member of Panamanian Chamber of Construction</p>
</div>

<script>
  // Smooth scroll for all navigation links (already using CSS scroll-behavior but ensure click override)
  document.querySelectorAll('.nav-links a, .btn-nav[href="#contact"], .hero-buttons a').forEach(anchor => {
    anchor.addEventListener('click', function(e) {
      const hash = this.getAttribute('href');
      if(hash && hash.startsWith("#")) {
        e.preventDefault();
        const targetElement = document.querySelector(hash);
        if(targetElement) {
          const offset = 80;
          const elementPosition = targetElement.getBoundingClientRect().top + window.scrollY - offset;
          window.scrollTo({ top: elementPosition, behavior: "smooth" });
        }
      }
    });
  });

  // Contact form validation
  const form = document.getElementById('contactForm');
  const nameInput = document.getElementById('fullname');
  const emailInput = document.getElementById('email');
  const messageInput = document.getElementById('message');
  const nameError = document.getElementById('nameError');
  const emailError = document.getElementById('emailError');
  const msgError = document.getElementById('msgError');
  const statusDiv = document.getElementById('formStatus');

  form.addEventListener('submit', (e) => {
    e.preventDefault();
    let isValid = true;
    nameError.innerText = '';
    emailError.innerText = '';
    msgError.innerText = '';
    statusDiv.innerHTML = '';

    const nameVal = nameInput.value.trim();
    const emailVal = emailInput.value.trim();
    const msgVal = messageInput.value.trim();

    if (nameVal === '') {
      nameError.innerText = 'Full name is required';
      isValid = false;
    }
    const emailPattern = /^[^\s@]+@([^\s@.,]+\.)+[^\s@.,]{2,}$/;
    if (emailVal === '') {
      emailError.innerText = 'Email address is required';
      isValid = false;
    } else if (!emailPattern.test(emailVal)) {
      emailError.innerText = 'Enter a valid email (e.g., name@domain.com)';
      isValid = false;
    }
    if (msgVal === '') {
      msgError.innerText = 'Please describe your project needs';
      isValid = false;
    }

    if (isValid) {
      statusDiv.innerHTML = '<div class="success-msg"><i class="fas fa-check-circle"></i> Thank you! Our team will contact you within 24 hours.</div>';
      form.reset();
      setTimeout(() => { statusDiv.innerHTML = ''; }, 5000);
    } else {
      statusDiv.innerHTML = '<div style="background:#5a1e1e; padding:0.7rem; border-radius:2rem; text-align:center;">Please fix the errors above</div>';
    }
  });

  // Additional interactive: alert for Get Quote button on navbar click (already linked to contact)
  // Make all "Get Quote" and other call-to-action buttons interactive
  const quoteBtns = document.querySelectorAll('.btn-nav, .btn-primary');
  quoteBtns.forEach(btn => {
    if(btn.getAttribute('onclick')) return;
    if(btn.innerText.includes('Get Quote') || btn.innerText.includes('Start Your Project')) {
      btn.addEventListener('click', function(e) {
        if(!btn.closest('a') && !btn.hasAttribute('onclick')) {
          const contactSec = document.getElementById('contact');
          if(contactSec) {
            const offset = 70;
            const pos = contactSec.getBoundingClientRect().top + window.scrollY - offset;
            window.scrollTo({ top: pos, behavior: 'smooth' });
          }
        }
      });
    }
  });
  // Also for home link on footer? smooth
  const footerHome = document.querySelector('.footer a');
  if(footerHome && footerHome.getAttribute('href')
