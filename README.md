<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gaurav Tanwar | Professional Consulting</title>
    <style>
        /* Base Styles & Reset */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        body {
            line-height: 1.6;
            color: #333;
            background-color: #f9f9f9;
        }
        a {
            text-decoration: none;
            color: inherit;
        }
        
        /* Navigation */
        header {
            background-color: #1a202c;
            color: #fff;
            padding: 1rem 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        header h1 {
            font-size: 1.5rem;
            letter-spacing: 1px;
        }
        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }
        nav a {
            transition: color 0.3s ease;
        }
        nav a:hover {
            color: #fbbf24;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #2d3748 0%, #1a202c 100%);
            color: white;
            text-align: center;
            padding: 5rem 5%;
        }
        .hero h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: #fbbf24;
        }
        .hero p {
            font-size: 1.2rem;
            max-width: 600px;
            margin: 0 auto 2rem auto;
            color: #e2e8f0;
        }
        .btn {
            background-color: #fbbf24;
            color: #1a202c;
            padding: 0.8rem 2rem;
            border-radius: 5px;
            font-weight: bold;
            display: inline-block;
            transition: background 0.3s ease;
        }
        .btn:hover {
            background-color: #f59e0b;
        }

        /* Container for content */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 5%;
        }
        .section-title {
            text-align: center;
            font-size: 2rem;
            margin-bottom: 3rem;
            color: #1a202c;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background: #fbbf24;
            margin: 0.5rem auto 0 auto;
        }

        /* Services Grid */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .service-card {
            background: #fff;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            text-align: center;
            transition: transform 0.3s ease;
            border-top: 4px solid #fbbf24;
        }
        .service-card:hover {
            transform: translateY(-5px);
        }
        .service-card h3 {
            margin-bottom: 1rem;
            color: #2d3748;
        }

        /* About Section */
        .about-content {
            display: flex;
            flex-wrap: wrap;
            gap: 2rem;
            align-items: center;
        }
        .about-text {
            flex: 1;
            min-width: 300px;
        }
        
        /* Contact Section */
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background: #fff;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }
        .form-group {
            margin-bottom: 1.5rem;
        }
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: bold;
        }
        .form-group input, .form-group textarea {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #cbd5e1;
            border-radius: 4px;
        }
        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }

        /* Footer */
        footer {
            background-color: #1a202c;
            color: #e2e8f0;
            text-align: center;
            padding: 2rem 5%;
            margin-top: 2rem;
        }

        @media (max-width: 768px) {
            nav ul {
                display: none; /* Can be replaced with a hamburger menu later */
            }
            .hero h2 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Navigation -->
    <header>
        <h1>Gaurav Tanwar</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h2>Guidance, Development & Insights</h2>
        <p>Combining analytical precision with deep insight to help you navigate your professional and personal journey. Based in Rajasthan.</p>
        <a href="#contact" class="btn">Book a Consultation</a>
    </section>

    <!-- About Section -->
    <section id="about" class="container">
        <h2 class="section-title">About Me</h2>
        <div class="about-content">
            <div class="about-text">
                <p>Hello! I am Gaurav Tanwar, currently operating out of Jaipur and Ajmer. I offer a unique blend of analytical problem-solving and insightful guidance. Whether you are seeking technical solutions in software development or looking for clarity through detailed chart analysis, I am here to help you achieve your goals.</p>
                <br>
                <p>My approach is rooted in understanding your unique needs and delivering practical, actionable results.</p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="container" style="background-color: #f1f5f9; border-radius: 8px;">
        <h2 class="section-title">My Services</h2>
        <div class="services-grid">
            <div class="service-card">
                <h3>Consultation Service One</h3>
                <p>Personalized sessions tailored to your current life path and goals. Gain clarity on the road ahead.</p>
            </div>
            <div class="service-card">
                <h3>Technical & Analytical Solutions</h3>
                <p>Expertise in developing structured, logical frameworks and software solutions to streamline your workflow.</p>
            </div>
            <div class="service-card">
                <h3>In-Depth Analysis</h3>
                <p>Comprehensive reviews and predictive insights based on exact data points to help you make informed decisions.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="container">
        <h2 class="section-title">Get In Touch</h2>
        <form class="contact-form" action="https://formspree.io/f/YOUR_ENDPOINT_HERE" method="POST">
            <p style="text-align: center; margin-bottom: 1.5rem;">Fill out the form below to schedule a session or inquire about a project.</p>
            <div class="form-group">
                <label for="name">Name</label>
                <input type="text" id="name" name="name" required placeholder="Your full name">
            </div>
            <div class="form-group">
                <label for="email">Email</label>
                <input type="email" id="email" name="email" required placeholder="Your email address">
            </div>
            <div class="form-group">
                <label for="message">Message / Required Service</label>
                <textarea id="message" name="message" required placeholder="How can I help you?"></textarea>
            </div>
            <button type="submit" class="btn" style="width: 100%; border: none; cursor: pointer;">Send Message</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Gaurav Tanwar. All rights reserved.</p>
    </footer>

</body>
</html>
