<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>NextGen Engineering & Infra Solutions</title>
<style>
/* Reset & Base */
* {margin:0; padding:0; box-sizing:border-box;}
body {font-family: 'Segoe UI', sans-serif; line-height:1.6; color:#333;}
a {text-decoration:none; color:inherit;}
ul {list-style:none;}

/* Header */
header {position:fixed; top:0; width:100%; background:#fff; box-shadow:0 2px 5px rgba(0,0,0,0.1); z-index:1000;}
header .container {display:flex; justify-content:space-between; align-items:center; padding:15px 40px;}
header .logo {font-size:1.6rem; font-weight:700;}
header .logo .blue {color:#0078d4;}
nav a {margin-left:20px; font-weight:500; color:#333;}
nav a:hover {color:#0078d4;}

/* Hero Section */
.hero {height:100vh; background:url('https://images.unsplash.com/photo-1581091215367-59ab6b22e1e8?auto=format&fit=crop&w=1600&q=80') center/cover no-repeat; display:flex; align-items:center; justify-content:center; text-align:center; color:#fff; position:relative;}
.hero::after {content:''; position:absolute; inset:0; background:rgba(0,0,0,0.5);}
.hero-content {position:relative; z-index:2; max-width:800px;}
.hero h1 {font-size:3rem; margin-bottom:20px;}
.hero p {font-size:1.2rem; margin-bottom:30px;}
.btn {background:#0078d4; color:#fff; padding:12px 25px; border:none; border-radius:5px; font-weight:600; cursor:pointer;}
.btn:hover {background:#005ea6;}

/* Sections */
section {padding:80px 20px; max-width:1000px; margin:auto;}
section h2 {font-size:2rem; color:#0078d4; margin-bottom:20px; text-align:center;}
section p, section li {margin-bottom:15px;}
.services, .testimonials, .projects {display:grid; grid-gap:20px;}
.services {grid-template-columns:repeat(auto-fit, minmax(250px,1fr));}
.projects {grid-template-columns:repeat(auto-fit, minmax(280px,1fr));}
.projects img {width:100%; border-radius:8px; transition: transform 0.3s;}
.projects img:hover {transform: scale(1.05);}
.testimonial {background:#f5f5f5; padding:20px; border-left:4px solid #0078d4; border-radius:5px;}

/* Contact Form */
form {display:flex; flex-direction:column; max-width:500px; margin:auto;}
form input, form textarea {padding:10px; margin-bottom:15px; border:1px solid #ccc; border-radius:5px;}
form button {width:fit-content; align-self:center;}

/* Footer */
footer {text-align:center; padding:20px; background:#f9f9f9; font-size:14px; margin-top:40px;}

/* Smooth scroll */
html {scroll-behavior:smooth;}

/* Responsive */
@media(max-width:768px){header .container {flex-direction:column;} nav a {margin:10px 5px; display:inline-block;} .hero h1{font-size:2rem;}}
</style>
</head>
<body>

<!-- Header -->
<header>
  <div class="container">
    <div class="logo"><span class="blue">NextGen</span> Engineering & Infra Solutions</div>
    <nav>
      <a href="#home">Home</a>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#projects">Projects</a>
      <a href="#testimonials">Testimonials</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<!-- Hero -->
<section class="hero" id="home">
  <div class="hero-content">
    <h1>Building the Next Generation of Infrastructure</h1>
    <p>Reliable. Professional. On-Time.</p>
    <a href="#contact" class="btn">Request a Quote</a>
  </div>
</section>

<!-- About -->
<section id="about">
  <h2>About Us</h2>
  <p>NextGen Engineering & Infra Solutions is a Bangalore-based firm specializing in high-quality infrastructure development. We handle electrical, plumbing, fabrication, erection, civil construction, and maintenance projects with unmatched professionalism.</p>
  <p><strong>Mission:</strong> Deliver top-class engineering services with safety, precision, and on-time completion.</p>
  <p><strong>Vision:</strong> Build the next generation of reliable, sustainable, and innovative infrastructure.</p>
</section>

<!-- Services -->
<section id="services">
  <h2>Our Services</h2>
  <div class="services">
    <div>
      <h3>Electrical & Plumbing</h3>
      <p>Expert electrical and plumbing installations for commercial and residential projects.</p>
    </div>
    <div>
      <h3>Fabrication & Erection Works</h3>
      <p>High-precision steel and metal fabrication with on-site erection services.</p>
    </div>
    <div>
      <h3>Civil Construction</h3>
      <p>End-to-end civil contracting with quality materials and skilled workforce.</p>
    </div>
    <div>
      <h3>Maintenance & Repair</h3>
      <p>Comprehensive maintenance solutions ensuring long-term performance.</p>
    </div>
  </div>
</section>

<!-- Projects -->
<section id="projects">
  <h2>Project Gallery</h2>
  <div class="projects">
    <img src="https://images.unsplash.com/photo-1505842465776-3d45f5c8eeec?auto=format&fit=crop&w=600&q=60" alt="Project 1">
    <img src="https://images.unsplash.com/photo-1599058917210-56d0b923bb35?auto=format&fit=crop&w=600&q=60" alt="Project 2">
    <img src="https://images.unsplash.com/photo-1567016545376-7c7e5c7d812f?auto=format&fit=crop&w=600&q=60" alt="Project 3">
    <img src="https://images.unsplash.com/photo-1542223616-1aee3c7b59f2?auto=format&fit=crop&w=600&q=60" alt="Project 4">
  </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
  <h2>Client Testimonials</h2>
  <div class="testimonials">
    <div class="testimonial">
      <p>“NextGen delivered our industrial fabrication project ahead of schedule with excellent quality. Highly recommended!”</p>
      <h4>— Ramesh, Site Manager</h4>
    </div>
    <div class="testimonial">
      <p>“Professional and reliable team. They handled our civil works flawlessly.”</p>
      <h4>— Anil, Contractor</h4>
    </div>
  </div>
</section>

<!-- Contact -->
<section id="contact">
  <h2>Request a Quote</h2>
  <form action="https://formsubmit.co/nextgenenggandinfrasolutions@outlook.com" method="POST">
    <input type="hidden" name="_captcha" value="false">
    <input type="hidden" name="_next" value="https://website04.github.io/nextgen-engg-infra/#contact">
    <input type="text" name="name" placeholder="Your Name" required>
    <input type="email" name="email" placeholder="Your Email" required>
    <input type="text" name="phone" placeholder="Phone Number">
    <textarea name="message" placeholder="Message / Project Details" rows="5" required></textarea>
    <button type="submit" class="btn">Send Request</button>
  </form>
  <p style="text-align:center; margin-top:20px;">📞 9986283353 / 7026117372 | 📧 nextgenenggandinfrasolutions@outlook.com | Serving all over Bangalore</p>
</section>

<!-- Footer -->
<footer>
  <p>© 2025 NextGen Engineering & Infra Solutions | All rights reserved</p>
</footer>

</body>
</html>
