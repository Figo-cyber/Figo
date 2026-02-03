<!DOCTYPE html>
<html>
<head>
    <title>Website Pertamaku</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Halo Dunia! 👋</h1>
    <p>Ini website pertama saya di GitHub Pages</p>
    <img https://tse4.mm.bing.net/th/id/OIP.Znp2lna2Fa8kOW4QHXy1vAHaHa?w=178&h=180&c=7&r=0&o=7&pid=1.7&rm=3
</body>
</html>
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio - [Nama Kamu]</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #6C63FF;
            --dark: #1a1a2e;
            --light: #f8f9fa;
            --gray: #6c757d;
        }
        
        body {
            background-color: var(--dark);
            color: var(--light);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* NAVBAR */
        nav {
            background: rgba(26, 26, 46, 0.95);
            backdrop-filter: blur(10px);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            padding: 1rem 0;
            border-bottom: 1px solid rgba(108, 99, 255, 0.2);
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--light);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--primary);
        }
        
        .nav-links {
            display: flex;
            gap: 2rem;
        }
        
        .nav-links a {
            color: var(--light);
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary);
        }
        
        .menu-toggle {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
        }
        
        /* HERO SECTION */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding-top: 80px;
            background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
        }
        
        .hero-content {
            display: flex;
            align-items: center;
            gap: 4rem;
        }
        
        .hero-text {
            flex: 1;
        }
        
        .hero-image {
            flex: 1;
            text-align: center;
        }
        
        .hero-image img {
            max-width: 100%;
            border-radius: 50%;
            border: 3px solid var(--primary);
            width: 300px;
            height: 300px;
            object-fit: cover;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            background: linear-gradient(45deg, #6C63FF, #FF6584);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        .hero h2 {
            font-size: 1.8rem;
            color: var(--gray);
            margin-bottom: 1.5rem;
            font-weight: 400;
        }
        
        .hero p {
            font-size: 1.1rem;
            margin-bottom: 2rem;
            color: #aaa;
        }
        
        .btn {
            display: inline-block;
            background: var(--primary);
            color: white;
            padding: 12px 30px;
            border-radius: 30px;
            text-decoration: none;
            font-weight: 600;
            transition: transform 0.3s, box-shadow 0.3s;
            border: none;
            cursor: pointer;
        }
        
        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(108, 99, 255, 0.3);
        }
        
        .btn-outline {
            background: transparent;
            border: 2px solid var(--primary);
            margin-left: 10px;
        }
        
        /* ABOUT SECTION */
        section {
            padding: 100px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            display: inline-block;
            position: relative;
            margin-bottom: 1rem;
        }
        
        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background: var(--primary);
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }
        
        .skills {
            margin-top: 2rem;
        }
        
        .skill-item {
            margin-bottom: 1.5rem;
        }
        
        .skill-name {
            display: flex;
            justify-content: space-between;
            margin-bottom: 8px;
        }
        
        .skill-bar {
            height: 10px;
            background: #2d3047;
            border-radius: 5px;
            overflow: hidden;
        }
        
        .skill-level {
            height: 100%;
            background: linear-gradient(90deg, var(--primary), #8a84ff);
            border-radius: 5px;
        }
        
        /* PROJECTS SECTION */
        .projects {
            background: #16213e;
        }
        
        .project-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        
        .project-card {
            background: #1a1a2e;
            border-radius: 10px;
            overflow: hidden;
            transition: transform 0.3s;
        }
        
        .project-card:hover {
            transform: translateY(-10px);
        }
        
        .project-img {
            height: 200px;
            background: linear-gradient(45deg, #6C63FF, #FF6584);
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 3rem;
        }
        
        .project-info {
            padding: 1.5rem;
        }
        
        .project-info h3 {
            margin-bottom: 10px;
        }
        
        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 1rem;
        }
        
        .tag {
            background: rgba(108, 99, 255, 0.1);
            color: var(--primary);
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
        }
        
        /* CONTACT SECTION */
        .contact-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }
        
        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 2rem;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            background: rgba(108, 99, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            color: var(--primary);
        }
        
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 15px;
            margin-bottom: 1rem;
            background: #2d3047;
            border: 1px solid #444;
            border-radius: 5px;
            color: white;
        }
        
        .contact-form textarea {
            height: 150px;
            resize: vertical;
        }
        
        /* FOOTER */
        footer {
            background: #0f1123;
            padding: 3rem 0;
            text-align: center;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
        }
        
        .social-links a {
            color: var(--light);
            font-size: 1.5rem;
            transition: color 0.3s;
        }
        
        .social-links a:hover {
            color: var(--primary);
        }
        
        .copyright {
            color: var(--gray);
            margin-top: 2rem;
        }
        
        /* RESPONSIVE */
        @media (max-width: 992px) {
            .hero-content {
                flex-direction: column;
                text-align: center;
            }
            
            .about-content,
            .contact-container {
                grid-template-columns: 1fr;
            }
            
            .menu-toggle {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 70px;
                left: -100%;
                width: 100%;
                flex-direction: column;
                background: var(--dark);
                padding: 2rem;
                transition: left 0.3s;
            }
            
            .nav-links.active {
                left: 0;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
        }
        
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>
    <!-- NAVBAR -->
    <nav>
        <div class="container nav-container">
            <a href="#" class="logo">Portfo<span>lio.</span></a>
            <div class="menu-toggle" id="menuToggle">
                <i class="fas fa-bars"></i>
            </div>
            <div class="nav-links" id="navLinks">
                <a href="#home">Home</a>
                <a href="#about">Tentang</a>
                <a href="#projects">Proyek</a>
                <a href="#contact">Kontak</a>
            </div>
        </div>
    </nav>

    <!-- HERO SECTION -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <div class="hero-text">
                    <h1>Halo, Saya [Nama Kamu]</h1>
                    <h2>Web Developer & Designer</h2>
                    <p>Saya membuat website yang indah, fungsional, dan responsif. 
                       Berpengalaman dalam HTML, CSS, JavaScript, dan framework modern.</p>
                    <div class="hero-buttons">
                        <a href="#projects" class="btn">Lihat Proyek</a>
                        <a href="#contact" class="btn btn-outline">Hubungi Saya</a>
                    </div>
                </div>
                <div class="hero-image">
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=774&q=80" alt="Profile Photo">
                </div>
            </div>
        </div>
    </section>

    <!-- ABOUT SECTION -->
    <section id="about">
        <div class="container">
            <div class="section-title">
                <h2>Tentang Saya</h2>
                <p>Kenali lebih dekat tentang saya</p>
            </div>
            <div class="about-content">
                <div>
                    <h3>Kreatif & Berdedikasi</h3>
                    <p>Saya seorang web developer dengan passion menciptakan pengalaman digital yang menarik. 
                       Saya senang memecahkan masalah kompleks dan terus belajar teknologi baru.</p>
                    <p>Saya telah mengerjakan berbagai proyek dari website perusahaan hingga aplikasi web interaktif.</p>
                    
                    <div class="skills">
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>HTML/CSS</span>
                                <span>95%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 95%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>JavaScript</span>
                                <span>85%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 85%"></div>
                            </div>
                        </div>
                        <div class="skill-item">
                            <div class="skill-name">
                                <span>UI/UX Design</span>
                                <span>80%</span>
                            </div>
                            <div class="skill-bar">
                                <div class="skill-level" style="width: 80%"></div>
                            </div>
                        </div>
                    </div>
                </div>
                <div>
                    <h3>Pengalaman</h3>
                    <div class="experience">
                        <div class="exp-item">
                            <h4>Web Developer</h4>
                            <p class="exp-company">PT. Teknologi Indonesia</p>
                            <p class="exp-date">2022 - Sekarang</p>
                            <p>Mengembangkan dan memelihara website perusahaan dengan teknologi terbaru.</p>
                        </div>
                        <div class="exp-item">
                            <h4>Frontend Developer</h4>
                            <p class="exp-company">Startup Digital</p>
                            <p class="exp-date">2021 - 2022</p>
                            <p>Membuat aplikasi web responsif dengan React.js dan API integration.</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- PROJECTS SECTION -->
    <section class="projects" id="projects">
        <div class="container">
            <div class="section-title">
                <h2>Proyek Terbaru</h2>
                <p>Beberapa karya terbaik saya</p>
            </div>
            <div class="project-grid">
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-shopping-cart"></i>
                    </div>
                    <div class="project-info">
                        <h3>E-commerce Website</h3>
                        <p>Website toko online dengan sistem cart, checkout, dan dashboard admin.</p>
                        <div class="project-tags">
                            <span class="tag">HTML</span>
                            <span class="tag">CSS</span>
                            <span class="tag">JavaScript</span>
                            <span class="tag">PHP</span>
                        </div>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <div class="project-info">
                        <h3>Mobile App UI</h3>
                        <p>Desain antarmuka aplikasi mobile untuk layanan kesehatan digital.</p>
                        <div class="project-tags">
                            <span class="tag">Figma</span>
                            <span class="tag">UI Design</span>
                            <span class="tag">Prototyping</span>
                        </div>
                    </div>
                </div>
                <div class="project-card">
                    <div class="project-img">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <div class="project-info">
                        <h3>Dashboard Analytics</h3>
                        <p>Dashboard untuk visualisasi data dengan grafik interaktif real-time.</p>
                        <div class="project-tags">
                            <span class="tag">React</span>
                            <span class="tag">Chart.js</span>
                            <span class="tag">API</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CONTACT SECTION -->
    <section id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Hubungi Saya</h2>
                <p>Mari bekerja sama!</p>
            </div>
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div>
                            <h3>Lokasi</h3>
                            <p>Jakarta, Indonesia</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h3>Email</h3>
                            <p>hello@example.com</p>
                        </div>
                    </div>
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div>
                            <h3>Telepon</h3>
                            <p>+62 812 3456 7890</p>
                        </div>
                    </div>
                </div>
                <form class="contact-form">
                    <input type="text" placeholder="Nama Lengkap" required>
                    <input type="email" placeholder="Alamat Email" required>
                    <input type="text" placeholder="Subjek" required>
                    <textarea placeholder="Pesan Anda" required></textarea>
                    <button type="submit" class="btn">Kirim Pesan</button>
                </form>
            </div>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <a href="#" class="logo">Portfo<span>lio.</span></a>
            <p>Membuat dunia digital yang lebih baik, satu website dalam satu waktu.</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-github"></i></a>
                <a href="#"><i class="fab fa-linkedin"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
            <div class="copyright">
                <p>&copy; 2024 [Nama Kamu]. Semua hak dilindungi.</p>
            </div>
        </div>
    </footer>

    <script>
        // Mobile Menu Toggle
        const menuToggle = document.getElementById('menuToggle');
        const navLinks = document.getElementById('navLinks');
        
        menuToggle.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // Close menu when clicking on a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
            });
        });
        
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Form submission (dummy)
        document.querySelector('.contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            alert('Terima kasih! Pesan Anda telah dikirim. (Ini hanya demo)');
            this.reset();
        });
    </script>
</body>
</html>
