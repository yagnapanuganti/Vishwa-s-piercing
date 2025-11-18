# Vishwa-s-piercing
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vishwa's Ear Piercing - The New Accent for Your Elegance</title>
    <!-- Google Fonts for an elegant look -->
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <!-- Icon Library (for cart, social media) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">

    <style>
        /* ======== GLOBAL STYLES & COLOR PALETTE ======== */
        :root {
            --font-primary: 'Playfair Display', serif;
            --font-secondary: 'Poppins', sans-serif;
            --color-gold: #D4AF37;
            --color-ruby: #9B111E;
            --color-emerald: #50C878;
            --color-dark: #2c1810;
            --color-light: #FFF8E7;
            --color-text: #333;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
            scroll-padding-top: 70px;
            /* Offset for fixed navbar */
        }

        body {
            font-family: var(--font-secondary);
            color: var(--color-text);
            background-color: var(--color-light);
            background-image: linear-gradient(rgba(255, 248, 231, 0.0), rgba(0, 0, 0, 0.5)), url('https://res.cloudinary.com/dpk7jrejo/image/upload/v1762174514/Gemini_Generated_Image_lpoo84lpoo84lpoo_pjbugm.png');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .page-section {
            padding-top: 80px;
            padding-bottom: 60px;
        }

        .page-section-overlay {
            background: rgba(255, 255, 255, 0.85);
            backdrop-filter: blur(5px);
        }

        h1,
        h2,
        h3 {
            font-family: var(--font-primary);
            font-weight: 700;
            color: var(--color-dark);
        }

        h2 {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 40px;
        }

        h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
        }

        p {
            line-height: 1.6;
            margin-bottom: 15px;
        }

        a {
            text-decoration: none;
            color: var(--color-ruby);
        }

        .hidden {
            display: none !important;
        }

        /* ======== BUTTONS ======== */
        .btn {
            display: inline-block;
            padding: 12px 28px;
            border-radius: 50px;
            font-weight: 600;
            font-family: var(--font-secondary);
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: all 0.3s ease;
            border: 2px solid transparent;
            cursor: pointer;
            text-align: center;
        }

        .btn-primary {
            background-color: var(--color-ruby);
            color: #FFFAF2;
        }

        .btn-primary:hover {
            background-color: #7a0d17;
            transform: translateY(-2px);
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .btn-secondary {
            background-color: transparent;
            color: #FFFAF2;
            border-color: #FFFAF2;
        }

        .btn-secondary:hover {
            background-color: var(--color-ruby);
            color: #FFFAF2;
            border-color: var(--color-ruby);
        }

        .btn-full {
            width: 100%;
        }

        /* ======== HEADER & NAVIGATION ======== */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.9);
            backdrop-filter: blur(10px);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            z-index: 1000;
        }

        .navbar .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 70px;
        }

        .nav-logo {
            font-family: var(--font-primary);
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--color-dark);
            cursor: pointer;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 30px;
        }

        .nav-link {
            font-weight: 600;
            color: var(--color-text);
            transition: color 0.3s ease;
            cursor: pointer;
        }

        .nav-link:hover,
        .nav-link.active {
            color: var(--color-ruby);
        }

        .nav-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--color-dark);
        }

        /* ======== HOME/HERO SECTION ======== */
        .hero {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: flex-end;
            text-align: center;
            padding-top: 70px;
        }

        .hero-content {
            max-width: 800px;
            padding: 0 20px 60px 20px;
            width: 100%;
            margin-left: auto;
            margin-right: auto;
        }

        .hero-title {
            font-size: 3.5rem;
            color: #FFFAF2;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            font-family: var(--font-primary);
            font-style: italic;
            color: #FFFAF2;
            margin-bottom: 30px;
        }

        .hero-buttons {
            margin-bottom: 20px;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .hero-buttons .btn.nav-link {
            color: #FFFAF2;
        }

        .hero-buttons .btn-secondary.nav-link {
            border-color: #FFFAF2;
        }

        .hero-buttons .btn-secondary.nav-link:hover {
            color: #FFFAF2;
        }

        /* ======== SERVICES HIGHLIGHT SECTION ======== */
        #services {
            background: rgba(255, 255, 255, 0.7);
        }

        .services-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
        }

        .service-card {
            background: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            border-top: 4px solid var(--color-gold);
        }

        .service-card i {
            font-size: 3rem;
            color: var(--color-ruby);
            margin-bottom: 15px;
        }

        .service-card h3 {
            font-size: 1.8rem;
            color: var(--color-dark);
        }

        .service-card p {
            font-size: 1rem;
            color: #555;
            margin-bottom: 0;
        }

        /* ======== COLLECTION SLIDER SECTION ======== */
        #collection {
            background: rgba(255, 248, 231, 0.9);
            padding-left: 0;
            padding-right: 0;
        }

        #collection h2 {
            padding-left: 20px;
            padding-right: 20px;
        }

        /* NEW: Category Filters */
        .category-filters {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 30px;
            flex-wrap: wrap;
            padding: 0 20px;
        }

        .category-btn {
            padding: 10px 22px;
            font-size: 1rem;
            border: 2px solid var(--color-ruby);
            background: transparent;
            color: var(--color-ruby);
            border-radius: 20px;
            cursor: pointer;
            transition: all 0.3s ease;
            font-weight: 600;
        }

        .category-btn:hover,
        .category-btn.active {
            background: var(--color-ruby);
            color: white;
        }

        .collection-slider-wrapper {
            position: relative;
        }

        .collection-slider {
            display: flex;
            overflow-x: auto;
            padding: 20px;
            gap: 20px;
            -ms-overflow-style: none;
            scrollbar-width: none;
        }

        .collection-slider::-webkit-scrollbar {
            display: none;
        }

        .collection-card {
            flex: 0 0 250px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            overflow: hidden;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            text-align: center;
            display: flex;
            flex-direction: column;
        }

        .collection-card-image {
            width: 100%;
            height: 220px;
            object-fit: cover;
        }

        .collection-card-info {
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .collection-card-info h3 {
            font-size: 1.4rem;
            color: var(--color-dark);
            margin-bottom: 15px;
            /* Added margin */
        }

        /* NEW: Select Button */
        .btn-select {
            padding: 8px 15px;
            font-size: 0.9rem;
            border-radius: 5px;
            background: var(--color-gold);
            color: var(--color-dark);
            border: none;
            width: 100%;
        }

        .btn-select:hover {
            background: #c5a230;
        }

        .btn-select:disabled {
            background: #ccc;
            color: #777;
            cursor: not-allowed;
        }

        /* Special card for Piercing Ceremony */
        .collection-card-special {
            flex: 0 0 250px;
            background: var(--color-ruby);
            color: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.08);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            text-align: center;
            cursor: pointer;
        }

        .collection-card-special:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }

        .collection-card-special i {
            font-size: 3rem;
            margin-bottom: 15px;
        }

        .collection-card-special h3 {
            font-size: 1.5rem;
            color: white;
            margin-bottom: 10px;
        }

        .collection-card-special p {
            font-size: 0.9rem;
            color: #FFFAF2;
            margin-bottom: 0;
        }

        /* ======== BOOKING SECTION (UPDATED) ======== */
        #book {
            background: rgba(255, 255, 255, 0.85);
        }

        #booking-form {
            /* RE-ADD 2-COLUMN LAYOUT */
            display: grid;
            grid-template-columns: 1fr;
            /* Default to 1 column */
            gap: 40px;
            max-width: 900px;
            /* Widen for 2 columns */
            margin: 0 auto;
            background: white;
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.07);
        }

        .form-column h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            border-bottom: 2px solid var(--color-gold);
            padding-bottom: 10px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .form-group input,
        .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-family: var(--font-secondary);
            font-size: 1rem;
        }

        .payment-note {
            font-size: 0.9rem;
            text-align: center;
            margin-top: 15px;
            color: #666;
        }

        /* NEW: Cart Summary in Form */
        #cart-summary-display {
            min-height: 150px;
            background: var(--color-light);
            border-radius: 5px;
            padding: 20px;
            margin-bottom: 20px;
        }

        #cart-summary-display p {
            color: #555;
            margin-bottom: 0;
        }

        .cart-summary-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 10px 0;
            border-bottom: 1px dashed #ddd;
            font-weight: 600;
        }

        .cart-summary-item:last-child {
            border-bottom: none;
        }

        .cart-summary-item button {
            background: var(--color-ruby);
            color: white;
            border: none;
            border-radius: 50%;
            width: 24px;
            height: 24px;
            font-size: 0.8rem;
            font-weight: bold;
            cursor: pointer;
            line-height: 24px;
        }

        /* Confirmation Message */
        #booking-confirmation {
            text-align: center;
            background: white;
            padding: 50px;
            border-radius: 10px;
        }

        .confirm-icon {
            font-size: 5rem;
            color: var(--color-emerald);
            margin-bottom: 20px;
        }

        #booking-confirmation h2 {
            font-size: 2.5rem;
            color: var(--color-dark);
        }

        #booking-confirmation p {
            font-size: 1.2rem;
            color: #555;
        }

        .booking-tracker {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-top: 40px;
            max-width: 700px;
            margin-left: auto;
            margin-right: auto;
            position: relative;
        }

        .step {
            text-align: center;
            width: 100px;
            position: relative;
            z-index: 2;
        }

        .step-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: #eee;
            color: #aaa;
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 0 auto 10px auto;
            font-size: 1.2rem;
            border: 3px solid #eee;
        }

        .step p {
            font-weight: 600;
            color: #aaa;
            font-size: 0.9rem;
        }

        .booking-tracker::before {
            content: '';
            position: absolute;
            top: 25px;
            left: 10%;
            right: 10%;
            height: 4px;
            background: #eee;
            z-index: 1;
        }

        .step.active .step-icon {
            background: var(--color-emerald);
            border-color: var(--color-emerald);
            color: white;
        }

        .step.active p {
            color: var(--color-dark);
        }

        /* ======== CONTACT SECTION ======== */
        #contact {
            background: rgba(255, 248, 231, 0.9);
        }

        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            background: white;
            padding: 40px;
            border-radius: 10px;
        }

        .contact-details h3,
        .contact-form-wrapper h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
        }

        .contact-details ul {
            list-style: none;
            margin: 20px 0;
        }

        .contact-details li {
            font-size: 1.1rem;
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .contact-details li i {
            font-size: 1.2rem;
            color: var(--color-ruby);
            width: 20px;
            text-align: center;
        }

        .social-icons a {
            font-size: 1.8rem;
            color: var(--color-dark);
            margin-right: 20px;
            transition: color 0.3s ease;
        }

        .social-icons a:hover {
            color: var(--color-ruby);
        }

        /* ======== FOOTER ======== */
        footer {
            text-align: center;
            padding: 30px;
            background: var(--color-dark);
            color: var(--color-light);
            margin-top: 0;
        }

        /* ======== CUSTOM MODAL (FOR CEREMONY & ALERTS) ======== */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.6);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 2000;
            opacity: 0;
            visibility: hidden;
            transition: opacity 0.3s ease, visibility 0.3s ease;
        }

        .modal-overlay.active {
            opacity: 1;
            visibility: visible;
        }

        .modal-content {
            background: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 20px rgba(0, 0, 0, 0.2);
            max-width: 500px;
            width: 90%;
            transform: scale(0.9);
            transition: transform 0.3s ease;
        }

        .modal-overlay.active .modal-content {
            transform: scale(1);
        }

        .modal-content p {
            font-size: 1.1rem;
            margin-bottom: 20px;
            color: var(--color-text);
        }

        #ceremony-modal-content {
            text-align: left;
        }

        #ceremony-modal-content h3 {
            text-align: center;
            font-size: 1.8rem;
            color: var(--color-dark);
        }

        #ceremony-modal-content ul {
            list-style: none;
            padding-left: 0;
            margin-top: 20px;
        }

        #ceremony-modal-content li {
            font-size: 1.1rem;
            margin-bottom: 15px;
            display: flex;
            align-items: flex-start;
            gap: 10px;
        }

        #ceremony-modal-content li i {
            color: var(--color-gold);
            padding-top: 5px;
        }

        .modal-buttons {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-top: 25px;
        }

        .modal-close-btn {
            position: absolute;
            top: 10px;
            right: 15px;
            font-size: 1.5rem;
            color: #888;
            cursor: pointer;
            transition: color 0.3s ease;
        }

        .modal-close-btn:hover {
            color: #333;
        }

        /* ======== RESPONSIVENESS (TABLET & MOBILE) ======== */
        @media (min-width: 769px) {

            /* 2-column booking form on desktop */
            #booking-form {
                grid-template-columns: 1.2fr 1fr;
            }
        }

        @media (max-width: 900px) {
            .contact-container {
                grid-template-columns: 1fr;
            }

            .booking-tracker::before {
                left: 50px;
                right: 50px;
            }
        }

        @media (max-width: 768px) {
            .nav-menu {
                position: fixed;
                top: 70px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 70px);
                background: white;
                flex-direction: column;
                align-items: center;
                padding-top: 40px;
                gap: 40px;
                transition: left 0.4s ease-in-out;
            }

            .nav-menu.active {
                left: 0;
            }

            .nav-link {
                font-size: 1.2rem;
            }

            .nav-toggle {
                display: block;
            }

            .hero-title {
                font-size: 2.5rem;
            }

            .hero-subtitle {
                font-size: 1.2rem;
            }

            .booking-tracker {
                flex-direction: column;
                align-items: center;
                gap: 10px;
            }

            .booking-tracker::before {
                top: 30px;
                bottom: 30px;
                left: 50%;
                transform: translateX(-50%);
                width: 4px;
                height: auto;
                right: auto;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .collection-card,
            .collection-card-special {
                flex-basis: 220px;
            }
        }

        @media (max-width: 480px) {
            .hero-title {
                font-size: 2rem;
            }

            .hero-buttons {
                flex-direction: column;
                gap: 15px;
            }

            #booking-form,
            .contact-container {
                padding: 20px;
            }

            .container {
                padding: 0 15px;
            }

            .collection-card,
            .collection-card-special {
                flex-basis: 200px;
            }

            #collection {
                padding-left: 0;
                padding-right: 0;
            }

            .collection-slider {
                padding: 20px 15px;
            }
        }
    </style>
</head>

<body>

    <header class="navbar">
        <div class="container">
            <a class="nav-logo nav-link" href="#home">Vishwa's</a>
            <nav>
                <ul class="nav-menu" id="nav-menu">
                    <li><a class="nav-link active" href="#home">Home</a></li>
                    <li><a class="nav-link" href="#collection">Collection</a></li>
                    <li><a class="nav-link" href="#book">Book Now</a></li>
                    <li><a class="nav-link" href="#contact">Contact</a></li>
                </ul>
            </nav>
            <div class="nav-toggle" id="nav-toggle">
                <i class="fas fa-bars"></i>
            </div>
        </div>
    </header>

    <main>
        <section id="home" class="hero">
            <div class="hero-content">
                <h1 class="hero-title">VISHWA'S EAR PIERCING</h1>
                <p class="hero-subtitle">"The new accent for your elegance."</p>
                <div class="hero-buttons">
                    <a class="btn btn-primary nav-link" href="#book">Book Now</a>
                    <a class="btn btn-secondary nav-link" href="#collection">View Collection</a>
                </div>
            </div>
        </section>

        <section id="services" class="page-section">
            <div class="container">
                <div class="services-grid">
                    <div class="service-card">
                        <i class="fas fa-home"></i>
                        <h3>At-Home Service</h3>
                        <p>Safe, hygienic, and professional piercing in the comfort of your home.</p>
                    </div>
                    <div class="service-card">
                        <i class="fas fa-store"></i>
                        <h3>In-Studio Piercing</h3>
                        <p>Visit our clean and welcoming studio for a personalized experience.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="collection" class="page-section">
            <div class="container">
                <h2>Our Collection</h2>
                <!-- NEW: Category Filters -->
                <div class="category-filters" id="category-filters">
                    <button class="category-btn active" data-category="ear">Ear</button>
                    <button class="category-btn" data-category="nose">Nose</button>
                    <button class="category-btn" data-category="other">Other</button>
                </div>
            </div>
            <div class="collection-slider-wrapper">
                <div class="collection-slider" id="collection-slider">
                    <!-- Items will be injected here by JavaScript -->
                </div>
            </div>
        </section>

        <section id="book" class="page-section page-section-overlay">
            <div class="container">
                <h2>Book Your Appointment</h2>
                <div class="booking-wrapper" id="booking-wrapper">
                    <!-- 
                      THIS IS UPDATED WITH YOUR LIVE URL
                    -->
                    <form id="booking-form" action="https://script.google.com/macros/s/AKfycbxgHgx4x88e-e6cEBMc01zMeXouQO4IV6DBVaLZQgzC67nULZwX9NhUzNWIwAnobzGKpA/exec" method="POST">
                        <!-- Left Column: User Details -->
                        <div class="form-column">
                            <h3>Booking Details</h3>
                            <input type="hidden" name="formType" value="booking">
                            <div class="form-group">
                                <label for="name">Name</label>
                                <input type="text" id="name" name="name" required>
                            </div>
                            <div class="form-group">
                                <label for="age">Age</label>
                                <input type="number" id="age" name="age" required>
                            </div>
                            <div class="form-group">
                                <label for="address">Address</label>
                                <input type="text" id="address" name="address" required>
                            </div>
                            <div class="form-group">
                                <label for="contact-num">Contact Number</label>
                                <input type="tel" id="contact-num" name="contact" required>
                            </div>
                            <div class="form-group">
                                <label for="preferred-date">Preferred Date</label>
                                <input type="date" id="preferred-date" name="preferred_date">
                            </div>
                            <div class="form-group">
                                <label for="message">Message</label>
                                <textarea id="message" name="message" rows="3"></textarea>
                            </div>
                        </div>

                        <!-- Right Column: Selections -->
                        <div class="form-column">
                            <h3>Your Selected Piercings</h3>
                            <div id="cart-summary-display">
                                <p>Please select at least one item from the <a class="nav-link" href="#collection">Collection</a>.</p>
                            </div>
                            <!-- This hidden input will hold the list of selected items for the form -->
                            <input type="hidden" name="selected_piercings" id="cart-summary-hidden">
                            <button type="submit" class="btn btn-primary btn-full" id="booking-submit-btn">Confirm Booking</button>
                            <p class="payment-note">Note: Payment is on delivery time.</p>
                        </div>
                    </form>

                    <!-- Confirmation Template -->
                    <div id="booking-confirmation-template" class="hidden">
                        <div id="booking-confirmation">
                            <div class="confirm-icon"><i class="fas fa-check-circle"></i></div>
                            <h2>Congratulations!</h2>
                            <p>Your booking is confirmed.</p>
                            <p>We will contact you shortly to confirm the date and time.</p>
                            <div class="booking-tracker">
                                <div class="step active">
                                    <div class="step-icon"><i class="fas fa-check"></i></div>
                                    <p>Confirmed</p>
                                </div>
                                <div class="step">
                                    <div class="step-icon"><i class="fas fa-calendar-alt"></i></div>
                                    <p>Date of Piercing</p>
                                </div>
                                <div class="step">
                                    <div class="step-icon"><i class="fas fa-motorcycle"></i></div>
                                    <p>On the Way</p>
                                </div>
                                <div class="step">
                                    <div class="step-icon"><i class="fas fa-star"></i></div>
                                    <p>Completed</p>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="page-section">
            <div class="container contact-container">
                <div class="contact-details">
                    <h3>Contact Us</h3>
                    <p>For any ceremony-related queries, feel free to get in touch. Consultations are free!</p>
                    <ul>
                        <li><i class="fas fa-user"></i> Vishwa Nelakonda</li>
                        <li><i class="fas fa-map-marker-alt"></i> Kondapur</li>
                        <li><i class="fas fa-phone"></i> +91 9059651118</li>
                        <li><i class="fas fa-envelope"></i> vishwachinna3210@gmail.com</li>
                    </ul>
                    <div class="social-icons">
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                        <a href="mailto:vishwachinna3210@gmail.com"><i class="fas fa-envelope"></i></a>
                    </div>
                </div>
                <div class="contact-form-wrapper">
                    <h3>Send us a Message</h3>
                    <!-- 
                      THIS IS UPDATED WITH YOUR LIVE URL
                    -->
                    <form id="contact-form" action="https://script.google.com/macros/s/AKfycbxgHgx4x88e-e6cEBMc01zMeXouQO4IV6DBVaLZQgzC67nULZwX9NhUzNWIwAnobzGKpA/exec" method="POST">
                        <input type="hidden" name="formType" value="contact">
                        <div class="form-group">
                            <label for="contact-name">Name</label>
                            <input type="text" id="contact-name" name="name" required>
                        </div>
                        <div class="form-group">
                            <label for="contact-phone">Phone</label>
                            <input type="tel" id="contact-phone" name="phone" required>
                        </div>
                        <div class="form-group">
                            <label for="contact-address">Address</label>
                            <input type="text" id="contact-address" name="address">
                        </div>
                        <button type="submit" class="btn btn-primary" id="contact-submit-btn">Send</button>
                    </form>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 Vishwa's Ear Piercing. All Rights Reserved.</p>
    </footer>

    <div id="ceremony-modal" class="modal-overlay">
        <div class="modal-content">
            <div id="ceremony-modal-content">
                <span class="modal-close-btn" id="ceremony-close-btn">&times;</span>
                <h3>Piercing Ceremony</h3>
                <ul>
                    <li><i class="fas fa-star"></i> <span>Welcome to Vishwa's Piercing.</span></li>
                    <li><i class="fas fa-star"></i> <span>Children's ear piercing ceremony is very special to us.</span></li>
                    <li><i class="fas fa-star"></i> <span>Book an appointment to get the catalogue of piercing jewellery.</span></li>
                    <li><i class="fas fa-star"></i> <span>Our professional will contact you.</span></li>
                </ul>
                <div class="modal-buttons">
                    <a id="modal-select-btn" class="btn btn-secondary nav-link" href="#collection">Select type of piercing</a>
                    <a id="modal-book-btn" class="btn btn-primary nav-link" href="#book">Book Now</a>
                </div>
            </div>
        </div>
    </div>

    <div id="alert-modal" class="modal-overlay">
        <div class="modal-content">
            <p id="alert-message" style="text-align: center;"></p>
            <button id="alert-close-btn" class="btn btn-primary" style="margin: 0 auto; display: block;">OK</button>
        </div>
    </div>


    <!-- ======== JAVASCRIPT (Updated for Selections) ======== -->
    <script>
        document.addEventListener("DOMContentLoaded", () => {

            // ======== NEW: PIERCING DATA ========
            const piercingData = [
                // Ear Piercings
                {
                    id: 1,
                    category: 'ear',
                    name: 'Forward Helix',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/forward-helix_wtfgww.jpg'
                },
                {
                    id: 2,
                    category: 'ear',
                    name: 'Rook',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/rook_kbldet.jpg'
                },
                {
                    id: 3,
                    category: 'ear',
                    name: 'Daith',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/daith_x37jjs.jpg'
                },
                {
                    id: 4,
                    category: 'ear',
                    name: 'Tragus',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/tragus_8dc5c9ae-2cfb-4065-89c3-4ad582d3abbc_fo3kqc.jpg'
                },
                {
                    id: 5,
                    category: 'ear',
                    name: 'Lobe',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/lobe_e0afd7cd-5566-42b5-ad66-ce8e94b858f9_nqriji.jpg'
                },
                {
                    id: 6,
                    category: 'ear',
                    name: 'Conch',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/conch_a5jc5u.jpg'
                },
                {
                    id: 7,
                    category: 'ear',
                    name: 'Helix',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/helix_uw6j30.jpg'
                },
                {
                    id: 8,
                    category: 'ear',
                    name: 'Flat',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762285499/Gemini_Generated_Image_x8l4vgx8l4vgx8l4_pxlw21.png'
                },
                // Nose Piercings
                {
                    id: 9,
                    category: 'nose',
                    name: 'Gemstone',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284897/gemstone-nose_iyogof.jpg'
                },
                {
                    id: 10,
                    category: 'nose',
                    name: 'Diamond',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284897/diamond-nose2_tpz6ih.jpg'
                },
                {
                    id: 11,
                    category: 'nose',
                    name: 'Hoop',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284897/nose-hoop_cc39e742-86b6-4189-9460-f21f356b7cb0_ofydai.jpg'
                },
                {
                    id: 12,
                    category: 'nose',
                    name: 'Stud',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/stud-nose_wj2dj8.jpg'
                },
                {
                    id: 13,
                    category: 'nose',
                    name: 'Septum',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/septum_hmkepv.jpg'
                },
                {
                    id: 14,
                    category: 'nose',
                    name: 'Charm',
                    image: 'https://res.cloudinary.com/dpk7jrejo/image/upload/v1762284896/charm-nose_xur9pc.jpg'
                },
                // Other
                {
                    id: 15,
                    category: 'other',
                    name: 'Other Piercings',
                    image: 'https://placehold.co/400x400/9B111E/FFFFFF?text=Other'
                }
            ];

            // ======== GLOBAL STATE ========
            let selectedPiercings = []; // This is our "cart"
            let currentCategory = 'ear'; // Default category

            // ======== SELECTORS ========
            const navToggle = document.getElementById("nav-toggle");
            const navMenu = document.getElementById("nav-menu");
            const allNavLinks = document.querySelectorAll(".nav-link");
            const allSections = document.querySelectorAll("main section[id]");
            const bookingForm = document.getElementById("booking-form");
            const bookingWrapper = document.getElementById("booking-wrapper");
            const bookingConfirmationTemplate = document.getElementById("booking-confirmation-template");
            const contactForm = document.getElementById("contact-form");
            const bookingSubmitBtn = document.getElementById("booking-submit-btn");
            const contactSubmitBtn = document.getElementById("contact-submit-btn");
            const categoryFilters = document.getElementById("category-filters");
            const collectionSlider = document.getElementById("collection-slider");
            const cartSummaryDisplay = document.getElementById("cart-summary-display");
            const cartSummaryHidden = document.getElementById("cart-summary-hidden");

            // ======== CUSTOM ALERT MODAL ========
            const alertModal = document.getElementById("alert-modal");
            const alertMessage = document.getElementById("alert-message");
            const alertCloseBtn = document.getElementById("alert-close-btn");

            function showAlert(message) {
                alertMessage.innerText = message;
                alertModal.classList.add("active");
            }

            function hideAlert() {
                alertModal.classList.remove("active");
            }
            alertCloseBtn.addEventListener("click", hideAlert);
            alertModal.addEventListener("click", (e) => {
                if (e.target === alertModal) hideAlert();
            });

            // ======== CEREMONY MODAL ========
            const ceremonyModal = document.getElementById("ceremony-modal");
            // Note: ceremonyOpenBtn is defined dynamically after render
            const ceremonyCloseBtn = document.getElementById("ceremony-close-btn");
            const modalBookBtn = document.getElementById("modal-book-btn");
            const modalSelectBtn = document.getElementById("modal-select-btn");

            function openCeremonyModal() {
                if (ceremonyModal) ceremonyModal.classList.add("active");
            }

            function closeCeremonyModal() {
                if (ceremonyModal) ceremonyModal.classList.remove("active");
            }

            if (ceremonyCloseBtn) ceremonyCloseBtn.addEventListener("click", closeCeremonyModal);
            if (modalBookBtn) modalBookBtn.addEventListener("click", closeCeremonyModal);
            if (modalSelectBtn) modalSelectBtn.addEventListener("click", closeCeremonyModal);
            if (ceremonyModal) ceremonyModal.addEventListener("click", (e) => {
                if (e.target === ceremonyModal) closeCeremonyModal();
            });

            // ======== NAVIGATION & SCROLLING ========
            navToggle.addEventListener("click", () => {
                navMenu.classList.toggle("active");
            });

            allNavLinks.forEach(link => {
                link.addEventListener('click', (e) => {

                    const href = link.getAttribute('href');

                    // Special case for cart summary link
                    if (e.currentTarget.parentElement && e.currentTarget.parentElement.id === 'cart-summary-display') {
                        // Don't prevent default, just close menu and scroll
                    } else {
                        e.preventDefault();
                    }

                    const targetId = href.substring(1);
                    const targetElement = document.getElementById(targetId);

                    if (targetElement) {
                        allNavLinks.forEach(l => l.classList.remove('active'));
                        const mainNavLink = document.querySelector(`.nav-menu .nav-link[href="${href}"]`);
                        if (mainNavLink) {
                            mainNavLink.classList.add('active');
                        } else if (link.classList.contains('nav-logo')) {
                            document.querySelector(`.nav-menu .nav-link[href="#home"]`).classList.add('active');
                        }
                        const navbarHeight = document.querySelector('.navbar').offsetHeight;
                        const elementPosition = targetElement.getBoundingClientRect().top + window.scrollY;
                        window.scrollTo({
                            top: elementPosition - navbarHeight,
                            behavior: 'smooth'
                        });
                    }
                    if (navMenu.classList.contains('active')) {
                        navMenu.classList.remove('active');
                    }
                });
            });

            window.addEventListener('scroll', () => {
                let currentSection = '';
                const navbarHeight = document.querySelector('.navbar').offsetHeight;
                allSections.forEach(section => {
                    const sectionTop = section.offsetTop - navbarHeight - 20;
                    if (window.scrollY >= sectionTop) {
                        currentSection = section.getAttribute('id');
                    }
                });
                allNavLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${currentSection}`) {
                        link.classList.add('active');
                    }
                });
                if (currentSection === 'home') {
                    document.querySelector('.nav-logo').classList.add('active');
                }
            });

            // ======== COLLECTION & SELECTION LOGIC ========

            function renderCollection(category) {
                if (!collectionSlider) return;
                collectionSlider.innerHTML = "";

                const ceremonyCard = document.createElement('div');
                ceremonyCard.className = 'collection-card-special';
                ceremonyCard.id = 'piercing-ceremony-btn';
                ceremonyCard.innerHTML = `
                    <i class="fas fa-star"></i>
                    <h3>Piercing Ceremony</h3>
                    <p>Learn more about our special service for children.</p>
                `;
                ceremonyCard.addEventListener('click', openCeremonyModal);
                collectionSlider.appendChild(ceremonyCard);

                const items = piercingData.filter(item => item.category === category);

                items.forEach(item => {
                    const card = document.createElement('div');
                    card.className = 'collection-card';
                    const isSelected = selectedPiercings.some(sel => sel.id === item.id);

                    card.innerHTML = `
                        <img src="${item.image}" alt="${item.name}" class="collection-card-image" onerror="this.src='https://placehold.co/400x400?text=Image+Error'">
                        <div class="collection-card-info">
                            <h3>${item.name}</h3>
                            <button class="btn btn-select" data-id="${item.id}" ${isSelected ? 'disabled' : ''}>
                                ${isSelected ? 'Selected' : 'Select'}
                            </button>
                        </div>
                    `;
                    collectionSlider.appendChild(card);
                });

                collectionSlider.querySelectorAll('.btn-select').forEach(button => {
                    button.addEventListener('click', handleSelectClick);
                });
            }

            categoryFilters.addEventListener('click', (e) => {
                if (e.target.tagName === 'BUTTON') {
                    currentCategory = e.target.dataset.category;
                    categoryFilters.querySelectorAll('button').forEach(btn => btn.classList.remove('active'));
                    e.target.classList.add('active');
                    renderCollection(currentCategory);
                }
            });

            function handleSelectClick(e) {
                const button = e.currentTarget;
                const id = parseInt(button.dataset.id);
                const item = piercingData.find(p => p.id === id);
                if (!item) return;

                const itemIndex = selectedPiercings.findIndex(sel => sel.id === id);
                if (itemIndex > -1) {
                    // Already selected
                } else {
                    selectedPiercings.push(item);
                    button.innerText = "Selected";
                    button.disabled = true;
                }
                updateBookingSummary();
            }

            function updateBookingSummary() {
                if (selectedPiercings.length === 0) {
                    cartSummaryDisplay.innerHTML = '<p>Please select at least one item from the <a class="nav-link" href="#collection">Collection</a>.</p>';
                    cartSummaryHidden.value = ""; // Clear hidden input
                    // Re-add event listener
                    cartSummaryDisplay.querySelector('.nav-link').addEventListener('click', (e) => {
                        e.preventDefault();
                        const href = e.currentTarget.getAttribute('href');
                        const targetElement = document.getElementById(href.substring(1));
                        if (targetElement) {
                            const navbarHeight = document.querySelector('.navbar').offsetHeight;
                            const elementPosition = targetElement.getBoundingClientRect().top + window.scrollY;
                            window.scrollTo({
                                top: elementPosition - navbarHeight,
                                behavior: 'smooth'
                            });
                        }
                    });
                } else {
                    cartSummaryDisplay.innerHTML = "";
                    let summaryText = "";

                    selectedPiercings.forEach(item => {
                        const itemDiv = document.createElement('div');
                        itemDiv.className = 'cart-summary-item';
                        itemDiv.innerHTML = `
                            <span>${item.name}</span>
                            <button type="button" data-id="${item.id}" title="Remove">&times;</button>
                        `;
                        cartSummaryDisplay.appendChild(itemDiv);
                        summaryText += `${item.name}\n`;
                    });

                    cartSummaryHidden.value = summaryText.trim();

                    cartSummaryDisplay.querySelectorAll('.cart-summary-item button').forEach(button => {
                        button.addEventListener('click', handleRemoveItem);
                    });
                }
            }

            function handleRemoveItem(e) {
                const id = parseInt(e.currentTarget.dataset.id);
                selectedPiercings = selectedPiercings.filter(item => item.id !== id);

                const collectionButton = collectionSlider.querySelector(`.btn-select[data-id="${id}"]`);
                if (collectionButton) {
                    collectionButton.innerText = "Select";
                    collectionButton.disabled = false;
                }
                updateBookingSummary();
            }

            // ======== GOOGLE SHEETS FORM SUBMISSION LOGIC ========
            async function handleFormSubmit(e) {
                e.preventDefault();
                const form = e.target;
                const submitButton = form.querySelector('button[type="submit"]');
                const originalButtonText = submitButton.innerText;

                if (form.id === 'booking-form' && selectedPiercings.length === 0) {
                    showAlert("Please select at least one piercing type before booking.");
                    const targetElement = document.getElementById('collection');
                    if (targetElement) {
                        const navbarHeight = document.querySelector('.navbar').offsetHeight;
                        const elementPosition = targetElement.getBoundingClientRect().top + window.scrollY;
                        window.scrollTo({
                            top: elementPosition - navbarHeight,
                            behavior: 'smooth'
                        });
                    }
                    return;
                }

                // This code should now run, since the URL is no longer a placeholder
                if (form.action.includes('YOUR_GOOGLE_SCRIPT_URL')) {
                    showAlert("Form is not active. Please follow the Google Sheets setup instructions.");
                    return;
                }

                submitButton.disabled = true;
                submitButton.innerText = "Submitting...";
                const data = new FormData(form);

                try {
                    const response = await fetch(form.action, {
                        method: "POST",
                        body: data,
                    });
                    const responseData = await response.json();

                    if (responseData.result === "success") {
                        if (form.id === 'booking-form') {
                            if (bookingWrapper && bookingConfirmationTemplate) {
                                bookingWrapper.innerHTML = bookingConfirmationTemplate.querySelector('#booking-confirmation').outerHTML;
                            }
                            selectedPiercings = []; // Clear selection on success
                        } else {
                            showAlert("Message sent successfully!");
                            form.reset();
                        }
                    } else {
                        throw new Error(responseData.message || "Unknown error occurred.");
                    }
                } catch (error) {
                    console.error("Form submission error:", error);
                    showAlert(`There was an error: ${error.message}. Please try again.`);
                } finally {
                    if (form.id !== 'booking-form' || !bookingWrapper.querySelector('#booking-confirmation')) {
                        submitButton.disabled = false;
                        submitButton.innerText = originalButtonText;
                    }
                }
            }

            if (bookingForm) {
                bookingForm.addEventListener("submit", handleFormSubmit);
            }
            if (contactForm) {
                contactForm.addEventListener("submit", handleFormSubmit);
            }

            // ======== INITIALIZE ========
            renderCollection(currentCategory); // Render the default 'ear' category on load
            updateBookingSummary(); // Run once to show the "Please select" message

        });
    </script>
</body>

</html>
