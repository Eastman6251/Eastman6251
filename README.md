<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Eastman | Senior Full Stack Software Engineer</title>
    <meta name="description" content="Senior Full Stack Software Engineer with 7+ years of experience in scalable web applications, AI/ML systems, and modern cloud architecture.">
    
    <!-- Using Google Fonts for a modern tech look -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
    
    <!-- Remix Icons for UI elements -->
    <link href="https://cdn.jsdelivr.net/npm/remixicon@3.5.0/fonts/remixicon.css" rel="stylesheet">

    <style>
        :root {
            /* Color Palette - Dark Modern Theme */
            --bg-body: #0d1117;
            --bg-card: #161b22;
            --bg-card-hover: #1f262e;
            --text-main: #c9d1d9;
            --text-heading: #f0f6fc;
            --text-muted: #8b949e;
            --accent-primary: #58a6ff; /* GitHub Blue */
            --accent-secondary: #238636; /* GitHub Green */
            --accent-highlight: #d29922; /* Gold */
            --border-color: #30363d;
            
            /* Spacing & Layout */
            --container-width: 1100px;
            --radius-md: 8px;
            --radius-lg: 12px;
            --transition-speed: 0.2s;
        }

        /* Reset & Base Styles */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'Inter', -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
            background-color: var(--bg-body);
            color: var(--text-main);
            line-height: 1.6;
            -webkit-font-smoothing: antialiased;
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: color var(--transition-speed);
        }

        ul {
            list-style: none;
        }

        /* Layout Utilities */
        .container {
            max-width: var(--container-width);
            margin: 0 auto;
            padding: 2rem 1.5rem;
        }

        .section-title {
            font-size: 1.5rem;
            color: var(--text-heading);
            margin-bottom: 1.5rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            border-bottom: 1px solid var(--border-color);
            padding-bottom: 0.5rem;
        }

        .section-title i {
            color: var(--accent-primary);
        }

        /* Header / Hero Section */
        header {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            padding: 3rem 0;
            border-bottom: 1px solid var(--border-color);
            margin-bottom: 3rem;
        }

        .avatar {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            border: 3px solid var(--accent-primary);
            margin-bottom: 1.5rem;
            object-fit: cover;
            background-color: var(--bg-card);
        }

        h1 {
            font-size: 2.5rem;
            color: var(--text-heading);
            margin-bottom: 0.5rem;
            font-weight: 700;
        }

        .role {
            font-size: 1.25rem;
            color: var(--accent-primary);
            margin-bottom: 1rem;
            font-weight: 500;
        }

        .bio {
            max-width: 700px;
            color: var(--text-muted);
            margin-bottom: 2rem;
            font-size: 1.1rem;
        }

        .social-links {
            display: flex;
            gap: 1.5rem;
            justify-content: center;
        }

        .social-btn {
            background-color: var(--bg-card);
            border: 1px solid var(--border-color);
            padding: 0.5rem 1rem;
            border-radius: var(--radius-md);
            display: flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 0.9rem;
            transition: transform 0.2s, border-color 0.2s;
        }

        .social-btn:hover {
            transform: translateY(-2px);
            border-color: var(--accent-primary);
            color: var(--text-heading);
        }

        /* About Section */
        .about-grid {
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 2rem;
            margin-bottom: 4rem;
        }

        .card {
            background-color: var(--bg-card);
            border: 1px solid var(--border-color);
            border-radius: var(--radius-lg);
            padding: 1.5rem;
            transition: background-color 0.3s ease;
        }
        
        .card:hover {
            background-color: var(--bg-card-hover);
        }

        .card-content p {
            margin-bottom: 1rem;
            color: var(--text-main);
        }

        .stats-list li {
            display: flex;
            align-items: flex-start;
            gap: 0.75rem;
            margin-bottom: 1rem;
            color: var(--text-muted);
            font-size: 0.95rem;
        }

        .stats-list i {
            color: var(--accent-highlight);
            margin-top: 3px;
        }

        /* Skills Section */
        .skills-container {
            margin-bottom: 4rem;
        }

        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 1.5rem;
        }

        .skill-category h3 {
            color: var(--text-heading);
            margin-bottom: 1rem;
            font-size: 1.1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .skill-category h3 span {
            font-size: 0.8rem;
            background: rgba(88, 166, 255, 0.15);
            color: var(--accent-primary);
            padding: 2px 8px;
            border-radius: 12px;
        }

        .tech-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .tech-tag {
            background-color: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--border-color);
            padding: 0.25rem 0.75rem;
            border-radius: 20px;
            font-size: 0.85rem;
            font-family: 'JetBrains Mono', monospace;
            color: var(--text-main);
            transition: all 0.2s;
            cursor: default;
        }

        .tech-tag:hover {
            border-color: var(--accent-primary);
            color: var(--accent-primary);
            background-color: rgba(88, 166, 255, 0.1);
        }

        /* Experience/Timeline Preview */
        .experience-preview {
            margin-bottom: 4rem;
        }
        
        .exp-item {
            border-left: 2px solid var(--border-color);
            padding-left: 1.5rem;
            margin-bottom: 2rem;
            position: relative;
        }

        .exp-item::before {
            content: '';
            position: absolute;
            left: -6px;
            top: 6px;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            background-color: var(--accent-primary);
        }

        .exp-title {
            font-size: 1.2rem;
            color: var(--text-heading);
            font-weight: 600;
        }

        .exp-meta {
            color: var(--text-muted);
            font-size: 0.9rem;
            margin-bottom: 0.5rem;
            font-family: 'JetBrains Mono', monospace;
        }

        /* Footer */
        footer {
            text-align: center;
            padding: 3rem 0;
            border-top: 1px solid var(--border-color);
            color: var(--text-muted);
            font-size: 0.9rem;
        }
        
        .footer-contact {
            margin-bottom: 1rem;
            font-size: 1.1rem;
        }
        
        .footer-contact a {
            color: var(--text-heading);
            font-weight: 600;
        }

        .footer-contact a:hover {
            color: var(--accent-primary);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .about-grid {
                grid-template-columns: 1fr;
            }
            
            h1 {
                font-size: 2rem;
            }
            
            .role {
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>

    <div class="container">
        
        <!-- Header Section -->
        <header>
            <!-- Using a high-quality placeholder avatar. Replace with your actual photo -->
            <img src="https://picsum.photos/seed/eastman/200/200" alt="Eastman Avatar" class="avatar">
            
            <h1>Eastman</h1>
            <p class="role">Senior Full Stack Software Engineer</p>
            
            <p class="bio">
                7+ Years of Experience • Scalable Architecture • AI/ML Integration • Full Lifecycle Development
            </p>

            <div class="social-links">
                <a href="https://github.com/daijro" target="_blank" class="social-btn">
                    <i class="ri-github-fill"></i> GitHub
                </a>
                <a href="mailto:daijro.dev@gmail.com" class="social-btn">
                    <i class="ri-mail-send-fill"></i> Email Me
                </a>
                <a href="#" class="social-btn">
                    <i class="ri-linkedin-fill"></i> LinkedIn
                </a>
            </div>
        </header>

        <!-- Main Content -->
        <main>

            <!-- Professional Summary -->
            <section id="about" class="about-grid">
                <div class="card">
                    <h2 class="section-title"><i class="ri-user-star-line"></i> Professional Profile</h2>
                    <div class="card-content">
                        <p>
                            I am a Senior Full Stack Software Engineer with over 7 years of experience designing and delivering scalable, high-performance web applications. My proven expertise spans the entire development lifecycle, including complex frontend architectures, robust backend services, database optimization, and seamless API integrations.
                        </p>
                        <p>
                            I have extensive experience working with <strong>startups, SMEs, and enterprise teams</strong>, building reliable and maintainable solutions that strictly align with business goals and user needs. As a strong collaborator, I work closely with product managers, designers, and engineers to translate abstract requirements into production-ready systems.
                        </p>
                        <p>
                            Highly effective in independent and distributed team environments, I apply modern development practices to deliver clean, efficient, and scalable code.
                        </p>
                    </div>
                </div>

                <div class="card">
                    <h2 class="section-title"><i class="ri-lightbulb-flash-line"></i> Key Focus Areas</h2>
                    <ul class="stats-list">
                        <li><i class="ri-stack-line"></i> Full-Stack Web Architecture</li>
                        <li><i class="ri-brain-line"></i> AI/ML Systems Design & Integration</li>
                        <li><i class="ri-server-line"></i> Cloud Infrastructure (AWS, Vercel)</li>
                        <li><i class="ri-shopping-cart-line"></i> E-Commerce & CMS Solutions</li>
                        <li><i class="ri-git-merge-line"></i> Agile & CI/CD Best Practices</li>
                        <li><i class="ri-shield-check-line"></i> Scalability & Performance Tuning</li>
                    </ul>
                </div>
            </section>

            <!-- Technical Skills Grid -->
            <section id="skills" class="skills-container">
                <h2 class="section-title"><i class="ri-terminal-box-line"></i> Technical Stack</h2>
                
                <div class="category-grid">
                    
                    <!-- Frontend -->
                    <div class="card skill-category">
                        <h3>Frontend Architecture <span>Modern UI</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">React.js</span>
                            <span class="tech-tag">Next.js</span>
                            <span class="tech-tag">Nuxt.js</span>
                            <span class="tech-tag">Vue.js</span>
                            <span class="tech-tag">Angular.js</span>
                            <span class="tech-tag">TypeScript (TS)</span>
                            <span class="tech-tag">JavaScript (JS)</span>
                            <span class="tech-tag">GraphQL API</span>
                            <span class="tech-tag">RESTful API</span>
                        </div>
                    </div>

                    <!-- Backend -->
                    <div class="card skill-category">
                        <h3>Backend Development <span>Server Logic</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">PHP</span>
                            <span class="tech-tag">Symfony</span>
                            <span class="tech-tag">Laravel</span>
                            <span class="tech-tag">Python</span>
                            <span class="tech-tag">Django</span>
                            <span class="tech-tag">Flask</span>
                            <span class="tech-tag">FASTAPI</span>
                            <span class="tech-tag">Node.js</span>
                            <span class="tech-tag">Nest.js</span>
                            <span class="tech-tag">Express.js</span>
                        </div>
                    </div>

                    <!-- AI & Data -->
                    <div class="card skill-category">
                        <h3>AI / Machine Learning <span>Intelligence</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">OpenAI</span>
                            <span class="tech-tag">TensorFlow</span>
                            <span class="tech-tag">PyTorch</span>
                            <span class="tech-tag">Pandas</span>
                            <span class="tech-tag">Pinecone</span>
                            <span class="tech-tag">Chatbot Dev</span>
                            <span class="tech-tag">AI System Design</span>
                        </div>
                    </div>

                    <!-- Database -->
                    <div class="card skill-category">
                        <h3>Data & Storage <span>Persistence</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">PostgreSQL</span>
                            <span class="tech-tag">MySQL</span>
                            <span class="tech-tag">MariaDB</span>
                            <span class="tech-tag">MongoDB</span>
                            <span class="tech-tag">DynamoDB</span>
                            <span class="tech-tag">GraphQL</span>
                        </div>
                    </div>

                    <!-- DevOps -->
                    <div class="card skill-category">
                        <h3>DevOps & Cloud <span>Infrastructure</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">AWS</span>
                            <span class="tech-tag">Vercel</span>
                            <span class="tech-tag">Netlify</span>
                            <span class="tech-tag">Docker</span>
                            <span class="tech-tag">CI/CD</span>
                            <span class="tech-tag">Git / GitHub</span>
                            <span class="tech-tag">Jira</span>
                            <span class="tech-tag">Agile / Scrum</span>
                        </div>
                    </div>

                    <!-- CMS / Other -->
                    <div class="card skill-category">
                        <h3>CMS & E-Commerce <span>Platforms</span></h3>
                        <div class="tech-tags">
                            <span class="tech-tag">Shopify</span>
                            <span class="tech-tag">WordPress</span>
                            <span class="tech-tag">WooCommerce</span>
                            <span class="tech-tag">Joomla</span>
                            <span class="tech-tag">Drupal</span>
                            <span class="tech-tag">Divi</span>
                            <span class="tech-tag">Elementor</span>
                            <span class="tech-tag">Squarespace</span>
                        </div>
                    </div>

                </div>
            </section>

            <!-- Experience Summary -->
            <section class="experience-preview">
                <h2 class="section-title"><i class="ri-briefcase-4-line"></i> Professional Experience</h2>
                
                <div class="exp-item">
                    <div class="exp-title">Senior Full Stack Engineer</div>
                    <div class="exp-meta">Startups, SMEs, & Enterprise Teams | Present</div>
                    <p class="card-content">
                        Leading the design and delivery of scalable web applications. Specializing in bridging the gap between complex AI/ML backend systems and user-friendly frontend interfaces. Implementing robust CI/CD pipelines and cloud infrastructure to ensure high availability.
                    </p>
                </div>

                <div class="exp-item">
                    <div class="exp-title">Full Stack Developer & Architect</div>
                    <div class="exp-meta">Freelance & Consulting | Previous Years</div>
                    <p class="card-content">
                        Developed custom solutions using PHP frameworks (Laravel, Symfony) and Python ecosystems (Django, FastAPI). Delivered numerous e-commerce platforms on Shopify and WordPress, alongside custom SaaS products built on React and Node.js.
                    </p>
                </div>
            </section>

        </main>

        <!-- Footer -->
        <footer>
            <div class="footer-contact">
                Ready to collaborate? <a href="mailto:daijro.dev@gmail.com">Get in touch</a>.
            </div>
            <p>&copy; 2025 Eastman. Built with clean, semantic HTML & CSS.</p>
        </footer>

    </div>

</body>
</html>
