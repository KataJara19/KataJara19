<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Katalina Jaramillo Loján | Portfolio</title>
    <style>
        /* Variables y Reset */
        :root {
            --bg-color: #0a0f16;
            --surface-color: #131b26;
            --primary-color: #00d2ff;
            --secondary-color: #3a7bd5;
            --text-main: #e2e8f0;
            --text-muted: #94a3b8;
            --font-main: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background-color: var(--bg-color);
            color: var(--text-main);
            font-family: var(--font-main);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Utilidad de Transiciones Elegantes (Fade In en Scroll) */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: opacity 0.8s ease-out, transform 0.8s ease-out;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Header / Hero Section */
        header {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 2rem;
            background: radial-gradient(circle at top, #131b26 0%, #0a0f16 100%);
        }

        h1 {
            font-size: 4rem;
            margin-bottom: 0.5rem;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        h2 {
            font-size: 1.5rem;
            color: var(--text-muted);
            font-weight: 400;
            margin-bottom: 2rem;
        }

        /* Container General */
        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 5rem 2rem;
        }

        .section-title {
            font-size: 2.5rem;
            margin-bottom: 3rem;
            text-align: center;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 60px;
            height: 4px;
            background: var(--primary-color);
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }

        /* About Section */
        .about-text {
            font-size: 1.2rem;
            text-align: center;
            max-width: 800px;
            margin: 0 auto;
            color: var(--text-muted);
        }

        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }

        .project-card {
            background-color: var(--surface-color);
            padding: 2rem;
            border-radius: 12px;
            border: 1px solid rgba(255, 255, 255, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease, border-color 0.3s ease;
        }

        .project-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 30px rgba(0, 210, 255, 0.1);
            border-color: var(--primary-color);
        }

        .project-card h3 {
            color: var(--primary-color);
            margin-bottom: 1rem;
            font-size: 1.4rem;
        }

        .project-card p {
            color: var(--text-muted);
            margin-bottom: 1.5rem;
            font-size: 0.95rem;
        }

        .tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tag {
            background: rgba(0, 210, 255, 0.1);
            color: var(--primary-color);
            padding: 0.3rem 0.8rem;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        /* Footer & Contact */
        footer {
            text-align: center;
            padding: 4rem 2rem;
            background-color: var(--surface-color);
        }

        .contact-links a {
            display: inline-block;
            margin: 0 1rem;
            color: var(--text-main);
            text-decoration: none;
            font-size: 1.2rem;
            transition: color 0.3s ease;
        }

        .contact-links a:hover {
            color: var(--primary-color);
        }
    </style>
</head>
<body>

    <!-- HERO SECTION -->
    <header class="fade-in">
        <h1>Katalina Jaramillo</h1>
        <h2>Full-Stack Developer & Cybersecurity Enthusiast</h2>
        <p style="color: var(--text-muted); font-size: 1.1rem; margin-top: -1rem;">Systems Engineering Student | AWS Student Builder Group Coordinator</p>
    </header>

    <!-- ABOUT SECTION -->
    <section class="container fade-in">
        <h2 class="section-title">About Me</h2>
        <p class="about-text">
            Dynamic 4th-semester Systems Engineering student at Universidad Internacional del Ecuador. 
            Passionate about merging secure cloud infrastructure, scalable backend systems, and modern user interfaces. 
            Actively building robust applications and simulating secure networking environments to bridge the gap 
            between development and cybersecurity.
        </p>
    </section>

    <!-- PROJECTS SECTION -->
    <section class="container">
        <h2 class="section-title fade-in">Featured Projects</h2>
        <div class="projects-grid">
            
            <!-- Project 1 -->
            <div class="project-card fade-in">
                <h3>TiendaEsmeralda (E-Commerce)</h3>
                <p>Architected a complete web store environment featuring secure user query workflows, structured database management, and robust transactional logic.</p>
                <div class="tags">
                    <span class="tag">Full-Stack</span>
                    <span class="tag">Databases</span>
                </div>
            </div>

            <!-- Project 2 -->
            <div class="project-card fade-in">
                <h3>Media Streaming Clone</h3>
                <p>Integration of modern frontend components interacting with custom backend architectures (Api-con-frontend & Replicación-YouTube). Managed state and optimized media fetching.</p>
                <div class="tags">
                    <span class="tag">React</span>
                    <span class="tag">FastAPI</span>
                </div>
            </div>

            <!-- Project 3 -->
            <div class="project-card fade-in">
                <h3>Security & Auth APIs</h3>
                <p>Engineered specialized backend endpoints (Ciberapi & API-SEGURIDAD) focused on robust authentication validation, secure data exchange protocols, and vulnerability testing.</p>
                <div class="tags">
                    <span class="tag">Cybersecurity</span>
                    <span class="tag">API</span>
                </div>
            </div>

            <!-- Project 4 -->
            <div class="project-card fade-in">
                <h3>Infrastructure & Threat Labs</h3>
                <p>Deployed multi-node networks (VMware, AlmaLinux, MikroTik). Conducted threat intelligence, script-based data encryption (XOR), and analyzed malware behavior (VIRUS).</p>
                <div class="tags">
                    <span class="tag">Networking</span>
                    <span class="tag">InfoSec</span>
                </div>
            </div>

        </div>
    </section>

    <!-- FOOTER / CONTACT -->
    <footer class="fade-in">
        <h2 style="color: var(--text-main); margin-bottom: 2rem;">Let's Connect</h2>
        <div class="contact-links">
            <a href="https://github.com/KataJara19" target="_blank">GitHub (@KataJara19)</a>
            <a href="#">Universidad Internacional del Ecuador</a>
        </div>
        <p style="margin-top: 3rem; color: var(--text-muted); font-size: 0.9rem;">
            Designed & Built by Katalina Jaramillo
        </p>
    </footer>

    <!-- JS para las transiciones elegantes -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.15 // El elemento aparecerá cuando el 15% sea visible
            };

            const observer = new IntersectionObserver((entries, observer) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                        observer.unobserve(entry.target); // Dejar de observar una vez que aparece
                    }
                });
            }, observerOptions);

            const elements = document.querySelectorAll('.fade-in');
            elements.forEach(el => observer.observe(el));
        });
    </script>
</body>
</html>
