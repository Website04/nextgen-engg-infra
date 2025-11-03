
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
   
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 15px;
        }

        /* Header Styles */
        header {
            background: linear-gradient(135deg, #1a3a5f 0%, #2c5282 100%);
            color: white;
            padding: 20px 0;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            display: flex;
            align-items: center;
        }

        .logo-icon {
            font-size: 2.5rem;
            margin-right: 15px;
            color: #4CAF50;
        }

        .logo-text h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }

        .logo-text .nextgen {
            font-size: 2.2rem;
            font-weight: 800;
            color: #4CAF50;
            display: block;
            line-height: 1.1;
        }

        .logo-text p {
            font-size: 0.9rem;
            opacity: 0.9;
        }

        .cta-button {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 12px 25px;
            font-size: 1rem;
            font-weight: 600;
            border-radius: 4px;
            cursor: pointer;
            transition: all 0.3s ease;
        }

        .cta-button:hover {
            background-color: #3d8b40;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(26, 58, 95, 0.8), rgba(44, 82, 130, 0.8)), url('https://images.unsplash.com/photo-1541888946425-d81bb19240f5?ixlib=rb-4.0.3&auto=format&fit=crop&w=1950&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 100px 0;
            text-align: center;
        }

        .hero h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            font-weight: 700;
        }

        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            opacity: 0.9;
        }

        .hero .nextgen {
            font-size: 3.2rem;
            font-weight: 800;
            color: #4CAF50;
            display: inline-block;
        }

        /* Section Styles */
        section {
            padding: 80px 0;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 2.2rem;
            color: #1a3a5f;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            width: 70px;
            height: 3px;
            background-color: #4CAF50;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
        }

        .section-title p {
            color: #666;
            max-width: 700px;
            margin: 0 auto;
        }

        /* About Section */
        .about-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }

        .about-text {
            flex: 1;
            min-width: 300px;
        }

        .about-text h3 {
            color: #1a3a5f;
            margin-bottom: 20px;
            font-size: 1.8rem;
        }

        .about-text p {
            margin-bottom: 25px;
            color: #555;
        }

        .mission-vision {
            display: flex;
            gap: 20px;
            margin-top: 30px;
        }

        .mission, .vision {
            flex: 1;
            background-color: white;
            padding: 25px;
            border-radius: 8px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }

        .mission h4, .vision h4 {
            color: #1a3a5f;
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        .mission i, .vision i {
            color: #4CAF50;
            margin-right: 10px;
            font-size: 1.2rem;
        }

        /* Services Section */
        .services {
            background-color: #f0f4f8;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 30px;
        }

        .service-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-10px);
        }

        .service-icon {
            background-color: #1a3a5f;
            color: white;
            font-size: 2.5rem;
            padding: 25px;
            text-align: center;
        }

        .service-content {
            padding: 25px;
        }

        .service-content h3 {
            color: #1a3a5f;
            margin-bottom: 15px;
            font-size: 1.4rem;
        }

        .service-content p {
            color: #666;
        }

        /* Quote Section */
        .quote-form {
            background-color: white;
            max-width: 800px;
            margin: 0 auto;
            padding: 40px;
            border-radius: 8px;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.1);
        }

        .form-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            color: #1a3a5f;
            font-weight: 600;
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 4px;
            font-size: 1rem;
            transition: border 0.3s ease;
        }

        .form-group input:focus, .form-group textarea:focus {
            border-color: #4CAF50;
            outline: none;
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .full-width {
            grid-column: 1 / -1;
        }

        .submit-btn {
            background-color: #4CAF50;
            color: white;
            border: none;
            padding: 14px 30px;
            font-size: 1.1rem;
            font-weight: 600;
            border-radius: 4px;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            background-color: #3d8b40;
        }

        /* Footer */
        footer {
            background-color: #1a3a5f;
            color: white;
            padding: 40px 0 20px;
        }

        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
            margin-bottom: 30px;
        }

        .footer-column {
            flex: 1;
            min-width: 250px;
        }

        .footer-column h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }

        .footer-column h3::after {
            content: '';
            position: absolute;
            width: 40px;
            height: 2px;
            background-color: #4CAF50;
            bottom: 0;
            left: 0;
        }

        .footer-column p, .footer-column a {
            color: #ccc;
            margin-bottom: 10px;
            display: block;
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-column a:hover {
            color: #4CAF50;
        }

        .contact-link {
            color: #4CAF50 !important;
            font-weight: 600;
            text-decoration: none !important;
        }

        .contact-link:hover {
            text-decoration: underline !important;
        }

        .social-icons {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }

        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: all 0.3s ease;
        }

        .social-icons a:hover {
            background-color: #4CAF50;
            transform: translateY(-3px);
        }

        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #aaa;
            font-size: 0.9rem;
        }

        /* Responsive Styles */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
                gap: 20px;
            }

            .hero h2 {
                font-size: 2.2rem;
            }

            .hero .nextgen {
                font-size: 2.5rem;
            }

            .mission-vision {
                flex-direction: column;
            }

            .form-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <div class="logo-icon">
                        <i class="fas fa-hard-hat"></i>
                    </div>
                    <div class="logo-text">
                        <h1><span class="nextgen">NextGen</span> Engineering & Infra Solutions</h1>
                        <p>Reliable, Professional. On-Time.</p>
                    </div>
                </div>
                <button class="cta-button">Request a Quote</button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h2>Building the <span class="nextgen">NextGen</span> of Infrastructure</h2>
            <p>Expert engineering solutions for electrical, plumbing, fabrication, erection, civil construction, and maintenance projects.</p>
            <button class="cta-button">Our Services</button>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <div class="section-title">
                <h2>About Us</h2>
                <p><span class="nextgen">NextGen</span> Engineering & Infra Solutions is a Bangalore based firm specializing in quality infrastructure development.</p>
            </div>
            <div class="about-content">
                <div class="about-text">
                    <h3>Your Trusted Infrastructure Partner</h3>
                    <p>We handle electrical, plumbing, fabrication, erection, civil construction, and maintenance projects with unmatched expertise and dedication. Our team of skilled professionals ensures every project meets the highest standards of quality and safety.</p>
                    
                    <div class="mission-vision">
                        <div class="mission">
                            <h4><i class="fas fa-bullseye"></i> Mission</h4>
                            <p>Deliver top-class engineering services with safety, precision, and on-time completion.</p>
                        </div>
                        <div class="vision">
                            <h4><i class="fas fa-eye"></i> Vision</h4>
                            <p>Building the next-generation of reliable, sustainable, and innovative infrastructure.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Services</h2>
                <p>Comprehensive infrastructure solutions tailored to your specific needs</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <div class="service-content">
                        <h3>Electrical & Plumbing</h3>
                        <p>Expert electrical and plumbing installations for commercial and residential projects with precision and safety standards.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-industry"></i>
                    </div>
                    <div class="service-content">
                        <h3>Fabrication & Erection Works</h3>
                        <p>High precision steel and metal fabrication with on-site erection services for industrial and commercial applications.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-building"></i>
                    </div>
                    <div class="service-content">
                        <h3>Civil Construction</h3>
                        <p>End-to-end civil contracting with quality materials and skilled workforce for durable and sustainable structures.</p>
                    </div>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-tools"></i>
                    </div>
                    <div class="service-content">
                        <h3>Maintenance & Repair</h3>
                        <p>Comprehensive maintenance solutions ensuring long term performance and reliability of your infrastructure.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Quote Section -->
    <section id="quote">
        <div class="container">
            <div class="section-title">
                <h2>Request a Quote</h2>
                <p>Get in touch with us for your project requirements</p>
            </div>
            <div class="quote-form">
                <form>
                    <div class="form-grid">
                        <div class="form-group">
                            <label for="name">Your Name</label>
                            <input type="text" id="name" placeholder="Enter your full name">
                        </div>
                        <div class="form-group">
                            <label for="email">Your Email</label>
                            <input type="email" id="email" placeholder="Enter your email address">
                        </div>
                        <div class="form-group">
                            <label for="phone">Phone Number</label>
                            <input type="tel" id="phone" placeholder="Enter your phone number">
                        </div>
                        <div class="form-group full-width">
                            <label for="message">Message / Project Details</label>
                            <textarea id="message" placeholder="Describe your project requirements"></textarea>
                        </div>
                    </div>
                    <button type="submit" class="submit-btn">Submit Request</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-column">
                    <h3><span class="nextgen">NextGen</span> Engineering</h3>
                    <p>Reliable, Professional. On-Time infrastructure solutions for all your needs.</p>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-facebook-f"></i></a>
                        <a href="#"><i class="fab fa-twitter"></i></a>
                        <a href="#"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div class="footer-column">
                    <h3>Quick Links</h3>
                    <a href="#about">About Us</a>
                    <a href="#services">Our Services</a>
                    <a href="#quote">Request a Quote</a>
                </div>
                <div class="footer-column">
                    <h3>Contact Info</h3>
                    <p><i class="fas fa-map-marker-alt"></i> Bangalore, India</p>
                    <p><i class="fas fa-phone"></i> <a href="tel:+917026117372" class="contact-link">   +917026117372</a></p>
                    <p><i class="fas fa-envelope"></i> <a href="mailto:Nextgenenggandinfrasolutions@outlook.com" class="contact-link">Nextgenenggandinfrasolutions@outlook.com</a></p>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2023 <span class="nextgen">NextGen</span> Engineering & Infra Solutions. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Form submission
        document.querySelector('form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Thank you for your inquiry! We will get back to you soon.');
            this.reset();
        });

        // CTA buttons
        document.querySelectorAll('.cta-button').forEach(button => {
            button.addEventListener('click', function() {
                document.getElementById('quote').scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>