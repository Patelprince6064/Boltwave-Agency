<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Boltwave Agency: Helping small businesses grow online effortlessly with expert digital marketing services for startups, freelancers, and local providers.">
    <meta name="keywords" content="digital marketing for small businesses, online growth for startups, SEO for freelancers, web design for local services">
    <title>Boltwave Agency - Grow Your Business Online Effortlessly</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500&family=Montserrat:wght@600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
    <!-- Favicon: simple blue logo as inline SVG -->
    <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Ccircle cx='50' cy='50' r='48' fill='%23007BFF'/%3E%3Ctext x='50' y='58' font-family='Montserrat,Roboto,Arial' font-size='48' fill='%23fff' text-anchor='middle'%3EB%3C/text%3E%3C/svg%3E">
    <style>
        :root{
            --blue: #007BFF;
            --blue-dark: #0056b3;
            --muted: #6c757d;
            --bg: #ffffff;
            --card: #ffffff;
            --radius: 10px;
            --container: 1200px;
        }
        /* Global Styles */
        body { font-family: 'Roboto', sans-serif; margin: 0; padding: 0; color: #222; background: var(--bg); line-height: 1.6; }
        h1, h2, h3 { font-family: 'Montserrat', sans-serif; margin: 0 0 12px 0; }
        a { text-decoration: none; color: var(--blue); }
        .container { max-width: var(--container); margin: 0 auto; padding: 0 20px; }
        .btn { display: inline-block; padding: 12px 24px; background: var(--blue); color: #fff; border-radius: 8px; transition: all 0.25s ease; font-weight: 600; }
        .btn:hover { background: var(--blue-dark); transform: translateY(-2px); }
        .section { padding: 72px 0; }
        .fade-in { opacity: 0; transform: translateY(20px); transition: all 0.6s ease; }
        .fade-in.in-view { opacity: 1; transform: translateY(0); }
        img { max-width: 100%; display: block; }

        /* Header */
        header { position: sticky; top: 0; background: #fff; box-shadow: 0 2px 8px rgba(0,0,0,0.06); z-index: 100; }
        nav { display: flex; justify-content: space-between; align-items: center; padding: 18px 0; }
        nav .logo { font-size: 22px; font-weight: 700; color: var(--blue); }
        nav ul { list-style: none; display: flex; gap: 18px; margin: 0; padding: 0; align-items: center; }
        nav ul li a { color: #222; transition: color 0.2s; font-weight: 500; }
        nav ul li a:hover { color: var(--blue); }
        .nav-right { display: flex; gap: 12px; align-items: center; }

        /* Hero */
        .hero { background: linear-gradient(135deg, rgba(0,123,255,0.06), rgba(0,123,255,0.02)); text-align: left; padding: 100px 0; display: grid; grid-template-columns: 1fr 540px; gap: 40px; align-items: center; }
        .hero h1 { font-size: 44px; color: #0b2540; margin-bottom: 12px; }
        .hero p { font-size: 18px; color: var(--muted); margin-bottom: 20px; }
        .hero-visual { border-radius: var(--radius); overflow: hidden; box-shadow: 0 10px 30px rgba(3,22,60,0.06); }
        .hero-cta { display:flex; gap:12px; align-items:center; }

        /* Services */
        .services { background: #f8fbff; }
        .services .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(260px, 1fr)); gap: 28px; }
        .service { text-align: center; padding: 24px; background: var(--card); border-radius: var(--radius); box-shadow: 0 6px 18px rgba(3,22,60,0.03); transition: transform 0.3s; }
        .service:hover { transform: translateY(-6px); }
        .service i { font-size: 36px; color: var(--blue); margin-bottom: 14px; }

        /* Portfolio/Testimonials */
        .portfolio .grid { display:grid; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr)); gap: 16px; }
        .portfolio img { width:100%; height:180px; object-fit:cover; border-radius: 10px; }
        .testimonial { background: #fff; padding: 18px; border-radius: 10px; margin-top: 18px; box-shadow: 0 6px 18px rgba(3,22,60,0.03); }
        .testimonial p { font-style: italic; color: #2b2b2b; }

        /* Pricing */
        .pricing .grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 24px; }
        .plan { background: #fff; padding: 24px; border-radius: 12px; box-shadow: 0 8px 24px rgba(3,22,60,0.04); }
        .plan h3 { color: var(--blue); margin-bottom: 6px; }
        .plan .price { font-size: 28px; font-weight: 700; margin: 12px 0; }

        /* About */
        .about { text-align: center; }
        .about img { max-width: 260px; border-radius: 50%; margin-bottom: 16px; }

        /* Contact */
        .contact form { max-width: 640px; margin: 0 auto; }
        .contact input, .contact textarea { width: 100%; padding: 12px; margin-bottom: 14px; border: 1px solid #e6eef9; border-radius: 8px; background: #fff; }
        .contact button { width: 100%; }

        /* Footer */
        footer { background: #0b2540; color: #fff; text-align: center; padding: 20px 0; }
        footer a { color: rgba(255,255,255,0.9); }

        /* WhatsApp Floating */
        .whatsapp-fab { position: fixed; right: 18px; bottom: 18px; z-index: 200; background: #25D366; color: #fff; width: 56px; height: 56px; border-radius: 50%; display:flex; align-items:center; justify-content:center; box-shadow: 0 8px 30px rgba(37,211,102,0.15); }
        .whatsapp-fab:hover { transform: translateY(-3px); }

        /* Responsive */
        @media (max-width: 1024px){ .hero{ grid-template-columns: 1fr; padding: 72px 0; } .hero-visual{ order:-1; } }
        @media (max-width: 768px) { nav ul { display: none; } .hero h1 { font-size: 32px; } .grid { grid-template-columns: 1fr; } }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">Boltwave Agency</div>
            <ul>
                <li><a href="#hero">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="nav-right">
                <a class="btn" href="#contact">Book a Free Call</a>
            </div>
        </nav>
    </header>

    <section id="hero" class="hero section fade-in">
        <div class="container">
            <h1>Helping Small Businesses Grow Online — Fast & Predictable</h1>
            <p>We build conversion-first websites, SEO, and social strategies for startups, freelancers, and local businesses. Launch quickly and start getting leads.</p>
            <div class="hero-cta" style="margin-top:18px;">
                <a href="#contact" class="btn">Book a Free Consultation</a>
                <a href="https://wa.me/919328761976" class="btn" style="background:#25D366;border-radius:8px;">Chat on WhatsApp</a>
            </div>
        </div>
        <div class="hero-visual">
            <img src="https://images.unsplash.com/photo-1521791136064-7986c2920216?auto=format&fit=crop&w=1200&q=80" alt="Team working on digital marketing strategy">
        </div>
    </section>

    <section id="services" class="services section fade-in">
        <div class="container">
            <h2>Our Services</h2>
            <p style="color:var(--muted);">Tailored digital solutions to boost your online presence and drive real results for small businesses.</p>
            <div class="grid" style="margin-top:20px;">
                <div class="service">
                    <i class="fas fa-search"></i>
                    <h3>SEO Optimization</h3>
                    <p>Rank higher on Google and attract more customers with our proven SEO strategies designed for startups and freelancers.</p>
                </div>
                <div class="service">
                    <i class="fas fa-code"></i>
                    <h3>Web Design & Development</h3>
                    <p>Beautiful, responsive websites that convert visitors into clients for local service providers.</p>
                </div>
                <div class="service">
                    <i class="fas fa-bullhorn"></i>
                    <h3>Social Media Marketing</h3>
                    <p>Build your brand and engage audiences across platforms like Instagram and Facebook.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="portfolio" class="portfolio section fade-in">
        <div class="container">
            <h2>Portfolio & Testimonials</h2>
            <p style="color:var(--muted);">See how we've helped real businesses like yours achieve online success.</p>
            <div class="grid" style="margin-top:18px;">
                <img src="https://images.unsplash.com/photo-1498050108023-c5249f4df085?auto=format&fit=crop&w=900&q=80" alt="Website design project screenshot">
                <img src="https://images.unsplash.com/photo-1559526324-593bc073d938?auto=format&fit=crop&w=900&q=80" alt="SEO analytics dashboard">
                <img src="https://images.unsplash.com/photo-1492724441997-5dc865305da7?auto=format&fit=crop&w=900&q=80" alt="Social media campaign visuals">
            </div>

            <div class="testimonial">
                <p>"Boltwave Agency transformed our online presence. Leads doubled in just two months!"</p>
                <cite>- Sarah Johnson, Local Fitness Studio</cite>
            </div>
            <div class="testimonial">
                <p>"Affordable and efficient — perfect for freelancers like me."</p>
                <cite>- Mike Chen, Freelance Photographer</cite>
            </div>
        </div>
    </section>

    <section id="pricing" class="pricing section fade-in">
        <div class="container">
            <h2>Pricing Plans</h2>
            <p style="color:var(--muted);">Flexible packages to fit your budget and goals. Start small, grow big.</p>
            <div class="grid" style="margin-top:20px;">
                <div class="plan">
                    <h3>Starter</h3>
                    <div class="price">$499/month</div>
                    <p>Basic SEO and social media setup for new startups.</p>
                    <a href="#contact" class="btn">Get Started Today</a>
                </div>
                <div class="plan">
                    <h3>Growth</h3>
                    <div class="price">$999/month</div>
                    <p>Full web design, advanced SEO, and marketing campaigns.</p>
                    <a href="#contact" class="btn">Get Started Today</a>
                </div>
                <div class="plan">
                    <h3>Premium</h3>
                    <div class="price">$1,999/month</div>
                    <p>Comprehensive digital strategy with ongoing support.</p>
                    <a href="#contact" class="btn">Get Started Today</a>
                </div>
            </div>
        </div>
    </section>

    <section id="about" class="about section fade-in">
        <div class="container">
            <h2>About Us</h2>
            <img src="https://images.unsplash.com/photo-1522071820081-009f0129c71c?auto=format&fit=crop&w=800&q=80" alt="Boltwave team">
            <p>At Boltwave Agency, we're a passionate team of digital experts dedicated to helping small businesses, startups, and freelancers thrive online. With over 5 years of experience, we've empowered clients to reach new heights.</p>
            <p>Our mission is simple: Make digital marketing accessible and effective for everyone, no matter your size.</p>
        </div>
    </section>

    <section id="contact" class="contact section fade-in">
        <div class="container">
            <h2>Contact Us</h2>
            <p style="color:var(--muted);">Ready to grow? Let's chat about your needs.</p>
            <form action="https://formspree.io/pp50646464@gmail.com" method="POST">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" placeholder="Tell us about your business goals..." rows="5" required></textarea>
                <!-- Optional: help the buyer identify the lead source -->
                <input type="hidden" name="_subject" value="New lead from Boltwave Agency website">
                <button type="submit" class="btn">Contact Us Now</button>
            </form>
            <p style="text-align:center;margin-top:12px;color:var(--muted);">Or email us directly at <a href="mailto:pp50646464@gmail.com">pp50646464@gmail.com</a></p>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2025 Boltwave Agency. All rights reserved. | Contact: <a href="mailto:pp50646464@gmail.com">pp50646464@gmail.com</a></p>
        </div>
    </footer>

    <!-- WhatsApp floating button -->
    <a class="whatsapp-fab" href="https://wa.me/919328761976" aria-label="Chat on WhatsApp" target="_blank" rel="noopener noreferrer">
        <i class="fab fa-whatsapp" style="font-size:20px;color:#fff"></i>
    </a>

    <script>
        // Simple fade-in animation on scroll
        const elements = document.querySelectorAll('.fade-in');
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('in-view');
                }
            });
        });
        elements.forEach(el => observer.observe(el));
    </script>
</body>
</html>
