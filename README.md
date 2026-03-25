# m-transport
website


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
        }

        body {
            background-color: var(--primary-bg);
            color: var(--text-light);
            line-height: 1.6;
        }

        /* === HERO SECTION === */
        .hero-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 4rem 1.5rem;
            max-width: 1200px;
            margin: 0 auto;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin-bottom: 3rem;
        }

        .hero-title {
            font-size: 2.5rem;
            font-weight: 800;
            line-height: 1.2;
            margin-bottom: 1rem;
        }

        .hero-subtitle {
            font-size: 1.125rem;
            color: var(--text-muted);
            margin-bottom: 2rem;
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
        }

        .btn-outline {
            background-color: transparent;
            color: var(--text-light);
            border: 2px solid var(--text-muted);
        }

        .btn-outline:hover {
            border-color: var(--text-light);
            background-color: rgba(255, 255, 255, 0.1);
        }

        /* === TRUST SIGNALS === */
        .trust-signals {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 1.5rem;
            font-size: 0.9rem;
            color: var(--text-muted);
            font-weight: 600;
        }

        /* === QUOTE FORM (Lead Engine) === */
        .quote-form-card {
            background-color: var(--form-bg);
            padding: 2rem;
            border-radius: 12px;
            width: 100%;
            max-width: 500px;
            box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.3);
            text-align: left;
        }

        .quote-form-title {
            color: var(--text-dark);
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
            font-weight: 700;
        }

        .quote-form-subtitle {
            color: #718096;
            font-size: 0.9rem;
            margin-bottom: 1.5rem;
        }

        .form-group {
            margin-bottom: 1rem;
        }

        .form-control {
            width: 100%;
            padding: 0.875rem 1rem;
            border: 1px solid var(--input-border);
            border-radius: 6px;
            font-size: 1rem;
            color: var(--text-dark);
            background-color: #F7FAFC;
        }

        .form-control:focus {
            outline: none;
            border-color: var(--accent-color);
            background-color: #FFF;
        }

        select.form-control {
            appearance: none;
            cursor: pointer;
        }

        .btn-submit {
            width: 100%;
            margin-top: 1rem;
        }

        /* === DESKTOP MEDIA QUERIES === */
        @media (min-width: 768px) {
            .hero-container {
                flex-direction: row;
                text-align: left;
                justify-content: space-between;
                align-items: flex-start;
                padding: 6rem 2rem;
            }

            .hero-content {
                max-width: 50%;
                padding-right: 2rem;
            }

            .hero-title {
                font-size: 3.5rem;
            }

            .btn-group {
                flex-direction: row;
            }

            .trust-signals {
                justify-content: flex-start;
            }
        }
    </style>
</head>
<body>

    <main class="hero-container">
        <div class="hero-content">
            <h1 class="hero-title">Move Your Goods Without the Stress.</h1>
            <p class="hero-subtitle">Fast, affordable, and reliable transport for your home or business. Book a truck in minutes and track your delivery in real-time.</p>
            
            <div class="btn-group">
                <a href="#quote" class="btn btn-primary">Get Instant Quote</a>
                <a href="tel:+1234567890" class="btn btn-outline">Call Us Now</a>
            </div>

            <div class="trust-signals">
                <span>⭐ 4.9/5 Average Rating</span>
                <span>🚚 10,000+ Deliveries</span>
                <span>🛡️ Fully Insured</span>
            </div>
        </div>

        <div class="quote-form-card" id="quote">
            <h2 class="quote-form-title">Ready to Move?</h2>
            <p class="quote-form-subtitle">Get your free, no-commitment quote instantly.</p>
            
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
                        <option value="house">House Shifting (Furniture/Boxes)</option>
                        <option value="business">Business / Commercial Goods</option>
                        <option value="single">Single Heavy Item</option>
                        <option value="other">Other</option>
                    </select>
                </div>

                <div class="form-group">
                    <input type="tel" class="form-control" placeholder="Phone Number / WhatsApp" required>
                </div>

                <button type="submit" class="btn btn-primary btn-submit">Get My Instant Quote</button>
            </form>
        </div>
    </main>

</body>
</html>
