<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Gaurav Tanwar | Expert Astrology & Guidance</title>
    <style>
        /* Base Styles & Reset */
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { line-height: 1.6; color: #333; background-color: #fafafa; overflow-x: hidden; }
        a { text-decoration: none; color: inherit; }
        
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
            z-index: 1000; 
            box-shadow: 0 2px 10px rgba(0,0,0,0.1); 
        }
        header h1 { font-size: 1.5rem; letter-spacing: 1px; color: #fbbf24; }
        
        nav ul { list-style: none; display: flex; gap: 1.5rem; }
        nav a { transition: color 0.3s ease; font-weight: 500; display: block; padding: 0.5rem; }
        nav a:hover { color: #fbbf24; }

        /* Hamburger Icon (Hidden by default) */
        .menu-toggle {
            display: none;
            background: none;
            border: none;
            color: #fbbf24;
            font-size: 1.8rem;
            cursor: pointer;
        }

        /* Hero Section */
        .hero { 
            background: linear-gradient(rgba(26, 32, 44, 0.9), rgba(45, 55, 72, 0.9)), url('https://images.unsplash.com/photo-1532767153582-b1a0e5145009?q=80&w=1920&auto=format&fit=crop') center/cover; 
            color: white; 
            text-align: center; 
            padding: 6rem 5%; 
        }
        .hero h2 { font-size: 3rem; margin-bottom: 1rem; color: #fbbf24; line-height: 1.2; }
        .hero p { font-size: 1.2rem; max-width: 700px; margin: 0 auto 2rem auto; color: #e2e8f0; }
        .btn { 
            background-color: #fbbf24; 
            color: #1a202c; 
            padding: 1rem 2rem; 
            border: none; 
            border-radius: 5px; 
            font-weight: bold; 
            display: inline-block; 
            cursor: pointer; 
            transition: background 0.3s ease; 
            text-transform: uppercase; 
            letter-spacing: 1px; 
            width: auto;
        }
        .btn:hover { background-color: #f59e0b; }

        /* Container */
        .container { max-width: 1200px; margin: 0 auto; padding: 4rem 5%; }
        .section-title { text-align: center; font-size: 2.2rem; margin-bottom: 2.5rem; color: #1a202c; }
        .section-title::after { content: ''; display: block; width: 60px; height: 3px; background: #fbbf24; margin: 0.8rem auto 0 auto; }

        /* About Section */
        .about-text { text-align: center; max-width: 800px; margin: 0 auto; font-size: 1.1rem; color: #4a5568; }

        /* Services Grid */
        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 2rem; }
        .service-card { 
            background: #fff; 
            padding: 2rem; 
            border-radius: 8px; 
            box-shadow: 0 4px 15px rgba(0,0,0,0.05); 
            transition: transform 0.3s ease; 
            border-top: 4px solid #fbbf24; 
        }
        .service-card:hover { transform: translateY(-5px); box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .service-card h3 { margin-bottom: 1rem; color: #2d3748; font-size: 1.4rem; }
        .service-card h4 { margin: 1.5rem 0 0.5rem 0; color: #1a202c; font-size: 1.1rem; }
        .service-card ul { margin-left: 1.5rem; margin-top: 0.5rem; color: #4a5568; }

        /* Contact Form */
        .contact-container { 
            display: flex; 
            flex-wrap: wrap; 
            gap: 3rem; 
            justify-content: center; 
            background: #fff; 
            padding: 3rem; 
            border-radius: 8px; 
            box-shadow: 0 4px 15px rgba(0,0,0,0.05); 
        }
        .contact-info { flex: 1; min-width: 250px; }
        .contact-form { flex: 2; min-width: 250px; width: 100%; }
        .form-row { display: flex; flex-wrap: wrap; gap: 1.5rem; margin-bottom: 1.5rem; }
        .form-group { flex: 1; min-width: 100%; } /* Stack by default, unstack on larger screens */
        .form-group label { display: block; margin-bottom: 0.5rem; font-weight: 600; color: #2d3748; }
        .form-group input, .form-group select, .form-group textarea { 
            width: 100%; 
            padding: 1rem 0.8rem; /* Larger padding for touch targets */
            border: 1px solid #cbd5e1; 
            border-radius: 4px; 
            background: #f8fafc; 
            font-family: inherit; 
            font-size: 1rem;
        }
        .form-group textarea { resize: vertical; min-height: 120px; }
        .btn-whatsapp { 
            background-color: #25D366; 
            color: white; 
            width: 100%; 
            font-size: 1.1rem; 
            display: flex; 
            justify-content: center; 
            align-items: center; 
            gap: 0.5rem;
        }
        .btn-whatsapp:hover { background-color: #128C7E; }

        /* Footer */
        footer { background-color: #1a202c; color: #e2e8f0; text-align: center; padding: 2rem 5%; }
        
        /* ===== Mobile Responsiveness Media Queries ===== */
        
        /* Tablets and larger screens */
        @media (min-width: 600px) {
            .form-group { min-width: 200px; } /* Unstack inputs side-by-side */
        }

        /* Mobile phones */
        @media (max-width: 768px) {
            .menu-toggle { display: block; }
            
            /* Mobile Navigation Menu */
            nav ul { 
                display: none; /* Hidden initially */
                flex-direction: column; 
                position: absolute; 
                top: 100%; 
                left: 0; 
                width: 100%; 
                background-color: #1a202c; 
                padding: 1rem 0; 
                text-align: center; 
                box-shadow: 0 4px 6px rgba(0,0,0,0.1); 
            }
            nav ul.active { display: flex; } /* Shown when toggled */
            nav ul li { width: 100%; border-bottom: 1px solid #2d3748; }
            nav ul li:last-child { border-bottom: none; }
            nav a { padding: 1rem; }

            /* Typography & Padding adjustments */
            .hero { padding: 4rem 1rem; }
            .hero h2 { font-size: 2.2rem; }
            .hero p { font-size: 1rem; }
            
            .container { padding: 3rem 1rem; }
            .section-title { font-size: 1.8rem; margin-bottom: 2rem; }
            
            .contact-container { padding: 1.5rem; gap: 2rem; }
            .service-card { padding: 1.5rem; }
            
            /* Ensure form row fields stack with vertical gap on mobile */
            .form-row { gap: 1rem; margin-bottom: 1rem; }
            .form-group { margin-bottom: 0.5rem; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Gaurav Tanwar</h1>
        <button class="menu-toggle" id="mobile-menu" aria-label="Toggle Navigation">
            &#9776; <!-- Hamburger Icon -->
        </button>
        <nav>
            <ul id="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero -->
    <section id="home" class="hero">
        <h2>Architect of Destiny & Logical Guide</h2>
        <p>Providing precise life readings, Kundli analysis, and actionable remedies. Align your karmic paths and navigate career, love, and life transitions with absolute clarity.</p>
        <a href="#contact" class="btn">Book Consultation</a>
    </section>

    <!-- About -->
    <section id="about" class="container">
        <h2 class="section-title">Professional Astrologer & Analyst</h2>
        <div class="about-text">
            <p>Welcome to Divine Insights. I am Gaurav Tanwar, based out of Jaipur and Ajmer. I specialize in deep-dive Janam Kundli analysis, utilizing ancient astrological principles combined with sharp, logical problem-solving.</p>
            <br>
            <p>Whether you are seeking exact timing for marriage, looking to understand career trends, or require specialized remedies to overcome life's obstacles, my approach bridges traditional wisdom with practical, modern clarity.</p>
        </div>
    </section>

    <!-- Services -->
    <section id="services" style="background-color: #f1f5f9;">
        <div class="container">
            <h2 class="section-title">My Services</h2>
            <div class="services-grid">
                
                <div class="service-card">
                    <h3>Vedic Astrology (Janam Kundli)</h3>
                    <p>Jyotish is the profound tool for understanding the karmic patterns that shape your life. By analyzing the precise planetary positions at your birth, we decode your destiny.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Karmic Alignment:</strong> Align your actions with planetary strengths.</li>
                        <li><strong>Dosha Solutions:</strong> Identify and remedy afflictions like Mangal Dosha or Sade Sati.</li>
                    </ul>
                </div>

                <div class="service-card">
                    <h3>Job & Career Consultation</h3>
                    <p>Your professional success is heavily influenced by your chart. We focus on aligning your work with your planetary strengths to identify your exact "Golden Period".</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Career Trends:</strong> Know exactly when to push for a promotion or shift paths.</li>
                        <li><strong>Business Suitability:</strong> Determine your path between job security and entrepreneurship.</li>
                    </ul>
                </div>

                <div class="service-card">
                    <h3>Love Affair & Marriage Timing</h3>
                    <p>Relationships are complex karmic bonds. We analyze the compatibility and future of your partnership to help you choose the right path for your heart.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Marriage Timing:</strong> Detailed timeline predictions for settling down.</li>
                        <li><strong>Compatibility Check:</strong> Analysis of how two charts interact (Gun Milan).</li>
                    </ul>
                </div>

                <div class="service-card">
                    <h3>Technical & Software Solutions</h3>
                    <p>In addition to spiritual guidance, I offer technical consulting. Leveraging a background in Salesforce, Apex, and LWC development to streamline your professional systems.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Structured Logic:</strong> Bringing development principles into problem-solving.</li>
                        <li><strong>Workflow Optimization:</strong> Tech-driven efficiency for your business.</li>
                    </ul>
                </div>

            </div>
        </div>
    </section>

    <!-- Contact Form (WhatsApp Integration) -->
    <section id="contact" class="container">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-container">
            <div class="contact-info">
                <h3 style="margin-bottom: 1rem; color: #1a202c;">Contact Details</h3>
                <p><strong>Name:</strong> Gaurav Tanwar</p>
                <p><strong>Locations:</strong> Jaipur & Ajmer, Rajasthan</p>
                <p style="margin-top: 1rem; color: #4a5568;">Fill out the form to reach me directly via WhatsApp for a quick response regarding your consultation or analysis requirements.</p>
            </div>
            
            <form class="contact-form" id="whatsappForm">
                <div class="form-row">
                    <div class="form-group">
                        <label for="name">Name *</label>
                        <input type="text" id="name" required placeholder="Your full name">
                    </div>
                    <div class="form-group">
                        <label for="phone">Phone *</label>
                        <input type="tel" id="phone" required placeholder="Your contact number">
                    </div>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" placeholder="Your email (optional)">
                    </div>
                    <div class="form-group">
                        <label for="age">Age</label>
                        <select id="age">
                            <option value="">Select Age</option>
                        </select>
                    </div>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label for="city">City</label>
                        <input type="text" id="city" placeholder="Your current city">
                    </div>
                </div>

                <div class="form-group" style="margin-bottom: 1.5rem;">
                    <label for="concern">Concern / Required Service *</label>
                    <textarea id="concern" required placeholder="e.g., Kundli Analysis, Career Trends, Marriage Timing..."></textarea>
                </div>

                <button type="submit" class="btn btn-whatsapp">
                    <!-- WhatsApp SVG Icon -->
                    <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" viewBox="0 0 16 16">
                        <path d="M13.601 2.326A7.85 7.85 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.9 7.9 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.9 7.9 0 0 0 13.6 2.326zM7.994 14.521a6.6 6.6 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.56 6.56 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592m3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.73.73 0 0 0-.529.247c-.182.198-.691.677-.691 1.654s.71 1.916.81 2.049c.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232z"/>
                    </svg>
                    SEND VIA WHATSAPP
                </button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Gaurav Tanwar | Terms & Conditions | Disclaimer</p>
    </footer>

    <!-- Scripts -->
    <script>
        // 1. Mobile Menu Toggle Logic
        const mobileMenu = document.getElementById('mobile-menu');
        const navLinks = document.getElementById('nav-links');
        const navItems = navLinks.querySelectorAll('a');

        mobileMenu.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });

        // Close mobile menu when a link is clicked
        navItems.forEach(item => {
            item.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });

        // 2. Populate Age Dropdown (15-99)
        const ageSelect = document.getElementById('age');
        for (let i = 15; i <= 99; i++) {
            let option = document.createElement('option');
            option.value = i;
            option.text = i;
            ageSelect.appendChild(option);
        }

        // 3. WhatsApp Submission Logic
        document.getElementById('whatsappForm').addEventListener('submit', function(e) {
            e.preventDefault();

            // *** IMPORTANT: REPLACE WITH YOUR ACTUAL WHATSAPP NUMBER ***
            // Format: Country code followed by the number without spaces or + signs.
            // Example for India: '919876543210'
            const myWhatsAppNumber = '910000000000'; 

            // Gather field values
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            const email = document.getElementById('email').value || 'Not provided';
            const age = document.getElementById('age').value || 'Not provided';
            const city = document.getElementById('city').value || 'Not provided';
            const concern = document.getElementById('concern').value;

            // Format the message text
            const message = `Hello Gaurav, I would like to book a consultation.%0A%0A` +
                            `*Name:* ${name}%0A` +
                            `*Phone:* ${phone}%0A` +
                            `*Email:* ${email}%0A` +
                            `*Age:* ${age}%0A` +
                            `*City:* ${city}%0A` +
                            `*Concern:* ${concern}`;

            // Create the WhatsApp link and open it
            const whatsappURL = `https://wa.me/${myWhatsAppNumber}?text=${message}`;
            window.open(whatsappURL, '_blank');
        });
    </script>
</body>
</html>
