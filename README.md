<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Samwa Plus Solutions Limited | Construction & General Supply</title>
    <style>
        /* CSS RESET & GENERAL STYLES */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary: #0f4c81; /* Corporate Blue */
            --secondary: #f5b041; /* Construction Amber/Gold */
            --dark: #2c3e50;
            --light: #f8f9fa;
            --white: #ffffff;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            color: var(--dark);
            line-height: 1.6;
            background-color: var(--light);
        }

        /* HEADER & NAVIGATION */
        header {
            background-color: var(--white);
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 20px;
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            color: var(--primary);
        }

        .logo span {
            color: var(--secondary);
        }

        nav ul {
            display: flex;
            list-style: none;
        }

        nav ul li {
            margin-left: 20px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: var(--primary);
        }

        /* HERO SECTION */
        .hero {
            background: linear-gradient(rgba(15, 76, 129, 0.85), rgba(44, 62, 80, 0.9)), url('https://unsplash.com') no-repeat center center/cover;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding: 0 20px;
            margin-top: 60px;
        }

        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .hero p {
            font-size: 20px;
            max-width: 800px;
            margin-bottom: 30px;
        }

        .btn {
            background-color: var(--secondary);
            color: var(--dark);
            padding: 12px 30px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            transition: background 0.3s, color 0.3s;
        }

        .btn:hover {
            background-color: var(--white);
            color: var(--primary);
        }

        /* SECTIONS GENERAL */
        section {
            padding: 80px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            font-size: 32px;
            color: var(--primary);
            margin-bottom: 40px;
            position: relative;
        }

        .section-title::after {
            content: '';
            display: block;
            width: 60px;
            height: 3px;
            background-color: var(--secondary);
            margin: 10px auto 0;
        }

        /* ABOUT SECTION */
        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            margin-bottom: 40px;
        }

        .about-box {
            background: var(--white);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .about-box h3 {
            color: var(--primary);
            margin-bottom: 15px;
            font-size: 22px;
        }

        /* CORE VALUES */
        .values-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
            gap: 20px;
            text-align: center;
        }

        .value-card {
            background: var(--primary);
            color: var(--white);
            padding: 20px;
            border-radius: 5px;
            font-weight: bold;
            transition: transform 0.3s, background-color 0.3s, color 0.3s;
        }

        .value-card:hover {
            transform: translateY(-5px);
            background-color: var(--secondary);
            color: var(--dark);
        }

        /* SERVICES SECTION */
        .services-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-category {
            background: var(--white);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border-top: 5px solid var(--primary);
        }

        .service-category h3 {
            color: var(--primary);
            margin-bottom: 20px;
            font-size: 22px;
        }

        .service-category ul {
            list-style: none;
        }

        .service-category ul li {
            padding: 8px 0;
            border-bottom: 1px solid #eee;
            position: relative;
            padding-left: 25px;
        }

        .service-category ul li::before {
            content: "✓";
            color: var(--secondary);
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        /* CONTACT & ADDRESS */
        .contact-grid {
            display: grid;
            grid-template-columns: 1.2fr 0.8fr;
            gap: 40px;
        }

        .info-box {
            background: var(--white);
            padding: 40px;
            border-radius: 6px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.02);
        }

        .info-box h3 {
            margin-bottom: 20px;
            color: var(--primary);
            text-transform: uppercase;
            font-size: 18px;
            border-bottom: 2px solid #f3f4f6;
            padding-bottom: 10px;
        }

        .info-box p {
            margin-bottom: 15px;
            font-size: 15px;
            display: flex;
            align-items: center;
        }

        .info-box strong {
            min-width: 100px;
            display: inline-block;
        }

        .info-box a {
            color: var(--accent);
            text-decoration: none;
            font-weight: 600;
        }

        .info-box a:hover {
            text-decoration: underline;
        }

        /* FOOTER */
        footer {
            background-color: var(--dark);
            color: var(--white);
            text-align: center;
            padding: 20px;
            margin-top: 40px;
        }

        /* RESPONSIVE DESIGN */
        @media (max-width: 768px) {
            .nav-container {
                flex-direction: column;
            }
            nav ul {
                margin-top: 15px;
            }
            .about-grid, .contact-grid {
                grid-template-columns: 1fr;
            }
            .hero h1 {
                font-size: 32px;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER & NAV -->
    <header>
        <div class="nav-container">
            <div class="logo">SAMWA <span>PLUS</span></div>
            <nav>
                <ul>
                    <li><a href="#home">Home</a></li>
                    <li><a href="#about">About Us</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- HERO SECTION -->
    <section id="home" class="hero">
        <h1>SAMWA PLUS SOLUTIONS LIMITED</h1>
        <p>Leading construction and general supply solutions across East Africa. Building with quality, integrity, and innovation.</p>
        <a href="#contact" class="btn">Get in Touch</a>
    </section>

    <!-- ABOUT SECTION -->
    <section id="about">
        <h2 class="section-title">About Us</h2>
        <div class="about-grid">
            <div class="about-box">
                <h3>Our Vision</h3>
                <p>To become one of the leading construction and general supply companies in East Africa through quality, integrity, and innovation.</p>
            </div>
            <div class="about-box">
                <h3>Our Mission</h3>
                <p>To provide reliable construction and supply solutions that exceed customer expectations while maintaining the highest standards of professionalism.</p>
            </div>
        </div>

        <h3 style="text-align: center; margin-bottom: 20px; color: var(--primary);">Core Values</h3>
        <div class="values-grid">
            <div class="value-card">Integrity</div>
            <div class="value-card">Excellence</div>
            <div class="value-card">Quality</div>
            <div class="value-card">Innovation</div>
            <div class="value-card">Teamwork</div>
            <div class="value-card">Accountability</div>
        </div>
    </section>

    <!-- SERVICES SECTION -->
    <section id="services" style="background-color: #f0f4f8;">
        <h2 class="section-title">Our Services</h2>
        <div class="services-container">
            
            <!-- Category 1 -->
            <div class="service-category">
                <h3>Building Construction</h3>
                <ul>
                    <li>Residential Buildings</li>
                    <li>Commercial Buildings</li>
                    <li>Institutional Buildings</li>
                    <li>Schools</li>
                    <li>Hospitals</li>
                    <li>Warehouses</li>
                </ul>
            </div>

            <!-- Category 2 -->
            <div class="service-category">
                <h3>Civil Engineering Works</h3>
                <ul>
                    <li>Roads Construction</li>
                    <li>Drainage Systems</li>
                    <li>Water Supply Projects</li>
                    <li>Sewer Lines</li>
                    <li>Culverts</li>
                    <li>Concrete Works</li>
                </ul>

                 <!-- CONTACT SECTION -->
    <section id="contact" style="background-color: #f3f4f6;">
        <h2 class="section-title">Get In Touch</h2>
        <div class="contact-grid">
            <P>
            <!-- Office Address Box -->
            <div class="info-box">
                <h3>Official Address</h3>
                <p><strong>Company:</strong> SAMWA PLUS SOLUTIONS LIMITED</p>
                <p><strong>P.O Box:</strong> P.O BOX 11660, 00200 - CITY SQUARE</p>
                <p><strong>Location:</strong> Nairobi, Kenya</p>
                <p><strong>Phone:</strong> <a href="tel: +254796258348">+254 796 258 348</a></p>
                <p><strong>Email:</strong> <a href="mailto:samwaplus@gmail.com">samwaplus@gmail.com</a></p>
            </div>
            </div>

            <!-- Category 3 -->
