<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MDs RCM Solutions - We Recover What You Deserve</title>
    <meta name="description" content="Expert medical billing and revenue cycle management services for US healthcare practices. HIPAA compliant with 5+ years experience. Free audit available.">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Open+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-blue: #0A74DA;
            --sky-blue: #64B5F6;
            --white: #FFFFFF;
            --light-gray: #F5F5F5;
            --accent-red: #E53935;
            --dark-gray: #333333;
            --medium-gray: #666666;
            --success-green: #28a745;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.6;
            color: var(--dark-gray);
            overflow-x: hidden;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 600;
        }

        /* Animated Background Elements */
        .floating-shapes {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: -1;
        }

        .shape {
            position: absolute;
            background: linear-gradient(45deg, var(--primary-blue), var(--sky-blue));
            border-radius: 50%;
            opacity: 0.1;
            animation: float 6s ease-in-out infinite;
        }

        .shape:nth-child(1) {
            width: 80px;
            height: 80px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .shape:nth-child(2) {
            width: 120px;
            height: 120px;
            top: 50%;
            right: 10%;
            animation-delay: 2s;
            background: linear-gradient(45deg, var(--accent-red), var(--sky-blue));
        }

        .shape:nth-child(3) {
            width: 60px;
            height: 60px;
            bottom: 20%;
            left: 20%;
            animation-delay: 4s;
            background: linear-gradient(45deg, var(--primary-blue), var(--accent-red));
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px) rotate(0deg); }
            50% { transform: translateY(-20px) rotate(180deg); }
        }

        /* Header */
        header {
            background: var(--white);
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            transition: all 0.3s ease;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }

        .logo {
            display: flex;
            align-items: center;
            text-decoration: none;
        }

        .logo img {
            height: 40px;
            margin-right: 10px;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark-gray);
            font-weight: 500;
            transition: color 0.3s ease;
            position: relative;
        }

        .nav-links a:hover {
            color: var(--primary-blue);
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            bottom: -5px;
            left: 0;
            background-color: var(--primary-blue);
            transition: width 0.3s ease;
        }

        .nav-links a:hover::after {
            width: 100%;
        }

        .cta-button {
            background: linear-gradient(135deg, var(--primary-blue), var(--sky-blue));
            color: var(--white);
            padding: 12px 25px;
            border: none;
            border-radius: 25px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(10, 116, 218, 0.3);
        }

        .cta-button:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(10, 116, 218, 0.4);
        }

        .accent-button {
            background: linear-gradient(135deg, var(--accent-red), #FF7043);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--primary-blue) 0%, #1e3c72 100%);
            color: var(--white);
            padding: 150px 0 100px;
            text-align: center;
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1000 100" fill="white" opacity="0.1"><polygon points="0,0 1000,100 1000,0"/></svg>');
            background-size: cover;
        }

        .hero-content {
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            animation: slideInDown 1s ease-out;
        }

        .hero .subtitle {
            font-size: 1.3rem;
            margin-bottom: 2rem;
            opacity: 0.9;
            animation: slideInUp 1s ease-out 0.3s both;
        }

        .hero-stats {
            display: flex;
            justify-content: center;
            gap: 3rem;
            margin: 3rem 0;
            animation: fadeIn 1s ease-out 0.6s both;
        }

        .stat {
            text-align: center;
        }

        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            display: block;
        }

        .stat-label {
            font-size: 0.9rem;
            opacity: 0.8;
        }

        @keyframes slideInDown {
            from { opacity: 0; transform: translateY(-50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes slideInUp {
            from { opacity: 0; transform: translateY(50px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Services Section */
        .services {
            padding: 100px 0;
            background: var(--light-gray);
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-gray);
        }

        .section-subtitle {
            text-align: center;
            font-size: 1.1rem;
            color: var(--medium-gray);
            margin-bottom: 4rem;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .service-card {
            background: var(--white);
            padding: 2.5rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.2), transparent);
            transition: left 0.5s ease;
        }

        .service-card:hover::before {
            left: 100%;
        }

        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.15);
        }

        .service-icon {
            font-size: 3rem;
            color: var(--primary-blue);
            margin-bottom: 1rem;
            background: linear-gradient(135deg, var(--primary-blue), var(--sky-blue));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }

        .service-card h3 {
            font-size: 1.4rem;
            margin-bottom: 1rem;
            color: var(--dark-gray);
        }

        .service-card p {
            color: var(--medium-gray);
            line-height: 1.6;
        }

        /* About Section */
        .about {
            padding: 100px 0;
            background: var(--white);
        }

        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }

        .about-text h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-gray);
        }

        .about-text p {
            font-size: 1.1rem;
            color: var(--medium-gray);
            margin-bottom: 1.5rem;
            line-height: 1.8;
        }

        .highlights {
            display: grid;
            grid-template-columns: repeat(2, 1fr);
            gap: 1rem;
            margin-top: 2rem;
        }

        .highlight {
            display: flex;
            align-items: center;
            padding: 1rem;
            background: var(--light-gray);
            border-radius: 10px;
            transition: all 0.3s ease;
        }

        .highlight:hover {
            background: var(--primary-blue);
            color: var(--white);
            transform: scale(1.05);
        }

        .highlight i {
            font-size: 1.5rem;
            color: var(--success-green);
            margin-right: 1rem;
        }

        .highlight:hover i {
            color: var(--white);
        }

        .about-image {
            position: relative;
        }

        .about-image img {
            width: 100%;
            border-radius: 15px;
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }

        /* Process Section */
        .process {
            padding: 100px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
        }

        .process-flow {
            margin-top: 50px;
            text-align: center;
        }

        .process-flow img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.15);
        }

        .process-steps {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .process-step {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 10px 20px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .process-step:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.15);
        }

        .step-number {
            display: inline-block;
            width: 50px;
            height: 50px;
            line-height: 50px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary-blue), var(--sky-blue));
            color: var(--white);
            font-weight: 700;
            margin-bottom: 1rem;
        }

        .process-step h3 {
            margin-bottom: 1rem;
        }

        /* HIPAA Section */
        .hipaa {
            padding: 100px 0;
            background: linear-gradient(135deg, var(--primary-blue), #1e3c72);
            color: var(--white);
            text-align: center;
        }

        .hipaa-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hipaa h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .hipaa-features {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .hipaa-feature {
            background: rgba(255,255,255,0.1);
            padding: 2rem;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            transition: all 0.3s ease;
        }

        .hipaa-feature:hover {
            background: rgba(255,255,255,0.2);
            transform: translateY(-5px);
        }

        .hipaa-feature i {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--accent-red);
        }

        /* Free Audit Section */
        .free-audit {
            padding: 100px 0;
            background: var(--light-gray);
            text-align: center;
        }

        .audit-benefits {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin: 3rem 0;
        }

        .benefit {
            background: var(--white);
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .benefit:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
        }

        .benefit i {
            font-size: 2rem;
            color: var(--success-green);
            margin-bottom: 1rem;
        }

        /* Testimonials Section */
        .testimonials {
            padding: 100px 0;
            background: var(--white);
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-top: 3rem;
        }

        .testimonial {
            background: var(--light-gray);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            position: relative;
            transition: all 0.3s ease;
        }

        .testimonial:hover {
            transform: translateY(-5px);
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .testimonial-image {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            margin: 0 auto 1rem;
            overflow: hidden;
        }

        .testimonial-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }

        .stars {
            color: #ffc107;
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        .specialty {
            font-weight: 600;
            color: var(--primary-blue);
            font-size: 1.1rem;
        }

        /* Contact Section */
        .contact {
            padding: 100px 0;
            background: var(--light-gray);
        }

        .contact-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }

        .contact-form {
            background: var(--white);
            padding: 3rem;
            border-radius: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--dark-gray);
        }

        .form-group input,
        .form-group textarea,
        .form-group select {
            width: 100%;
            padding: 1rem;
            border: 2px solid #e0e0e0;
            border-radius: 10px;
            font-size: 1rem;
            transition: all 0.3s ease;
        }

        .form-group input:focus,
        .form-group textarea:focus,
        .form-group select:focus {
            outline: none;
            border-color: var(--primary-blue);
            box-shadow: 0 0 0 3px rgba(10, 116, 218, 0.1);
        }

        .submit-btn {
            background: linear-gradient(135deg, var(--primary-blue), var(--sky-blue));
            color: var(--white);
            padding: 1rem 2rem;
            border: none;
            border-radius: 25px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            width: 100%;
        }

        .submit-btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 25px rgba(10, 116, 218, 0.3);
        }

        .contact-info {
            padding: 2rem 0;
        }

        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 2rem;
            padding: 1.5rem;
            background: var(--white);
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .contact-item:hover {
            transform: translateX(10px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .contact-item i {
            font-size: 1.5rem;
            color: var(--primary-blue);
            margin-right: 1rem;
            min-width: 40px;
        }

        /* Footer */
        footer {
            background: var(--dark-gray);
            color: var(--white);
            padding: 50px 0 30px;
            text-align: center;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h3 {
            margin-bottom: 1rem;
            color: var(--accent-red);
        }

        .footer-section a {
            color: var(--white);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .footer-section a:hover {
            color: var(--accent-red);
        }

        .footer-bottom {
            border-top: 1px solid #555;
            padding-top: 2rem;
            margin-top: 2rem;
        }

        /* Mobile Menu */
        .mobile-menu {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark-gray);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .mobile-menu {
                display: block;
            }

            .hero h1 {
                font-size: 2.5rem;
            }

            .hero-stats {
                flex-direction: column;
                gap: 1rem;
            }

            .about-content,
            .contact-content {
                grid-template-columns: 1fr;
                gap: 2rem;
            }

            .services-grid,
            .testimonials-grid {
                grid-template-columns: 1fr;
            }

            .highlights {
                grid-template-columns: 1fr;
            }
        }

        /* 3D Pulse Animation for CTAs */
        .pulse {
            animation: pulse 2s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }

        /* Smooth Scroll */
        html {
            scroll-behavior: smooth;
        }

        /* Loading Animation */
        .loading {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .loading.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Video section */
        .video-section {
            padding: 100px 0;
            background: linear-gradient(135deg, #f5f7fa 0%, #e2e6ec 100%);
            text-align: center;
        }

        .video-container {
            margin-top: 3rem;
            position: relative;
            width: 100%;
            padding-bottom: 56.25%; /* 16:9 Aspect Ratio */
            height: 0;
        }

        .video-container iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border-radius: 15px;
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
        }

        .video-text {
            max-width: 800px;
            margin: 2rem auto 0;
        }
    </style>
</head>
<body>
    <!-- Floating Background Shapes -->
    <div class="floating-shapes">
        <div class="shape"></div>
        <div class="shape"></div>
        <div class="shape"></div>
    </div>

    <!-- Header -->
    <header>
        <nav class="container">
            <a href="#" class="logo">
                <img src="5yujq0oc46.png" alt="MDs RCM Solutions Logo">
            </a>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#process">Our Process</a></li>
                <li><a href="#hipaa">HIPAA</a></li>
                <li><a href="#audit">Free Audit</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="cta-button">Get Started</a>
            <div class="mobile-menu">
                <i class="fas fa-bars"></i>
            </div>
        </nav>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="container">
            <div class="hero-content">
                <h1>We Recover What You Deserve</h1>
                <p class="subtitle">Expert medical billing and revenue cycle management for US healthcare practices since 2019</p>
                
                <div class="hero-stats">
                    <div class="stat">
                        <span class="stat-number">5+</span>
                        <span class="stat-label">Years Experience</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">98%</span>
                        <span class="stat-label">Collection Rate</span>
                    </div>
                    <div class="stat">
                        <span class="stat-number">100%</span>
                        <span class="stat-label">HIPAA Compliant</span>
                    </div>
                </div>
                
                <a href="#audit" class="cta-button pulse accent-button" style="font-size: 1.2rem; padding: 15px 35px;">
                    <i class="fas fa-chart-line"></i> Get Your FREE Audit
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services loading">
        <div class="container">
            <h2 class="section-title">Comprehensive RCM Services</h2>
            <p class="section-subtitle">Complete revenue cycle management solutions designed to maximize your practice's financial performance</p>
            
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-file-medical"></i>
                    </div>
                    <h3>Prior Authorization</h3>
                    <p>Streamlined prior authorization processes to reduce claim denials and ensure faster approvals for your patients' treatments.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-calculator"></i>
                    </div>
                    <h3>Billing & Charge Entry</h3>
                    <p>Accurate and timely charge entry with expert medical coding to maximize reimbursements and minimize errors.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-hand-holding-usd"></i>
                    </div>
                    <h3>AR Recovery</h3>
                    <p>Specialized recovery of aged accounts receivable dating back to 2023. We recover what others can't.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-times-circle"></i>
                    </div>
                    <h3>Denial Management</h3>
                    <p>Comprehensive denial analysis and resolution to recover lost revenue and prevent future denials.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-credit-card"></i>
                    </div>
                    <h3>Payment Posting & Statements</h3>
                    <p>Accurate payment posting and professional patient statements to ensure proper cash flow management.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-shield-alt"></i>
                    </div>
                    <h3>Eligibility & Benefits Verification</h3>
                    <p>Real-time insurance verification to prevent claim rejections and ensure proper coverage validation.</p>
                </div>
                
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-cogs"></i>
                    </div>
                    <h3>Insurance Portal Setup</h3>
                    <p>Complete setup and management of insurance portals to streamline your billing operations.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about loading">
        <div class="container">
            <div class="about-content">
                <div class="about-text">
                    <h2>Founded in 2019, Trusted by Practices Nationwide</h2>
                    <p>MDs RCM Solutions was established with a mission to revolutionize medical billing for healthcare practices across the United States. With over 5 years of dedicated service, we've helped hundreds of practices optimize their revenue cycles and focus on what matters most - patient care.</p>
                    <p>Our team of certified medical billing professionals understands the complexities of modern healthcare reimbursement. We combine industry expertise with cutting-edge technology to deliver results that exceed expectations.</p>
                    
                    <div class="highlights">
                        <div class="highlight">
                            <i class="fas fa-check-circle"></i>
                            <span>AAPC Certified Coders</span>
                        </div>
                        <div class="highlight">
                            <i class="fas fa-check-circle"></i>
                            <span>5+ Years Experience</span>
                        </div>
                        <div class="highlight">
                            <i class="fas fa-check-circle"></i>
                            <span>HIPAA Compliant</span>
                        </div>
                        <div class="highlight">
                            <i class="fas fa-check-circle"></i>
                            <span>US-Based Team</span>
                        </div>
                    </div>
                </div>
                
                <div class="about-image">
                    <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/ga058cbec6b79f61d07f86e8fe6435b469c5ed3650a092e09bf8ba4a67e64314d908af7c06281d312a4c25f075d03753e9f2b8580fe9873aea5890e103a3e5bea_640.jpg" alt="Medical professionals in surgery">
                </div>
            </div>
        </div>
    </section>

    <!-- Process Section -->
    <section id="process" class="process loading">
        <div class="container">
            <h2 class="section-title">Our Billing Process</h2>
            <p class="section-subtitle">A streamlined, transparent approach to optimize your revenue cycle</p>
            
            <div class="process-flow">
                <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/telehealth_billing_chart.jpg" alt="Medical Billing Process Flow">
            </div>
            
            <div class="process-steps">
                <div class="process-step">
                    <div class="step-number">1</div>
                    <h3>Patient Registration</h3>
                    <p>Accurate collection and verification of patient demographics and insurance information</p>
                </div>
                
                <div class="process-step">
                    <div class="step-number">2</div>
                    <h3>Charge Capture</h3>
                    <p>Precise documentation of services provided using appropriate CPT and ICD-10 codes</p>
                </div>
                
                <div class="process-step">
                    <div class="step-number">3</div>
                    <h3>Claim Submission</h3>
                    <p>Timely, error-free submission to insurance carriers with required documentation</p>
                </div>
                
                <div class="process-step">
                    <div class="step-number">4</div>
                    <h3>Payment Posting</h3>
                    <p>Prompt and accurate posting of payments with detailed reconciliation</p>
                </div>
                
                <div class="process-step">
                    <div class="step-number">5</div>
                    <h3>Denial Management</h3>
                    <p>Aggressive follow-up on denied claims with targeted resolution strategies</p>
                </div>
                
                <div class="process-step">
                    <div class="step-number">6</div>
                    <h3>AR Recovery</h3>
                    <p>Specialized techniques to recover aged accounts and maximize collections</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Video Section -->
    <section id="video" class="video-section loading">
        <div class="container">
            <h2 class="section-title">See How We Transform Your Revenue Cycle</h2>
            <p class="section-subtitle">Our proven approach to medical billing explained</p>
            
            <div class="video-container">
                <iframe width="560" height="315" src="https://www.youtube.com/embed/gbzYjRlg3W4" title="Medical Billing Process" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </div>
            
            <div class="video-text">
                <p>Our advanced medical billing system streamlines the entire revenue cycle, from patient registration to payment reconciliation. By implementing our proven methodology, healthcare providers can significantly reduce claim denials, accelerate reimbursements, and improve overall financial performance.</p>
            </div>
        </div>
    </section>

    <!-- HIPAA Compliance Section -->
    <section id="hipaa" class="hipaa loading">
        <div class="container">
            <div class="hipaa-content">
                <h2>Your Data Security is Our Priority</h2>
                <p>We maintain the highest standards of HIPAA compliance to protect your practice and patient information. Our security measures exceed industry requirements.</p>
                
                <div class="hipaa-features">
                    <div class="hipaa-feature">
                        <i class="fas fa-lock"></i>
                        <h3>256-bit Encryption</h3>
                        <p>Military-grade encryption protects all data transmissions</p>
                    </div>
                    
                    <div class="hipaa-feature">
                        <i class="fas fa-user-shield"></i>
                        <h3>Access Controls</h3>
                        <p>Role-based access ensures only authorized personnel handle your data</p>
                    </div>
                    
                    <div class="hipaa-feature">
                        <i class="fas fa-clipboard-check"></i>
                        <h3>Regular Audits</h3>
                        <p>Continuous monitoring and compliance audits ensure security</p>
                    </div>
                    
                    <div class="hipaa-feature">
                        <i class="fas fa-certificate"></i>
                        <h3>Certified Team</h3>
                        <p>All team members are HIPAA trained and certified</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Free Audit Section -->
    <section id="audit" class="free-audit loading">
        <div class="container">
            <h2 class="section-title">Get Your FREE Revenue Cycle Audit</h2>
            <p class="section-subtitle">Discover hidden revenue opportunities in your practice with our comprehensive analysis</p>
            
            <div class="audit-benefits">
                <div class="benefit">
                    <i class="fas fa-search-dollar"></i>
                    <h3>Revenue Analysis</h3>
                    <p>Identify missed revenue opportunities and optimization areas</p>
                </div>
                
                <div class="benefit">
                    <i class="fas fa-chart-bar"></i>
                    <h3>Performance Metrics</h3>
                    <p>Benchmark your practice against industry standards</p>
                </div>
                
                <div class="benefit">
                    <i class="fas fa-lightbulb"></i>
                    <h3>Actionable Insights</h3>
                    <p>Receive specific recommendations for immediate improvements</p>
                </div>
                
                <div class="benefit">
                    <i class="fas fa-gift"></i>
                    <h3>Completely FREE</h3>
                    <p>No obligations, no hidden fees - just valuable insights</p>
                </div>
            </div>
            
            <a href="#contact" class="cta-button pulse accent-button" style="font-size: 1.2rem; padding: 15px 35px; margin-top: 2rem; display: inline-block;">
                <i class="fas fa-download"></i> Request Your Free Audit
            </a>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="testimonials loading">
        <div class="container">
            <h2 class="section-title">Trusted by Medical Professionals</h2>
            <p class="section-subtitle">See what our clients say about our services</p>
            
            <div class="testimonials-grid">
                <div class="testimonial">
                    <div class="testimonial-image">
                        <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/dr-olga-leonardi.jpg" alt="Dr. Olga Leonardi">
                    </div>
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p>"Outstanding service and incredible results. Our revenue increased by 35% in just 6 months!"</p>
                    <div class="specialty">Podiatry Specialist</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-image">
                        <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/dr-lilly-rose.jpg" alt="Dr. Lilly Rose">
                    </div>
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p>"Professional, reliable, and results-driven. They recovered accounts we thought were impossible to collect."</p>
                    <div class="specialty">DME Facility</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-image">
                        <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/dr-steven-sherwin.jpg" alt="Dr. Steven Sherwin">
                    </div>
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p>"Finally, a billing company that understands our needs. Excellent communication and transparency."</p>
                    <div class="specialty">General Practice</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-image">
                        <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/g79d7812b313ee0d6a6e54d8d6f078926706ea779c7231d0e37e8dcb4046e53348f0d00d651c92fe6002fc0fbd9951512b6a089393c38305a67c4f113a2953073_640.jpg" alt="Internal Medicine Doctor">
                    </div>
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p>"Their expertise in denial management saved us thousands. Highly recommend their services."</p>
                    <div class="specialty">Internal Medicine</div>
                </div>
                
                <div class="testimonial">
                    <div class="testimonial-image">
                        <img src="https://public.youware.com/users-website-assets/prod/2f94db55-7303-4d13-9dd5-a0a7b542ae8a/g72da8b85b49cdc5576bc632a8872a6e79dd2383375ac34bd943a391d2afce58f5da5093f30412e8fac3fe56af0f3a94735473feda16331445ce83fd12e4b5fbf_640.jpg" alt="Orthopedics Doctor">
                    </div>
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <p>"Streamlined our entire billing process. Now we can focus on our patients instead of paperwork."</p>
                    <div class="specialty">Orthopedics</div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact loading">
        <div class="container">
            <h2 class="section-title">Let's Optimize Your Revenue Together</h2>
            <p class="section-subtitle">Ready to see real results? Contact us today for your free consultation</p>
            
            <div class="contact-content">
                <div class="contact-form">
                    <h3>Request Your Free Consultation</h3>
                    <!-- Google Form Embed -->
                    <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSdKtZ5PZ7-Vz7n6iVJXGxvmqgb2QnHSHv8WPJ89lsHtbYb0Jw/viewform?embedded=true" width="100%" height="650" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
                </div>
                
                <div class="contact-info">
                    <h3>Get in Touch</h3>
                    
                    <div class="contact-item">
                        <i class="fas fa-clock"></i>
                        <div>
                            <h4>Business Hours</h4>
                            <p>Monday - Friday: 8:00 AM - 6:00 PM EST</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-shield-alt"></i>
                        <div>
                            <h4>HIPAA Compliant</h4>
                            <p>Your data is secure and protected</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-chart-line"></i>
                        <div>
                            <h4>Free Audit</h4>
                            <p>No cost, no obligation analysis</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <i class="fas fa-handshake"></i>
                        <div>
                            <h4>Trusted Partner</h4>
                            <p>Serving practices across the United States</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h3>MDs RCM Solutions</h3>
                    <p>Expert medical billing and revenue cycle management for US healthcare practices since 2019.</p>
                </div>
                
                <div class="footer-section">
                    <h3>Services</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li><a href="#services">Prior Authorization</a></li>
                        <li><a href="#services">Billing & Charge Entry</a></li>
                        <li><a href="#services">AR Recovery</a></li>
                        <li><a href="#services">Denial Management</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>Company</h3>
                    <ul style="list-style: none; padding: 0;">
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#hipaa">HIPAA Compliance</a></li>
                        <li><a href="#audit">Free Audit</a></li>
                        <li><a href="#contact">Contact</a></li>
                    </ul>
                </div>
                
                <div class="footer-section">
                    <h3>Contact Info</h3>
                    <p>Hours: Mon-Fri 8AM-6PM EST</p>
                    <p>HIPAA Compliant | US-Based Team</p>
                </div>
            </div>
            
            <div class="footer-bottom">
                <p>&copy; 2024 MDs RCM Solutions. All rights reserved. | HIPAA Compliant | Professional Medical Billing Services</p>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Loading animations on scroll
        function isElementInViewport(el) {
            const rect = el.getBoundingClientRect();
            return (
                rect.top >= 0 &&
                rect.left >= 0 &&
                rect.bottom <= (window.innerHeight || document.documentElement.clientHeight) &&
                rect.right <= (window.innerWidth || document.documentElement.clientWidth)
            );
        }

        function handleScrollAnimations() {
            const elements = document.querySelectorAll('.loading');
            elements.forEach(el => {
                if (isElementInViewport(el)) {
                    el.classList.add('visible');
                }
            });
        }

        window.addEventListener('scroll', handleScrollAnimations);
        window.addEventListener('load', handleScrollAnimations);

        // Header scroll effect
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            if (window.scrollY > 100) {
                header.style.background = 'rgba(255, 255, 255, 0.95)';
                header.style.backdropFilter = 'blur(10px)';
            } else {
                header.style.background = 'var(--white)';
                header.style.backdropFilter = 'none';
            }
        });

        // Mobile menu toggle (if needed for future enhancement)
        document.querySelector('.mobile-menu').addEventListener('click', function() {
            const navLinks = document.querySelector('.nav-links');
            navLinks.style.display = navLinks.style.display === 'flex' ? 'none' : 'flex';
        });

        // Add intersection observer for better performance
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        document.querySelectorAll('.loading').forEach(el => {
            observer.observe(el);
        });

        // Add counter animation for hero stats
        function animateCounters() {
            const counters = document.querySelectorAll('.stat-number');
            counters.forEach(counter => {
                const target = counter.textContent;
                const isPercentage = target.includes('%');
                const isPlus = target.includes('+');
                const numericValue = parseInt(target.replace(/[^\d]/g, ''));
                
                let current = 0;
                const increment = numericValue / 50; // 50 steps
                const timer = setInterval(() => {
                    current += increment;
                    if (current >= numericValue) {
                        current = numericValue;
                        clearInterval(timer);
                    }
                    
                    let displayValue = Math.floor(current);
                    if (isPercentage) displayValue += '%';
                    if (isPlus) displayValue += '+';
                    
                    counter.textContent = displayValue;
                }, 30);
            });
        }

        // Trigger counter animation when hero section is visible
        const heroObserver = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    animateCounters();
                    heroObserver.unobserve(entry.target);
                }
            });
        });

        heroObserver.observe(document.querySelector('.hero'));
    </script>
</body>
</html>

