#website on M transport

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>M Transport | Fast & Reliable</title>
    <style>
        /* === BASE STYLES & VARIABLES === */
        :root {
            --primary-bg: #0B132B; /* Dark Navy */
            --accent-color: #FF9F1C; /* Vibrant Orange */
            --accent-hover: #F48C06;
            --text-light: #FFFFFF;
            --text-muted: #A0AEC0;
            --form-bg: #FFFFFF;
            --input-border: #E2E8F0;
            --text-dark: #1A202C;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: var(--primary-bg);
            color: var(--text-light);
            line-height: 1.6;
        }

        /* === NAVIGATION === */
        header {
            width: 100%;
            padding: 1.5rem 1.5rem;
            display: flex;
            flex-direction: column;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            gap: 1rem;
        }

        .logo {
            font-size: 1.75rem;
            font-weight: 800;
            color: var(--accent-color);
            text-decoration: none;
            letter-spacing: -1px;
        }

        .logo span {
            color: var(--text-light);
        }

        .contact-fast-links {
            display: flex;
            gap: 0.8rem;
            flex-wrap: wrap;
            justify-content: center;
        }

        .contact-link {
            color: var(--text-light);
            text-decoration: none;
            font-size: 0.85rem;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 6px;
            padding: 0.6rem 1rem;
            border-radius: 50px;
            background: rgba(255, 255, 255, 0.1);
            transition: 0.3s;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }

        .contact-link:hover {
            background: var(--accent-color);
            color: #000;
            border-color: var(--accent-color);
        }

        /* === HERO SECTION === */
        .hero-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 2rem 1.5rem 4rem;
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin-bottom: 3rem;
        }

        .hero-title {
            font-size: 2.8rem;
            font-weight: 800;
            line-height: 1.1;
            margin-bottom: 1.5rem;
        }

        .hero-subtitle {
            font-size: 1.125rem;
            color: var(--text-muted);
            margin-bottom: 2.5rem;
        }

        /* === BUTTONS === */
        .btn-group {
            display: flex;
            flex-direction: column;
            gap: 1rem;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            padding: 1rem 2rem;
            font-size: 1.125rem;
            font-weight: 700;
            border-radius: 8px;
            text-decoration: none;
            text-align: center;
            transition: all 0.3s ease;
            cursor: pointer;
            border: none;
        }

        .btn-primary {
            background-color: var(--accent-color);
            color: #000;
        }

        .btn-primary:hover {
            background-color: var(--accent-hover);
            transform: translateY(-2px);
            box-shadow: 0 10px 15px -3px rgba(255, 159, 28, 0.4);
        }

        .btn-outline {
            background-color: transparent;
            color: var(--text-light);
            border: 2px solid var(--text-muted);
        }

        .btn-outline:hover {
            border-color: var(--text-light);
            background: rgba(255, 255, 255, 0.05);
        }

        /* === QUOTE FORM === */
        .quote-form-card {
            background-color: var(--form-bg);
            padding: 2.5rem 2rem;
            border-radius: 16px;
            width: 100%;
            max-width: 500px;
            box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5);
            text-align: left;
            border-top: 8px solid var(--accent-color);
        }

        .quote-form-title {
            color: var(--text-dark);
            font-size: 1.6rem;
            margin-bottom: 0.5rem;
            font-weight: 800;
        }

        .form-group {
            margin-bottom: 1.2rem;
        }

        .form-control {
            width: 100%;
            padding: 1rem;
            border: 1px solid var(--input-border);
            border-radius: 8px;
            font-size: 1rem;
            color: var(--text-dark);
            background-color: #F8FAFC;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--accent-color);
            background-color: #FFF;
            box-shadow: 0 0 0 3px rgba(255, 159, 28, 0.1);
        }

        .form-footer-contact {
            margin-top: 1.5rem;
            padding-top: 1.2rem;
            border-top: 1px solid #edf2f7;
            font-size: 0.9rem;
            color: #4A5568;
            text-align: center;
        }

        .footer-link {
            color: var(--accent-hover);
            text-decoration: none;
            font-weight: 700;
        }

        /* === DESKTOP MEDIA QUERIES === */
        @media (min-width: 768px) {
            header {
                flex-direction: row;
                justify-content: space-between;
                padding: 2.5rem 2rem;
            }

            .hero-container {
                flex-direction: row;
                text-align: left;
                justify-content: space-between;
                align-items: flex-start;
                padding: 5rem 2rem 8rem;
            }

            .hero-content {
                max-width: 50%;
                padding-right: 3rem;
                margin-top: 2rem;
            }

            .hero-title {
                font-size: 3.8rem;
            }

            .btn-group {
                flex-direction: row;
            }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">M <span>Transport</span></a>
        
        <div class="contact-fast-links">
            <a href="mailto:mahmudul.bge38@gmail.com" class="contact-link">
                ✉️ Email Me
            </a>
            <a href="https://wa.me/8801738958981?text=Hello,%20I%20am%20interested%20in%20M%20Transport%20services." class="contact-link" target="_blank">
                💬 WhatsApp
            </a>
            <a href="tel:+8801738958981" class="contact-link">
                📞 Call Now
            </a>
        </div>
    </header>

    <main class="hero-container">
        <div class="hero-content">
            <h1 class="hero-title"> Move Your Goods Stress-Free. </h1>
            <p class="hero-subtitle">Fast, affordable, and reliable transport for your home or business. Book a truck in minutes and track your delivery in real-time.</p>
            
            <div class="btn-group">
                <a href="#quote" class="btn btn-primary">Get Instant Quote</a>
                <a href="https://wa.me/8801738958981?text=Hi,%20I%20need%20a%20transport%20quote." class="btn btn-outline" target="_blank">Chat on WhatsApp</a>
            </div>
        </div>

        <div class="quote-form-card" id="quote">
            <h2 class="quote-form-title">Ready to Move?</h2>
            <p style="color: #718096; font-size: 0.95rem; margin-bottom: 1.5rem;">Fill in the details for a quick price estimate.</p>
            
            <form action="#" method="POST">
                <div class="form-group">
                    <input type="text" class="form-control" placeholder="Pickup Location" required>
                </div>
                
                <div class="form-group">
                    <input type="text" class="form-control" placeholder="Drop-off Location" required>
                </div>
                
                <div class="form-group">
                    <select class="form-control" required>
                        <option value="" disabled selected>Type of Goods</option>
                        <option value="house">House Shifting</option>
                        <option value="business">Business / Commercial</option>
                        <option value="single">Single Heavy Item</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <div class="form-group">
                    <input type="tel" class="form-control" placeholder="Your Phone Number" required>
                </div>

                <button type="submit" class="btn btn-primary" style="width: 100%; margin-top: 10px; font-size: 1.2rem;">Calculate My Quote</button>
            </form>

            <div class="form-footer-contact">
                Need help? <br>
                <a href="https://wa.me/8801738958981" class="footer-link">WhatsApp: 01738958981</a> <br>
                <a href="mailto:mahmudul.bge38@gmail.com" class="footer-link">mahmudul.bge38@gmail.com</a>
            </div>
        </div>
    </main>

</body>
</html>
