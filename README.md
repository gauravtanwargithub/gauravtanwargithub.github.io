<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gaurav Tanwar | Expert Astrology & Guidance</title>
    <style>
        /* Base Styles & Reset */
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { line-height: 1.6; color: #333; background-color: #fafafa; }
        a { text-decoration: none; color: inherit; }
        
        /* Navigation */
        header { background-color: #1a202c; color: #fff; padding: 1rem 5%; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; z-index: 100; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        header h1 { font-size: 1.5rem; letter-spacing: 1px; color: #fbbf24; }
        nav ul { list-style: none; display: flex; gap: 1.5rem; flex-wrap: wrap; }
        nav a { transition: color 0.3s ease; font-weight: 500; }
        nav a:hover { color: #fbbf24; }

        /* Hero Section */
        .hero { background: linear-gradient(rgba(26, 32, 44, 0.9), rgba(45, 55, 72, 0.9)), url('https://images.unsplash.com/photo-1532767153582-b1a0e5145009?q=80&w=1920&auto=format&fit=crop') center/cover; color: white; text-align: center; padding: 6rem 5%; }
        .hero h2 { font-size: 3rem; margin-bottom: 1rem; color: #fbbf24; }
        .hero p { font-size: 1.2rem; max-width: 700px; margin: 0 auto 2rem auto; color: #e2e8f0; }
        .btn { background-color: #fbbf24; color: #1a202c; padding: 0.8rem 2rem; border: none; border-radius: 5px; font-weight: bold; display: inline-block; cursor: pointer; transition: background 0.3s ease; text-transform: uppercase; letter-spacing: 1px; }
        .btn:hover { background-color: #f59e0b; }

        /* Container */
        .container { max-width: 1200px; margin: 0 auto; padding: 4rem 5%; }
        .section-title { text-align: center; font-size: 2.2rem; margin-bottom: 3rem; color: #1a202c; }
        .section-title::after { content: ''; display: block; width: 60px; height: 3px; background: #fbbf24; margin: 0.8rem auto 0 auto; }

        /* About Section */
        .about-text { text-align: center; max-width: 800px; margin: 0 auto; font-size: 1.1rem; color: #4a5568; }

        /* Services Grid */
        .services-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 2rem; }
        .service-card { background: #fff; padding: 2.5rem 2rem; border-radius: 8px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); transition: transform 0.3s ease; border-top: 4px solid #fbbf24; }
        .service-card:hover { transform: translateY(-5px); box-shadow: 0 10px 25px rgba(0,0,0,0.1); }
        .service-card h3 { margin-bottom: 1rem; color: #2d3748; font-size: 1.4rem; }
        .service-card h4 { margin: 1.5rem 0 0.5rem 0; color: #1a202c; font-size: 1.1rem; }
        .service-card ul { margin-left: 1.5rem; margin-top: 0.5rem; color: #4a5568; }

        /* Contact Form */
        .contact-container { display: flex; flex-wrap: wrap; gap: 3rem; justify-content: center; background: #fff; padding: 3rem; border-radius: 8px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); }
        .contact-info { flex: 1; min-width: 300px; }
        .contact-form { flex: 2; min-width: 300px; }
        .form-row { display: flex; flex-wrap: wrap; gap: 1rem; margin-bottom: 1.5rem; }
        .form-group { flex: 1; min-width: 200px; }
        .form-group label { display: block; margin-bottom: 0.5rem; font-weight: 600; color: #2d3748; }
        .form-group input, .form-group select, .form-group textarea { width: 100%; padding: 0.8rem; border: 1px solid #cbd5e1; border-radius: 4px; background: #f8fafc; font-family: inherit; }
        .form-group textarea { resize: vertical; min-height: 120px; }
        .btn-whatsapp { background-color: #25D366; color: white; width: 100%; font-size: 1.1rem; }
        .btn-whatsapp:hover { background-color: #128C7E; }

        /* Footer */
        footer { background-color: #1a202c; color: #e2e8f0; text-align: center; padding: 2rem 5%; }
        
        @media (max-width: 768px) {
            .hero h2 { font-size: 2rem; }
            nav ul { justify-content: center; }
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <h1>Gaurav Tanwar</h1>
        <nav>
            <ul>
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
    <section id="services" class="container" style="background-color: #f1f5f9; max-width: 100%;">
        <div style="max-width: 1200px; margin: 0 auto;">
            <h2 class="section-title">My Services</h2>
            <div class="services-grid">
                
                <!-- Vedic Astrology -->
                <div class="service-card">
                    <h3>Vedic Astrology (Janam Kundli)</h3>
                    <p>Jyotish is the profound tool for understanding the karmic patterns that shape your life. By analyzing the precise planetary positions at your birth, we decode your destiny.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Karmic Alignment:</strong> Align your actions with planetary strengths.</li>
                        <li><strong>Dosha Solutions:</strong> Identify and remedy afflictions like Mangal Dosha or Sade Sati.</li>
                    </ul>
                </div>

                <!-- Job & Career -->
                <div class="service-card">
                    <h3>Job & Career Consultation</h3>
                    <p>Your professional success is heavily influenced by your chart. We focus on aligning your work with your planetary strengths to identify your exact "Golden Period".</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Career Trends:</strong> Know exactly when to push for a promotion or shift paths.</li>
                        <li><strong>Business Suitability:</strong> Determine your path between job security and entrepreneurship.</li>
                    </ul>
                </div>

                <!-- Love & Marriage -->
                <div class="service-card">
                    <h3>Love Affair & Marriage Timing</h3>
                    <p>Relationships are complex karmic bonds. We analyze the compatibility and future of your partnership to help you choose the right path for your heart.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Marriage Timing:</strong> Detailed timeline predictions for settling down.</li>
                        <li><strong>Compatibility Check:</strong> Analysis of how two charts interact (Gun Milan).</li>
                    </ul>
                </div>

                <!-- Remedies -->
                <div class="service-card">
                    <h3>Grounding Remedies</h3>
                    <p>Astrology is about providing solutions. We provide a combination of Vedic rituals, scientific logic, and modern habits powerful in their results.</p>
                    <h4>What You Gain:</h4>
                    <ul>
                        <li><strong>Mantra & Rituals:</strong> Daily habits to appease difficult planets.</li>
                        <li><strong>Practical Actions:</strong> Logical steps to mitigate challenges shown in your chart.</li>
                    </ul>
                </div>

                <!-- Technical Solutions -->
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
                <h3 style="margin-bottom: 1rem;">Contact Details</h3>
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
                            <!-- JavaScript will populate this from 15 to 99 -->
                        </select>
                    </div>
                </div>

                <div class="form-row">
                    <div class="form-group">
                        <label for="city">City</label>
                        <input type="text" id="city" placeholder="Your current city">
                    </div>
                </div>

                <div class="form-group">
                    <label for="concern">Concern / Required Service *</label>
                    <textarea id="concern" required placeholder="e.g., Kundli Analysis, Career Trends, Marriage Timing..."></textarea>
                </div>

                <button type="submit" class="btn btn-whatsapp">SEND VIA WHATSAPP</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Gaurav Tanwar | Terms & Conditions | Disclaimer</p>
    </footer>

    <!-- Scripts -->
    <script>
        // Populate Age Dropdown (15-99)
        const ageSelect = document.getElementById('age');
        for (let i = 15; i <= 99; i++) {
            let option = document.createElement('option');
            option.value = i;
            option.text = i;
            ageSelect.appendChild(option);
        }

        // WhatsApp Submission Logic
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
