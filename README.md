<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Doris Massage | Professional Mobile Spa Services</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;500;600&family=Montserrat:wght@300;400;500;600&display=swap" rel="stylesheet">
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary: #556B2F;
            --secondary: #8F9779;
            --accent: #B5651D;
            --light: #F5F5DC;
            --dark: #4A5D23;
            --text: #333333;
            --transition: all 0.3s ease;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            line-height: 1.6;
            color: var(--text);
            background-color: var(--light);
            overflow-x: hidden;
        }
        
        h1, h2, h3, h4 {
            font-family: 'Playfair Display', serif;
            font-weight: 500;
            margin-bottom: 1rem;
            color: var(--dark);
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 1.5rem;
        }
        
        h2 {
            font-size: 2.2rem;
            text-align: center;
            margin-bottom: 2.5rem;
            position: relative;
        }
        
        h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: var(--accent);
        }
        
        p {
            margin-bottom: 1.2rem;
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: white;
            padding: 12px 28px;
            border-radius: 30px;
            font-weight: 500;
            border: none;
            cursor: pointer;
            transition: var(--transition);
            font-size: 1rem;
            text-align: center;
        }
        
        .btn:hover {
            background-color: var(--dark);
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .btn-secondary {
            background-color: var(--primary);
        }
        
        .btn-secondary:hover {
            background-color: var(--dark);
        }
        
        section {
            padding: 80px 0;
        }
        
        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 15px rgba(0, 0, 0, 0.05);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
        }
        
        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 600;
            color: var(--dark);
        }
        
        .logo span {
            color: var(--accent);
        }
        
        nav {
            display: flex;
            align-items: center;
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            font-weight: 500;
            transition: var(--transition);
            position: relative;
        }
        
        .nav-links a:hover {
            color: var(--accent);
        }
        
        .nav-links a.active {
            color: var(--accent);
        }
        
        .nav-links a.active:after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: var(--accent);
        }
        
        .menu-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark);
        }
        
        /* Hero Section */
        .hero {
            height: 90vh;
            background: linear-gradient(rgba(85, 107, 47, 0.7), rgba(85, 107, 47, 0.7)), url('https://images.unsplash.com/photo-1599901860904-17e6ed7083a0?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            display: flex;
            align-items: center;
            text-align: center;
            margin-top: 80px;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            color: white;
            font-size: 3.2rem;
            margin-bottom: 1.5rem;
        }
        
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
        }
        
        /* Features Section */
        .features {
            background-color: #f8f8f2;
        }
        
        .features-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
            margin-top: 40px;
        }
        
        .feature-card {
            text-align: center;
            padding: 30px;
            border-radius: 10px;
            transition: var(--transition);
            background-color: white;
        }
        
        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.08);
        }
        
        .feature-icon {
            font-size: 3rem;
            color: var(--accent);
            margin-bottom: 20px;
        }
        
        .feature-card h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }
        
        /* Services Section */
        .services {
            background-color: white;
        }
        
        .services-container {
            max-width: 900px;
            margin: 0 auto;
        }
        
        .service-note {
            background-color: #f8f8f2;
            padding: 25px;
            border-radius: 10px;
            margin-bottom: 40px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            border-left: 4px solid var(--accent);
        }
        
        .service-note h3 {
            color: var(--accent);
            margin-bottom: 10px;
        }
        
        .services-table {
            width: 100%;
            border-collapse: collapse;
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .services-table thead {
            background-color: var(--primary);
            color: white;
        }
        
        .services-table th {
            padding: 20px;
            text-align: left;
            font-weight: 600;
        }
        
        .services-table td {
            padding: 18px 20px;
            border-bottom: 1px solid #eee;
        }
        
        .services-table tr:last-child td {
            border-bottom: none;
        }
        
        .services-table tr:hover {
            background-color: rgba(85, 107, 47, 0.05);
        }
        
        .service-duration {
            color: var(--accent);
            font-weight: 500;
        }
        
        .service-price {
            font-weight: 600;
            color: var(--dark);
        }
        
        /* Testimonials Section */
        .testimonials {
            background-color: #f8f8f2;
        }
        
        .testimonials-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }
        
        .testimonial-card {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
        }
        
        .testimonial-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.08);
        }
        
        .testimonial-header {
            display: flex;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .testimonial-img {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            object-fit: cover;
            margin-right: 15px;
        }
        
        .testimonial-info h4 {
            margin-bottom: 5px;
        }
        
        .testimonial-info p {
            margin-bottom: 0;
            color: var(--accent);
            font-size: 0.9rem;
        }
        
        .testimonial-rating {
            color: #ffc107;
            margin-bottom: 15px;
        }
        
        /* Contact Section */
        .contact {
            background-color: white;
        }
        
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 50px;
            margin-top: 40px;
        }
        
        .contact-info h3 {
            color: var(--accent);
            margin-bottom: 20px;
        }
        
        .contact-detail {
            display: flex;
            align-items: center;
            margin-bottom: 25px;
        }
        
        .contact-icon {
            background-color: var(--accent);
            color: white;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            font-size: 1.2rem;
        }
        
        .contact-form {
            background-color: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-family: 'Montserrat', sans-serif;
            transition: var(--transition);
        }
        
        .form-control:focus {
            outline: none;
            border-color: var(--accent);
        }
        
        textarea.form-control {
            min-height: 150px;
            resize: vertical;
        }
        
        /* Booking Section */
        .booking {
            background-color: white;
        }
        
        .booking-container {
            max-width: 800px;
            margin: 0 auto;
            background-color: #f8f8f2;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.08);
        }
        
        .booking-steps {
            display: flex;
            justify-content: space-between;
            margin-bottom: 40px;
            position: relative;
        }
        
        .booking-steps:before {
            content: '';
            position: absolute;
            top: 20px;
            left: 0;
            right: 0;
            height: 2px;
            background-color: #ddd;
            z-index: 1;
        }
        
        .step {
            text-align: center;
            position: relative;
            z-index: 2;
            background-color: #f8f8f2;
            padding: 0 15px;
        }
        
        .step-number {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: #ddd;
            color: var(--dark);
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 10px;
            font-weight: 600;
            transition: var(--transition);
        }
        
        .step.active .step-number {
            background-color: var(--accent);
            color: white;
        }
        
        .step p {
            font-size: 0.9rem;
            margin-bottom: 0;
        }
        
        .booking-form-section {
            display: none;
        }
        
        .booking-form-section.active {
            display: block;
        }
        
        .service-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .service-option {
            background-color: white;
            padding: 25px;
            border-radius: 10px;
            cursor: pointer;
            transition: var(--transition);
            border: 2px solid transparent;
            text-align: center;
        }
        
        .service-option:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.08);
        }
        
        .service-option.selected {
            border-color: var(--accent);
            background-color: rgba(181, 101, 29, 0.05);
        }
        
        .service-option h4 {
            margin-bottom: 10px;
        }
        
        .service-option .price {
            font-size: 1.5rem;
            color: var(--accent);
            font-weight: 600;
            margin-bottom: 5px;
        }
        
        .service-option .duration {
            color: var(--primary);
            font-size: 0.9rem;
        }
        
        .payment-notice {
            background-color: rgba(85, 107, 47, 0.1);
            padding: 25px;
            border-radius: 10px;
            margin-top: 30px;
            border-left: 4px solid var(--primary);
        }
        
        .payment-notice h4 {
            color: var(--primary);
            margin-bottom: 10px;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            margin-bottom: 20px;
        }
        
        .footer-links h4, .footer-contact h4 {
            margin-bottom: 20px;
            font-size: 1.2rem;
            color: var(--secondary);
        }
        
        .footer-links ul {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            color: var(--secondary);
            padding-left: 5px;
        }
        
        .footer-contact p {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }
        
        .footer-contact i {
            margin-right: 10px;
            color: var(--secondary);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
            color: rgba(255, 255, 255, 0.7);
        }
        
        /* Responsive Design */
        @media (max-width: 992px) {
            h1 {
                font-size: 2.4rem;
            }
            
            h2 {
                font-size: 1.9rem;
            }
            
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .booking-steps {
                flex-direction: column;
                align-items: center;
                gap: 30px;
            }
            
            .booking-steps:before {
                display: none;
            }
        }
        
        @media (max-width: 768px) {
            .menu-toggle {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 80px;
                left: 0;
                background-color: white;
                width: 100%;
                flex-direction: column;
                align-items: center;
                padding: 20px 0;
                box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
                transform: translateY(-100%);
                opacity: 0;
                visibility: hidden;
                transition: var(--transition);
                z-index: 999;
            }
            
            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
                visibility: visible;
            }
            
            .nav-links li {
                margin: 15px 0;
            }
            
            .hero {
                height: 80vh;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .hero p {
                font-size: 1rem;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.7rem;
            }
            
            section {
                padding: 60px 0;
            }
            
            .booking-container {
                padding: 30px 20px;
            }
            
            .service-options {
                grid-template-columns: 1fr;
            }
        }
        
        @media (max-width: 576px) {
            .hero h1 {
                font-size: 1.9rem;
            }
            
            .btn {
                padding: 10px 22px;
            }
            
            .services-table {
                display: block;
                overflow-x: auto;
            }
            
            .contact-form {
                padding: 30px 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Doris<span>Massage</span></a>
            
            <div class="menu-toggle" id="menuToggle">
                <i class="fas fa-bars"></i>
            </div>
            
            <nav>
                <ul class="nav-links" id="navLinks">
                    <li><a href="#home" class="nav-link active">Home</a></li>
                    <li><a href="#services" class="nav-link">Services & Pricing</a></li>
                    <li><a href="#testimonials" class="nav-link">Testimonials</a></li>
                    <li><a href="#contact" class="nav-link">Contact</a></li>
                    <li><a href="#booking" class="nav-link btn">Book Now</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Main Content Area -->
    <main id="mainContent">
        <!-- Home Page Content - Loaded by default -->
        <section id="homeSection" class="page-section">
            <section class="hero">
                <div class="container hero-content">
                    <h1>Luxury Spa Services Delivered to Your Door</h1>
                    <p>Experience ultimate relaxation with our professional mobile massage and spa treatments. We bring the spa experience to your home, hotel, or office with everything needed for your complete rejuvenation.</p>
                    <a href="#booking" class="btn">Book Your Session</a>
                    <a href="#services" class="btn btn-secondary">View Services</a>
                </div>
            </section>
            
            <section class="features">
                <div class="container">
                    <h2>Why Choose Our Mobile Spa</h2>
                    <div class="features-container">
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1544161515-4ab6ce6db874?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80" alt="Therapist arriving at a home" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <div class="feature-icon">
                                <i class="fas fa-home"></i>
                            </div>
                            <h3>Convenience</h3>
                            <p>Enjoy premium spa services without leaving your home. We set up everything needed for your treatment in your preferred space.</p>
                        </div>
                        
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1562322140-8baeececf3df?ixlib=rb-4.0.3&auto=format&fit=crop&w=1469&q=80" alt="Professional massage setup in a home" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <div class="feature-icon">
                                <i class="fas fa-user-shield"></i>
                            </div>
                            <h3>Professional & Licensed</h3>
                            <p>Our therapists are fully licensed, insured, and trained in a variety of massage techniques to address your specific needs.</p>
                        </div>
                        
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1591348278863-32811c5d43df?ixlib=rb-4.0.3&auto=format&fit=crop&w=1470&q=80" alt="Massage oils and equipment" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <div class="feature-icon">
                                <i class="fas fa-spa"></i>
                            </div>
                            <h3>Fully Equipped</h3>
                            <p>We bring all necessary equipment: massage table, premium oils, towels, music, and ambiance elements for a complete spa experience.</p>
                        </div>
                    </div>
                </div>
            </section>
            
            <section class="services">
                <div class="container">
                    <h2>Popular Services</h2>
                    <div class="features-container">
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1591343395082-e120087004b4?ixlib=rb-4.0.3&auto=format&fit=crop&w=687&q=80" alt="Full Body Massage" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <h3>Full Body Massage</h3>
                            <p>50 minutes of complete relaxation targeting all major muscle groups for stress relief and improved circulation.</p>
                            <div style="margin-top:15px; color:var(--accent); font-weight:600;">$100</div>
                            <a href="#booking" class="btn" style="margin-top:15px; padding:8px 20px; font-size:0.9rem;">Book Now</a>
                        </div>
                        
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1600334129128-685c5582fd35?ixlib=rb-4.0.3&auto=format&fit=crop&w=1170&q=80" alt="Hot Stone Massage" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <h3>Hot Stone Massage</h3>
                            <p>Warm stones are used to release deep muscle tension, promote relaxation, and improve energy flow throughout the body.</p>
                            <div style="margin-top:15px; color:var(--accent); font-weight:600;">$150</div>
                            <a href="#booking" class="btn" style="margin-top:15px; padding:8px 20px; font-size:0.9rem;">Book Now</a>
                        </div>
                        
                        <div class="feature-card">
                            <img src="https://images.unsplash.com/photo-1600334089648-c6728c87e7a9?ixlib=rb-4.0.3&auto=format&fit=crop&w=1170&q=80" alt="Foot Massage" style="width:100%; height:200px; object-fit:cover; border-radius:8px; margin-bottom:20px;">
                            <h3>Foot Scrub & Massage</h3>
                            <p>Exfoliating foot scrub followed by a relaxing foot and lower leg massage to rejuvenate tired feet and improve circulation.</p>
                            <div style="margin-top:15px; color:var(--accent); font-weight:600;">$50</div>
                            <a href="#booking" class="btn" style="margin-top:15px; padding:8px 20px; font-size:0.9rem;">Book Now</a>
                        </div>
                    </div>
                    <div style="text-align:center; margin-top:40px;">
                        <a href="#services" class="btn">View All Services & Pricing</a>
                    </div>
                </div>
            </section>
        </section>
        
        <!-- Other page sections (initially hidden) -->
        <section id="servicesSection" class="page-section" style="display: none;"></section>
        <section id="testimonialsSection" class="page-section" style="display: none;"></section>
        <section id="contactSection" class="page-section" style="display: none;"></section>
        <section id="bookingSection" class="page-section" style="display: none;"></section>
    </main>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-container">
                <div class="footer-about">
                    <div class="footer-logo">Doris<span>Massage</span></div>
                    <p>Professional mobile spa services bringing relaxation and rejuvenation directly to your doorstep. Licensed, insured, and dedicated to your wellbeing.</p>
                    <div style="margin-top:20px;">
                        <a href="#" style="color:white; margin-right:15px;"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" style="color:white; margin-right:15px;"><i class="fab fa-instagram"></i></a>
                        <a href="https://wa.me/14244008570" style="color:white;"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                
                <div class="footer-links">
                    <h4>Quick Links</h4>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#services">Services & Pricing</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                        <li><a href="#contact">Contact Us</a></li>
                        <li><a href="#booking">Book Now</a></li>
                    </ul>
                </div>
                
                <div class="footer-contact">
                    <h4>Contact Info</h4>
<p>
    <i class="fas fa-envelope"></i>
    <a href="mailto:dorissandy0@gmail.com" style="color: inherit; text-decoration: none;">
        dorissandy0@gmail.com
    </a>
</p>
    <i class="fab fa-whatsapp"></i>
    <a href="https://wa.me/1424408570?text=Hello%20Doris,%20I%20would%20like%20to%20book%20a%20massage." target="_blank" style="color: inherit; text-decoration: none;">
        +1 (424) 400-8570
    </a>
</p>
                    <p><i class="fas fa-map-marker-alt"></i> Serving the Greater Area with Mobile Spa Services</p>
                    <p><i class="fas fa-clock"></i> By Appointment Only</p>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Doris Massage. All rights reserved.</p>
                <p style="margin-top:5px; font-size:0.8rem;">Website designed for mobile spa home service business</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');
        
        if (menuToggle) {
            menuToggle.addEventListener('click', () => {
                navLinks.classList.toggle('active');
            });
        }
        
        // Close mobile menu when clicking on a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });
        
        // Navigation System
        document.addEventListener('DOMContentLoaded', function() {
            // Get the initial hash from URL or default to 'home'
            const initialHash = window.location.hash.substring(1) || 'home';
            
            // Load the appropriate page based on hash
            loadPage(initialHash);
            
            // Set up navigation click handlers
            document.querySelectorAll('.nav-link').forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    const page = this.getAttribute('href').substring(1);
                    loadPage(page);
                    
                    // Update URL hash without page reload
                    window.history.pushState({}, '', '#' + page);
                });
            });
            
            // Handle browser back/forward buttons
            window.addEventListener('hashchange', function() {
                const page = window.location.hash.substring(1) || 'home';
                loadPage(page);
            });
        });
        
        function loadPage(page) {
            // Hide all page sections
            document.querySelectorAll('.page-section').forEach(section => {
                section.style.display = 'none';
            });
            
            // Update active nav link
            document.querySelectorAll('.nav-link').forEach(link => {
                link.classList.remove('active');
                if (link.getAttribute('href') === '#' + page) {
                    link.classList.add('active');
                }
            });
            
            // Show the requested page
            let targetSection;
            switch(page) {
                case 'home':
                    targetSection = document.getElementById('homeSection');
                    break;
                case 'services':
                    if (!document.getElementById('servicesSection').innerHTML) {
                        loadServicesPage();
                    }
                    targetSection = document.getElementById('servicesSection');
                    break;
                case 'testimonials':
                    if (!document.getElementById('testimonialsSection').innerHTML) {
                        loadTestimonialsPage();
                    }
                    targetSection = document.getElementById('testimonialsSection');
                    break;
                case 'contact':
                    if (!document.getElementById('contactSection').innerHTML) {
                        loadContactPage();
                    }
                    targetSection = document.getElementById('contactSection');
                    break;
                case 'booking':
                    if (!document.getElementById('bookingSection').innerHTML) {
                        loadBookingPage();
                    }
                    targetSection = document.getElementById('bookingSection');
                    break;
                default:
                    targetSection = document.getElementById('homeSection');
            }
            
            if (targetSection) {
                targetSection.style.display = 'block';
                // Scroll to top of the page
                window.scrollTo(0, 0);
            }
        }
        
        // Services Page Content
        function loadServicesPage() {
            const container = document.getElementById('servicesSection');
            container.innerHTML = `
                <section class="services">
                    <div class="container">
                        <h2>Services & Pricing</h2>
                        
                        <div class="service-note">
                            <h3><i class="fas fa-info-circle"></i> Important Note</h3>
                            <p>All our massage services include a complimentary, soothing conclusion to enhance your relaxation experience. The only exception is the Foot Scrub & Massage, which focuses specifically on foot and lower leg treatment.</p>
                            <p><strong>We offer outcall service to any location of your choice</strong> - homes, hotels, or offices. Our therapist brings all necessary equipment for a complete spa experience.</p>
                        </div>
                        
                        <div class="services-container">
                            <table class="services-table">
                                <thead>
                                    <tr>
                                        <th>Service</th>
                                        <th>Duration</th>
                                        <th>Price</th>
                                        <th>Action</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td><strong>Reservation Fee</strong><br><small>Required to secure your appointment</small></td>
                                        <td class="service-duration">—</td>
                                        <td class="service-price">$50</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Full Body Massage</strong><br><small>Complete relaxation targeting all major muscle groups</small></td>
                                        <td class="service-duration">50 min</td>
                                        <td class="service-price">$100</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Ultimate Full Body Massage</strong><br><small>Extended session for deep relaxation and tension release</small></td>
                                        <td class="service-duration">75 min</td>
                                        <td class="service-price">$155</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Deep Tissue Back Massage</strong><br><small>Focuses on chronic tension in back and shoulder muscles</small></td>
                                        <td class="service-duration">40 min</td>
                                        <td class="service-price">$95</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Hot Stone Massage (Full Body)</strong><br><small>Warm stones release deep muscle tension</small></td>
                                        <td class="service-duration">75 min</td>
                                        <td class="service-price">$150</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Lower Leg and Foot Massage</strong><br><small>Targeted relief for tired legs and feet</small></td>
                                        <td class="service-duration">30 min</td>
                                        <td class="service-price">$65</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                    <tr>
                                        <td><strong>Foot Scrub & Massage</strong><br><small>Exfoliating scrub followed by soothing massage</small></td>
                                        <td class="service-duration">30 min</td>
                                        <td class="service-price">$50</td>
                                        <td><a href="#booking" class="btn" style="padding:8px 15px; font-size:0.9rem;">Book Now</a></td>
                                    </tr>
                                </tbody>
                            </table>
                            
                            <div style="text-align:center; margin-top:40px;">
                                <a href="#booking" class="btn">Book Your Service Now</a>
                            </div>
                        </div>
                    </div>
                </section>
                
                <section class="features" style="background-color:#f8f8f2;">
                    <div class="container">
                        <h2>What to Expect</h2>
                        <div class="features-container">
                            <div class="feature-card">
                                <div class="feature-icon">
                                    <i class="fas fa-calendar-check"></i>
                                </div>
                                <h3>Easy Booking</h3>
                                <p>Schedule your appointment online in just a few clicks. You'll receive a confirmation and our therapist will contact you to finalize details.</p>
                            </div>
                            
                            <div class="feature-card">
                                <div class="feature-icon">
                                    <i class="fas fa-truck"></i>
                                </div>
                                <h3>We Come to You</h3>
                                <p>Our therapist arrives at your chosen location with all equipment: massage table, linens, oils, music, and ambiance elements.</p>
                            </div>
                            
                            <div class="feature-card">
                                <div class="feature-icon">
                                    <i class="fas fa-hand-sparkles"></i>
                                </div>
                                <h3>Professional Service</h3>
                                <p>Enjoy a customized treatment in the comfort of your own space. Our therapists are trained to adapt to your specific needs and preferences.</p>
                            </div>
                        </div>
                    </div>
                </section>
            `;
        }
        
        // Testimonials Page Content
        function loadTestimonialsPage() {
            const container = document.getElementById('testimonialsSection');
            container.innerHTML = `
                <section class="testimonials">
                    <div class="container">
                        <h2>Client Testimonials</h2>
                        <p style="text-align:center; max-width:800px; margin:0 auto 40px;">Don't just take our word for it. Here's what our clients have to say about their mobile spa experience with Doris Massage.</p>
                        
                        <div class="testimonials-container">
                            <div class="testimonial-card">
                                <div class="testimonial-header">
                                    <img src="https://images.unsplash.com/photo-1494790108755-2616b786d4d9?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" alt="Sarah Johnson" class="testimonial-img">
                                    <div class="testimonial-info">
                                        <h4>Sarah Johnson</h4>
                                        <p>Marketing Executive</p>
                                    </div>
                                </div>
                                <div class="testimonial-rating">
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                </div>
                                <p>"After months of back pain from my office chair, I booked the deep tissue massage. Doris was punctual, professional, and transformed my living room into a spa. The pain relief was immediate and lasting. I've already booked my next session!"</p>
                            </div>
                            
                            <div class="testimonial-card">
                                <div class="testimonial-header">
                                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=687&q=80" alt="Michael Rodriguez" class="testimonial-img">
                                    <div class="testimonial-info">
                                        <h4>Michael Rodriguez</h4>
                                        <p>Frequent Traveler</p>
                                    </div>
                                </div>
                                <div class="testimonial-rating">
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                </div>
                                <p>"As someone constantly in hotels, finding a reliable massage therapist is tough. This service is a lifesaver. I booked the Ultimate Full Body to my hotel after a long flight. It was the most convenient and effective way to combat jet lag. The therapist was discreet and incredibly skilled."</p>
                            </div>
                            
                            <div class="testimonial-card">
                                <div class="testimonial-header">
                                    <img src="https://images.unsplash.com/photo-1544725176-7c40e5a71c5e?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1167&q=80" alt="Jessica & David Miller" class="testimonial-img">
                                    <div class="testimonial-info">
                                        <h4>Jessica & David Miller</h4>
                                        <p>Couples Massage Clients</p>
                                    </div>
                                </div>
                                <div class="testimonial-rating">
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                </div>
                                <p>"We booked a couples massage for our anniversary. It was the perfect, luxurious treat without the hassle of leaving home. The therapists were incredibly professional and set up in our living room seamlessly. The entire experience from booking to the actual massage was flawless. 10/10!"</p>
                            </div>
                            
                            <div class="testimonial-card">
                                <div class="testimonial-header">
                                    <img src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=764&q=80" alt="Amanda Chen" class="testimonial-img">
                                    <div class="testimonial-info">
                                        <h4>Amanda Chen</h4>
                                        <p>New Mother</p>
                                    </div>
                                </div>
                                <div class="testimonial-rating">
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                    <i class="fas fa-star"></i>
                                </div>
                                <p>"As a new mom, I desperately needed some self-care but couldn't leave the house. The mobile spa service was a game-changer! The foot scrub and massage was exactly what I needed. The therapist was so understanding and worked around my baby's schedule. I felt rejuvenated and human again!"</p>
                            </div>
                        </div>
                        
                        <div style="text-align:center; margin-top:50px;">
                            <a href="#booking" class="btn">Book Your Experience Today</a>
                        </div>
                    </div>
                </section>
            `;
        }
        
        // Contact Page Content
        function loadContactPage() {
            const container = document.getElementById('contactSection');
            container.innerHTML = `
                <section class="contact">
                    <div class="container">
                        <h2>Contact Us</h2>
                        <p style="text-align:center; max-width:800px; margin:0 auto 40px;">Have questions or ready to book your mobile spa experience? Get in touch with us using the form below or contact us directly.</p>
                        
                        <div class="contact-container">
                            <div class="contact-info">
                                <h3>Get In Touch</h3>
                                <p>We're here to answer any questions you may have about our mobile spa services. Reach out to us and we'll respond as soon as possible.</p>
                                
                                <div class="contact-detail">
                                    <div class="contact-icon">
                                        <i class="fas fa-envelope"></i>
                                    </div>
                                    <div>
                                        <h4>Email</h4>
                                        <p>dorissandy0@gmail.com</p>
                                    </div>
                                </div>
                                
                                <div class="contact-detail">
                                    <div class="contact-icon">
                                        <i class="fab fa-whatsapp"></i>
                                    </div>
                                    <div>
                                        <h4>WhatsApp</h4>
                                        <p>+1 (424) 400-8570</p>
                                    </div>
                                </div>
                                
                                <div class="contact-detail">
                                    <div class="contact-icon">
                                        <i class="fas fa-map-marker-alt"></i>
                                    </div>
                                    <div>
                                        <h4>Service Area</h4>
                                        <p>We offer outcall service to homes, hotels, and offices throughout the Greater Area.</p>
                                    </div>
                                </div>
                                
                                <div class="contact-detail">
                                    <div class="contact-icon">
                                        <i class="fas fa-clock"></i>
                                    </div>
                                    <div>
                                        <h4>Hours</h4>
                                        <p>By appointment only<br>Flexible scheduling available</p>
                                    </div>
                                </div>
                            </div>
                            
                            <div class="contact-form">
                                <h3>Send a Message</h3>
                                <form id="contactForm">
                                    <div class="form-group">
                                        <label for="name">Full Name *</label>
                                        <input type="text" id="name" class="form-control" required>
                                    </div>
                                    
                                    <div class="form-group">
                                        <label for="email">Email Address *</label>
                                        <input type="email" id="email" class="form-control" required>
                                    </div>
                                    
                                    <div class="form-group">
                                        <label for="phone">Phone Number</label>
                                        <input type="tel" id="phone" class="form-control">
                                    </div>
                                    
                                    <div class="form-group">
                                        <label for="subject">Subject</label>
                                        <select id="subject" class="form-control">
                                            <option value="general">General Inquiry</option>
                                            <option value="booking">Booking Question</option>
                                            <option value="service">Service Information</option>
                                            <option value="other">Other</option>
                                        </select>
                                    </div>
                                    
                                    <div class="form-group">
                                        <label for="message">Message *</label>
                                        <textarea id="message" class="form-control" required></textarea>
                                    </div>
                                    
                                    <button type="submit" class="btn" style="width:100%;">Send Message</button>
                                </form>
                                
                                <div id="formMessage" style="margin-top:20px; display:none;"></div>
                            </div>
                        </div>
                    </div>
                </section>
            `;
            
            // Add contact form submission handler
            const contactForm = document.getElementById('contactForm');
            if (contactForm) {
                contactForm.addEventListener('submit', function(e) {
                    e.preventDefault();
                    
                    // In a real implementation, this would send to a server
                    const formMessage = document.getElementById('formMessage');
                    formMessage.innerHTML = '<div style="background-color:#d4edda; color:#155724; padding:15px; border-radius:5px; border:1px solid #c3e6cb;">Thank you for your message! We will get back to you within 24 hours.</div>';
                    formMessage.style.display = 'block';
                    
                    // Scroll to message
                    formMessage.scrollIntoView({ behavior: 'smooth' });
                    
                    // Reset form
                    contactForm.reset();
                });
            }
        }
        
        // Booking Page Content
        function loadBookingPage() {
            const container = document.getElementById('bookingSection');
            container.innerHTML = `
                <section class="booking">
                    <div class="container">
                        <h2>Book Your Session</h2>
                        <p style="text-align:center; max-width:800px; margin:0 auto 40px;">Schedule your mobile spa experience in just a few simple steps. Select your service, choose your time, and we'll handle the rest.</p>
                        
                        <div class="booking-container">
                            <div class="booking-steps">
                                <div class="step active" id="step1">
                                    <div class="step-number">1</div>
                                    <p>Select Service</p>
                                </div>
                                <div class="step" id="step2">
                                    <div class="step-number">2</div>
                                    <p>Choose Time</p>
                                </div>
                                <div class="step" id="step3">
                                    <div class="step-number">3</div>
                                    <p>Your Details</p>
                                </div>
                                <div class="step" id="step4">
                                    <div class="step-number">4</div>
                                    <p>Confirmation</p>
                                </div>
                            </div>
                            
                            <!-- Step 1: Service Selection -->
                            <div class="booking-form-section active" id="serviceSelection">
                                <h3>Select Your Service</h3>
                                <p>Choose from our range of professional massage and spa treatments.</p>
                                
                                <div class="service-options" id="serviceOptions">
                                    <!-- Service options will be populated by JavaScript -->
                                </div>
                                
                                <div class="payment-notice">
                                    <h4><i class="fas fa-info-circle"></i> Payment Information</h4>
                                    <p>After you submit your booking request, Doris will contact you via text within 1 hour to confirm timing and arrange secure payment directly. Your appointment is only confirmed after this payment arrangement.</p>
                                </div>
                                
                                <div style="text-align:right; margin-top:30px;">
                                    <button class="btn" id="nextToTime">Next: Choose Time</button>
                                </div>
                            </div>
                            
                            <!-- Step 2: Time Selection -->
                            <div class="booking-form-section" id="timeSelection">
                                <h3>Select Date & Time</h3>
                                <p>Choose your preferred date and time for your mobile spa service.</p>
                                
                                <div class="form-group">
                                    <label for="bookingDate">Preferred Date *</label>
                                    <input type="date" id="bookingDate" class="form-control" required>
                                </div>
                                
                                <div class="form-group">
                                    <label for="bookingTime">Preferred Time *</label>
                                    <select id="bookingTime" class="form-control" required>
                                        <option value="">Select a time</option>
                                        <option value="9:00">9:00 AM</option>
                                        <option value="10:00">10:00 AM</option>
                                        <option value="11:00">11:00 AM</option>
                                        <option value="12:00">12:00 PM</option>
                                        <option value="13:00">1:00 PM</option>
                                        <option value="14:00">2:00 PM</option>
                                        <option value="15:00">3:00 PM</option>
                                        <option value="16:00">4:00 PM</option>
                                        <option value="17:00">5:00 PM</option>
                                        <option value="18:00">6:00 PM</option>
                                        <option value="19:00">7:00 PM</option>
                                    </select>
                                </div>
                                
                                <div class="form-group">
                                    <label for="locationType">Service Location Type *</label>
                                    <select id="locationType" class="form-control" required>
                                        <option value="">Select location type</option>
                                        <option value="home">Private Home</option>
                                        <option value="hotel">Hotel</option>
                                        <option value="office">Office</option>
                                        <option value="other">Other</option>
                                    </select>
                                </div>
                                
                                <div style="display:flex; justify-content:space-between; margin-top:30px;">
                                    <button class="btn btn-secondary" id="backToService">Back to Services</button>
                                    <button class="btn" id="nextToDetails">Next: Your Details</button>
                                </div>
                            </div>
                            
                            <!-- Step 3: Client Details -->
                            <div class="booking-form-section" id="clientDetails">
                                <h3>Your Information</h3>
                                <p>Please provide your details so we can contact you to confirm your booking.</p>
                                
                                <div class="form-group">
                                    <label for="clientName">Full Name *</label>
                                    <input type="text" id="clientName" class="form-control" required>
                                </div>
                                
                                <div class="form-group">
                                    <label for="clientEmail">Email Address *</label>
                                    <input type="email" id="clientEmail" class="form-control" required>
                                </div>
                                
                                <div class="form-group">
                                    <label for="clientPhone">Phone Number *</label>
                                    <input type="tel" id="clientPhone" class="form-control" required>
                                    <small style="display:block; margin-top:5px; color:#666;">Doris will text you at this number to confirm your booking and arrange payment</small>
                                </div>
                                
                                <div class="form-group">
                                    <label for="clientAddress">Service Address *</label>
                                    <textarea id="clientAddress" class="form-control" required placeholder="Please provide the full address where you'd like the service performed"></textarea>
                                </div>
                                
                                <div class="form-group">
                                    <label for="specialRequests">Special Requests or Notes</label>
                                    <textarea id="specialRequests" class="form-control" placeholder="Any specific areas of focus, allergies, or other information we should know"></textarea>
                                </div>
                                
                                <div style="display:flex; justify-content:space-between; margin-top:30px;">
                                    <button class="btn btn-secondary" id="backToTime">Back to Time Selection</button>
                                    <button class="btn" id="submitBooking">Submit Booking Request</button>
                                </div>
                            </div>
                            
                            <!-- Step 4: Confirmation -->
                            <div class="booking-form-section" id="confirmation">
                                <div style="text-align:center; padding:40px 20px;">
                                    <div class="feature-icon" style="font-size:4rem; color:#4CAF50;">
                                        <i class="fas fa-check-circle"></i>
                                    </div>
                                    <h3>Booking Request Submitted!</h3>
                                    <p>Thank you for your booking request. <strong>Doris will contact you via text within 1 hour</strong> to confirm your appointment details and arrange payment directly.</p>
                                    <p>Your appointment is not confirmed until you receive this confirmation text and payment is arranged.</p>
                                    <div style="background-color:rgba(85, 107, 47, 0.1); padding:20px; border-radius:10px; margin:30px 0; text-align:left;">
                                        <h4>Next Steps:</h4>
                                        <ol style="padding-left:20px; margin-top:10px;">
                                            <li>Wait for Doris to text you (within 1 hour)</li>
                                            <li>Confirm your appointment time and details</li>
                                            <li>Arrange payment directly with Doris</li>
                                            <li>Prepare your space for your spa experience</li>
                                        </ol>
                                    </div>
                                    <a href="#home" class="btn">Return to Homepage</a>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
            `;
            
            // Initialize booking page functionality
            initializeBookingPage();
        }
        
        // Initialize booking page
        function initializeBookingPage() {
            // Services data
            const services = [
                { id: 1, name: "Reservation Fee", duration: "—", price: 50, desc: "Required to secure your appointment" },
                { id: 2, name: "Full Body Massage", duration: "50 min", price: 100, desc: "Complete relaxation targeting all major muscle groups" },
                { id: 3, name: "Ultimate Full Body Massage", duration: "75 min", price: 155, desc: "Extended session for deep relaxation and tension release" },
                { id: 4, name: "Deep Tissue Back Massage", duration: "40 min", price: 95, desc: "Focuses on chronic tension in back and shoulder muscles" },
                { id: 5, name: "Hot Stone Massage (Full Body)", duration: "75 min", price: 150, desc: "Warm stones release deep muscle tension" },
                { id: 6, name: "Lower Leg and Foot Massage", duration: "30 min", price: 65, desc: "Targeted relief for tired legs and feet" },
                { id: 7, name: "Foot Scrub & Massage", duration: "30 min", price: 50, desc: "Exfoliating scrub followed by soothing massage" }
            ];
            
            // Populate service options
            const serviceOptions = document.getElementById('serviceOptions');
            if (serviceOptions) {
                services.forEach(service => {
                    const serviceOption = document.createElement('div');
                    serviceOption.className = 'service-option';
                    serviceOption.dataset.id = service.id;
                    serviceOption.innerHTML = `
                        <h4>${service.name}</h4>
                        <p>${service.desc}</p>
                        <div class="price">$${service.price}</div>
                        <div class="duration">${service.duration}</div>
                    `;
                    serviceOptions.appendChild(serviceOption);
                    
                    // Add click event to select service
                    serviceOption.addEventListener('click', function() {
                        // Remove selected class from all options
                        document.querySelectorAll('.service-option').forEach(option => {
                            option.classList.remove('selected');
                        });
                        
                        // Add selected class to clicked option
                        this.classList.add('selected');
                        
                        // Store selected service
                        window.selectedService = service;
                    });
                });
            }
            
            // Set minimum date for booking to today
            const bookingDate = document.getElementById('bookingDate');
            if (bookingDate) {
                const today = new Date().toISOString().split('T')[0];
                bookingDate.min = today;
                
                // Set default to 3 days from now
                const defaultDate = new Date();
                defaultDate.setDate(defaultDate.getDate() + 3);
                bookingDate.value = defaultDate.toISOString().split('T')[0];
            }
            
            // Step navigation
            let currentStep = 1;
            
            // Next to time step
            const nextToTime = document.getElementById('nextToTime');
            if (nextToTime) {
                nextToTime.addEventListener('click', function() {
                    if (!window.selectedService) {
                        alert('Please select a service before continuing.');
                        return;
                    }
                    
                    // Update steps
                    document.getElementById('step1').classList.remove('active');
                    document.getElementById('step2').classList.add('active');
                    
                    // Show time selection, hide service selection
                    document.getElementById('serviceSelection').classList.remove('active');
                    document.getElementById('timeSelection').classList.add('active');
                    
                    currentStep = 2;
                });
            }
            
            // Back to service step
            const backToService = document.getElementById('backToService');
            if (backToService) {
                backToService.addEventListener('click', function() {
                    // Update steps
                    document.getElementById('step2').classList.remove('active');
                    document.getElementById('step1').classList.add('active');
                    
                    // Show service selection, hide time selection
                    document.getElementById('timeSelection').classList.remove('active');
                    document.getElementById('serviceSelection').classList.add('active');
                    
                    currentStep = 1;
                });
            }
            
            // Next to details step
            const nextToDetails = document.getElementById('nextToDetails');
            if (nextToDetails) {
                nextToDetails.addEventListener('click', function() {
                    const bookingDate = document.getElementById('bookingDate').value;
                    const bookingTime = document.getElementById('bookingTime').value;
                    const locationType = document.getElementById('locationType').value;
                    
                    if (!bookingDate || !bookingTime || !locationType) {
                        alert('Please fill in all required fields before continuing.');
                        return;
                    }
                    
                    // Update steps
                    document.getElementById('step2').classList.remove('active');
                    document.getElementById('step3').classList.add('active');
                    
                    // Show client details, hide time selection
                    document.getElementById('timeSelection').classList.remove('active');
                    document.getElementById('clientDetails').classList.add('active');
                    
                    currentStep = 3;
                });
            }
            
            // Back to time step
            const backToTime = document.getElementById('backToTime');
            if (backToTime) {
                backToTime.addEventListener('click', function() {
                    // Update steps
                    document.getElementById('step3').classList.remove('active');
                    document.getElementById('step2').classList.add('active');
                    
                    // Show time selection, hide client details
                    document.getElementById('clientDetails').classList.remove('active');
                    document.getElementById('timeSelection').classList.add('active');
                    
                    currentStep = 2;
                });
            }
            
            // Submit booking
            const submitBooking = document.getElementById('submitBooking');
            if (submitBooking) {
                submitBooking.addEventListener('click', function() {
                    const clientName = document.getElementById('clientName').value;
                    const clientEmail = document.getElementById('clientEmail').value;
                    const clientPhone = document.getElementById('clientPhone').value;
                    const clientAddress = document.getElementById('clientAddress').value;
                    
                    if (!clientName || !clientEmail || !clientPhone || !clientAddress) {
                        alert('Please fill in all required fields before submitting.');
                        return;
                    }
                    
                    // In a real implementation, this data would be sent to a server
                    // For this demo, we'll simulate a booking submission
                    
                    // Update steps
                    document.getElementById('step3').classList.remove('active');
                    document.getElementById('step4').classList.add('active');
                    
                    // Show confirmation, hide client details
                    document.getElementById('clientDetails').classList.remove('active');
                    document.getElementById('confirmation').classList.add('active');
                    
                    // Scroll to top of confirmation
                    document.getElementById('confirmation').scrollIntoView({ behavior: 'smooth' });
                    
                    // Simulate sending notification to Doris
                    console.log('Booking submitted:');
                    console.log('Service:', window.selectedService);
                    console.log('Client:', clientName, clientEmail, clientPhone);
                    console.log('Address:', clientAddress);
                    console.log('Doris should receive a notification to contact client at:', clientPhone);
                });
            }
        }
    </script>
</body>
</html>
