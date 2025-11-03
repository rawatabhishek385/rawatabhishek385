<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Abhishek Rawat | GitHub Profile</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=JetBrains+Mono:wght@300;400;500&display=swap');
        
        :root {
            --primary: #6C63FF;
            --secondary: #4A44C6;
            --dark: #1A1A2E;
            --darker: #0F0F1B;
            --light: #F5F5F7;
            --accent: #FF6584;
            --success: #2ECC71;
            --warning: #F39C12;
            --gradient: linear-gradient(135deg, var(--primary), var(--secondary));
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            background-color: var(--darker);
            color: var(--light);
            line-height: 1.6;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            padding: 80px 0 40px;
            text-align: center;
            background: linear-gradient(135deg, var(--dark), var(--darker));
            position: relative;
            overflow: hidden;
        }
        
        .header-content {
            position: relative;
            z-index: 2;
        }
        
        .profile-img {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 4px solid var(--primary);
            margin: 0 auto 20px;
            background: var(--gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            color: white;
        }
        
        h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            font-weight: 700;
        }
        
        .tagline {
            font-size: 1.2rem;
            color: #aaa;
            margin-bottom: 20px;
        }
        
        .animated-badge {
            display: inline-block;
            background: var(--gradient);
            color: white;
            padding: 8px 16px;
            border-radius: 30px;
            font-size: 0.9rem;
            margin: 5px;
            animation: float 3s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        /* Section Styles */
        section {
            padding: 60px 0;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }
        
        h2 {
            font-size: 2rem;
            margin-bottom: 30px;
            position: relative;
            display: inline-block;
        }
        
        h2:after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 0;
            width: 60px;
            height: 4px;
            background: var(--gradient);
            border-radius: 2px;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }
        
        /* About Section */
        .about-content {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            align-items: center;
        }
        
        .about-text {
            flex: 1;
            min-width: 300px;
        }
        
        .about-highlights {
            flex: 1;
            min-width: 300px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
        }
        
        .highlight-card {
            background: rgba(255,255,255,0.05);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .highlight-card:hover {
            transform: translateY(-5px);
            background: rgba(255,255,255,0.08);
        }
        
        .highlight-card i {
            font-size: 2rem;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .skill-category {
            background: rgba(255,255,255,0.05);
            padding: 25px;
            border-radius: 10px;
        }
        
        .skill-category h3 {
            margin-bottom: 20px;
            color: var(--primary);
            font-size: 1.3rem;
        }
        
        .skill-items {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .skill-item {
            background: var(--gradient);
            padding: 8px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }
        
        /* Stats Section */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .stat-card {
            background: rgba(255,255,255,0.05);
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            background: rgba(255,255,255,0.08);
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            background: var(--gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 10px;
        }
        
        /* Contact Section */
        .contact-container {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            justify-content: center;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 15px;
            background: rgba(255,255,255,0.05);
            padding: 15px 25px;
            border-radius: 10px;
            transition: transform 0.3s ease;
        }
        
        .contact-item:hover {
            transform: translateY(-5px);
            background: rgba(255,255,255,0.08);
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: var(--gradient);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
        }
        
        /* Footer */
        footer {
            padding: 40px 0;
            text-align: center;
            background: rgba(0,0,0,0.3);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }
        
        .social-link {
            width: 50px;
            height: 50px;
            border-radius: 50%;
            background: rgba(255,255,255,0.05);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.5rem;
            transition: all 0.3s ease;
        }
        
        .social-link:hover {
            background: var(--gradient);
            transform: translateY(-5px);
        }
        
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 1s ease forwards;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            h1 {
                font-size: 2rem;
            }
            
            section {
                padding: 40px 0;
            }
            
            .about-content, .contact-container {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <div class="header-content">
                <div class="profile-img">
                    <i class="fas fa-user"></i>
                </div>
                <h1>Abhishek Rawat</h1>
                <p class="tagline">Full Stack Developer | Android Enthusiast</p>
                <div>
                    <span class="animated-badge">MCA Graduate</span>
                    <span class="animated-badge" style="animation-delay: 0.5s;">Web Developer</span>
                    <span class="animated-badge" style="animation-delay: 1s;">Android Developer</span>
                </div>
            </div>
        </div>
    </header>

    <section id="about">
        <div class="container">
            <h2 class="section-title">About Me</h2>
            <div class="about-content">
                <div class="about-text">
                    <p>I'm a passionate developer with a Master's in Computer Applications, specializing in Full Stack Web Development and Android Development. I'm constantly learning new technologies and improving my skills to build innovative solutions.</p>
                    <br>
                    <p>My journey in technology started with a curiosity about how things work, which evolved into a passion for creating digital experiences that make a difference. I believe in writing clean, efficient code and always strive to stay updated with the latest industry trends.</p>
                </div>
                <div class="about-highlights">
                    <div class="highlight-card fade-in">
                        <i class="fas fa-graduation-cap"></i>
                        <h3>Education</h3>
                        <p>Master of Computer Applications</p>
                    </div>
                    <div class="highlight-card fade-in" style="animation-delay: 0.2s;">
                        <i class="fas fa-laptop-code"></i>
                        <h3>Focus</h3>
                        <p>Full Stack & Android Development</p>
                    </div>
                    <div class="highlight-card fade-in" style="animation-delay: 0.4s;">
                        <i class="fas fa-rocket"></i>
                        <h3>Passion</h3>
                        <p>Creating Impactful Solutions</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="skills">
        <div class="container">
            <h2 class="section-title">Technical Skills</h2>
            <div class="skills-container">
                <div class="skill-category fade-in">
                    <h3><i class="fas fa-code"></i> Frontend Development</h3>
                    <div class="skill-items">
                        <div class="skill-item">HTML</div>
                        <div class="skill-item">CSS</div>
                        <div class="skill-item">JavaScript</div>
                        <div class="skill-item">React</div>
                    </div>
                </div>
                <div class="skill-category fade-in" style="animation-delay: 0.2s;">
                    <h3><i class="fas fa-mobile-alt"></i> Mobile Development</h3>
                    <div class="skill-items">
                        <div class="skill-item">Android</div>
                        <div class="skill-item">Java</div>
                    </div>
                </div>
                <div class="skill-category fade-in" style="animation-delay: 0.4s;">
                    <h3><i class="fas fa-database"></i> Database & Backend</h3>
                    <div class="skill-items">
                        <div class="skill-item">MySQL</div>
                        <div class="skill-item">Oracle</div>
                        <div class="skill-item">Node.js</div>
                        <div class="skill-item">MongoDB</div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="stats">
        <div class="container">
            <h2 class="section-title">GitHub Statistics</h2>
            <div class="stats-container">
                <div class="stat-card fade-in">
                    <div class="stat-number">50+</div>
                    <p>Projects Completed</p>
                </div>
                <div class="stat-card fade-in" style="animation-delay: 0.2s;">
                    <div class="stat-number">1000+</div>
                    <p>Code Commits</p>
                </div>
                <div class="stat-card fade-in" style="animation-delay: 0.4s;">
                    <div class="stat-number">15+</div>
                    <p>Technologies Used</p>
                </div>
                <div class="stat-card fade-in" style="animation-delay: 0.6s;">
                    <div class="stat-number">2+</div>
                    <p>Years of Experience</p>
                </div>
            </div>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2 class="section-title">Get In Touch</h2>
            <div class="contact-container">
                <div class="contact-item fade-in">
                    <div class="contact-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <div>
                        <h3>Email</h3>
                        <p>rawatabhishek385@gmail.com</p>
                    </div>
                </div>
                <div class="contact-item fade-in" style="animation-delay: 0.2s;">
                    <div class="contact-icon">
                        <i class="fas fa-phone"></i>
                    </div>
                    <div>
                        <h3>Phone</h3>
                        <p>+91 7668543534</p>
                    </div>
                </div>
                <div class="contact-item fade-in" style="animation-delay: 0.4s;">
                    <div class="contact-icon">
                        <i class="fas fa-map-marker-alt"></i>
                    </div>
                    <div>
                        <h3>Location</h3>
                        <p>India</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <footer>
        <div class="container">
            <div class="social-links">
                <a href="https://github.com/rawatabhishek385" class="social-link">
                    <i class="fab fa-github"></i>
                </a>
                <a href="#" class="social-link">
                    <i class="fab fa-linkedin-in"></i>
                </a>
                <a href="mailto:rawatabhishek385@gmail.com" class="social-link">
                    <i class="fas fa-envelope"></i>
                </a>
            </div>
            <p>© 2023 Abhishek Rawat. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Simple animation on scroll
        document.addEventListener('DOMContentLoaded', function() {
            const fadeElements = document.querySelectorAll('.fade-in');
            
            const fadeInOnScroll = function() {
                fadeElements.forEach(element => {
                    const elementTop = element.getBoundingClientRect().top;
                    const elementVisible = 150;
                    
                    if (elementTop < window.innerHeight - elementVisible) {
                        element.style.opacity = 1;
                        element.style.transform = 'translateY(0)';
                    }
                });
            };
            
            // Set initial state
            fadeElements.forEach(element => {
                element.style.opacity = 0;
                element.style.transform = 'translateY(20px)';
                element.style.transition = 'opacity 0.6s ease, transform 0.6s ease';
            });
            
            window.addEventListener('scroll', fadeInOnScroll);
            fadeInOnScroll(); // Check on load
        });
    </script>
</body>
</html>
