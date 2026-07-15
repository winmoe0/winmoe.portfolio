
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <!-- SEO Optimization -->
  <title>Win Moe | English Educator | Portfolio</title>
  <meta name="description" content="Professional portfolio of Win Moe, English educator, content creator, TEFL/TESOL certified teacher, and English Communication student.">
  <meta name="keywords" content="Win Moe, English Teacher, English Educator, Portfolio, Chiang Mai, Payap University, Mon National College, TEFL">
  <meta name="author" content="Win Moe">

  <!-- Google Fonts & Icon Libraries -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
  
  <style>
    /* --- Picto Layout Theme System & Variables --- */
    :root {
      --primary-color: #9333ea;
      --primary-hover: #7e22ce;
      --secondary-color: #00b4d8;
      --accent-color: #df9e51; /* Elegant Gold */
      --bg-light: radial-gradient(circle at 50% 50%, #eef3f7 0%, #dbe4ee 100%);
      --card-light: rgba(255, 255, 255, 0.92);
      --text-light: #1e2530;
      --text-muted-light: #4b5563;
      --border-light: rgba(0, 0, 0, 0.05);
      
      --bg-main: var(--bg-light);
      --card-bg: var(--card-light);
      --text-main: var(--text-light);
      --text-muted: var(--text-muted-light);
      --border-color: var(--border-light);
      --glass-shadow: 0 30px 70px rgba(31, 45, 65, 0.08);
      
      --transition-speed: 0.3s;
    }

    [data-theme="dark"] {
      --bg-main: #0f172a;
      --card-bg: #1e293b;
      --text-main: #f8fafc;
      --text-muted: #94a3b8;
      --border-color: rgba(255, 255, 255, 0.08);
      --glass-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.3);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
      font-size: 16px;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background: var(--bg-main);
      background-color: #f0f4f8; /* Dark mode fallback */
      color: var(--text-main);
      transition: background var(--transition-speed), color var(--transition-speed);
      overflow-x: hidden;
      padding: 40px 20px;
      -webkit-font-smoothing: antialiased;
    }

    /* --- Reusable Layout Components --- */
    .portfolio-base-card {
      max-width: 1200px;
      margin: 0 auto;
      background: var(--card-bg);
      border-radius: 32px;
      box-shadow: var(--glass-shadow);
      border: 1px solid rgba(255, 255, 255, 0.7);
      padding: 30px 50px 60px 50px;
      overflow: hidden;
    }

    .container-box {
      width: 100%;
      max-width: 1100px;
      margin: 0 auto;
      padding: 60px 0;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 2.2em;
      font-weight: 700;
      color: #111827;
    }
    
    [data-theme="dark"] .section-title h2 {
      color: #fff;
    }

    .title-line {
      width: 60px;
      height: 4px;
      background-color: var(--primary-color);
      margin: 10px auto 0;
      border-radius: 2px;
    }

    /* --- Loader Styling --- */
    .loader-container {
      position: fixed;
      top: 0; left: 0; width: 100%; height: 100%;
      background-color: #f3f4f6;
      display: flex; justify-content: center; align-items: center;
      z-index: 9999;
      transition: opacity 0.5s ease, visibility 0.5s;
    }
    .loader {
      width: 50px; height: 50px;
      border: 5px solid rgba(147, 51, 234, 0.1);
      border-top-color: var(--primary-color);
      border-radius: 50%;
      animation: spin 1s infinite linear;
    }
    @keyframes spin { to { transform: rotate(360deg); } }

    /* --- Embedded Navbar Custom Styles --- */
    .picto-navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 15px 0 40px 0;
      border-bottom: 1px solid var(--border-color);
    }

    .picto-logo {
      font-size: 1.3em;
      font-weight: 700;
      color: var(--text-main);
      display: flex;
      align-items: center;
      gap: 10px;
    }

    .logo-badge {
      background: var(--primary-color);
      color: white;
      width: 36px;
      height: 36px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 0.9em;
      font-weight: 600;
    }

    .picto-nav-links {
      display: flex;
      align-items: center;
      list-style: none;
      gap: 35px;
    }

    .picto-nav-links a {
      text-decoration: none;
      color: #5c677d;
      font-weight: 500;
      font-size: 0.92em;
      transition: color 0.25s ease;
    }

    .picto-nav-links a:hover, .picto-nav-links a.active {
      color: var(--text-main);
    }

    .picto-nav-links a.nav-contact-btn {
      background: var(--primary-color);
      color: white;
      padding: 10px 24px;
      border-radius: 8px;
      font-weight: 500;
      transition: background-color 0.25s ease;
    }

    .picto-nav-links a.nav-contact-btn:hover {
      background: var(--primary-hover);
    }

    .theme-btn {
      background: none; border: none;
      color: var(--text-main); font-size: 1.2em;
      cursor: pointer; transition: color var(--transition-speed);
      margin-left: 15px;
    }

    .hamburger {
      display: none; flex-direction: column; gap: 5px; cursor: pointer;
    }
    .hamburger span {
      width: 25px; height: 3px; background-color: var(--text-main);
      border-radius: 2px; transition: all 0.3s ease;
    }

    /* --- Picto Hero Layout Elements --- */
    .picto-hero {
      display: grid;
      grid-template-columns: 1.1fr 0.9fr;
      gap: 50px;
      align-items: center;
      padding: 60px 0;
    }

    .picto-greeting {
      font-size: 3.8em;
      font-weight: 700;
      color: var(--text-main);
      line-height: 1.15;
      margin-bottom: 24px;
      letter-spacing: -1px;
    }

    .picto-lead-text {
      font-size: 1.05em;
      line-height: 1.7;
      color: var(--text-muted);
      margin-bottom: 35px;
      max-width: 520px;
    }

    .highlight-purple { color: #7e22ce; border-bottom: 1px dashed #c084fc; font-weight: 500; }
    .highlight-pink { color: #db2777; border-bottom: 1px dashed #f472b6; font-weight: 500; }

    .btn-picto-purple {
      display: inline-block;
      background: var(--primary-color);
      color: white;
      text-decoration: none;
      padding: 14px 32px;
      border-radius: 8px;
      font-weight: 600;
      font-size: 0.95em;
      box-shadow: 0 10px 25px rgba(147, 51, 234, 0.25);
      transition: all 0.25s ease;
      margin-bottom: 50px;
    }

    .btn-picto-purple:hover {
      background: var(--primary-hover);
      transform: translateY(-2px);
      box-shadow: 0 12px 28px rgba(126, 34, 206, 0.35);
    }

    .picto-mini-stats {
      display: flex;
      gap: 40px;
      border-top: 1px solid var(--border-color);
      padding-top: 30px;
      max-width: 450px;
    }

    .mini-stat-item h3 { font-size: 1.6em; font-weight: 700; color: var(--text-main); margin: 0; }
    .mini-stat-item p { font-size: 0.88em; color: var(--text-muted); margin: 2px 0 0 0; }

    .picto-hero-right { display: flex; justify-content: flex-end; }
    .picto-img-container {
      width: 100%; max-width: 430px;
      border-radius: 24px; overflow: hidden;
      box-shadow: 0 20px 50px rgba(0, 0, 0, 0.04);
      background-color: #f3f4f6;
      border: 4px solid #fff;
    }
    .picto-img-container img { width: 100%; height: auto; display: block; object-fit: cover; }

    /* --- About & Tags styling --- */
    .about-box {
      background: rgba(0, 0, 0, 0.01);
      border-radius: 16px; padding: 40px;
      border: 1px solid var(--border-color);
    }
    .about-box h3 { font-size: 1.6em; margin-bottom: 15px; }
    .about-box p { color: var(--text-muted); line-height: 1.7; margin-bottom: 20px; }
    .about-tags { display: flex; flex-wrap: wrap; gap: 15px; margin-top: 25px; }
    .about-tags span {
      background: #fff; border: 1px solid var(--border-color);
      padding: 8px 16px; border-radius: 30px; font-size: 0.9em;
    }
    .about-tags span i { color: var(--accent-color); margin-right: 5px; }

    /* --- Qualifications Cards --- */
    .qual-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 25px; }
    .qual-card {
      background-color: #fff; border: 1px solid var(--border-color);
      border-radius: 16px; padding: 30px; position: relative;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
    }
    .qual-card:hover { transform: translateY(-5px); box-shadow: 0 10px 25px rgba(0,0,0,0.03); }
    .qual-icon { font-size: 1.8em; color: var(--primary-color); margin-bottom: 20px; }
    .qual-status {
      position: absolute; top: 30px; right: 30px; font-size: 0.75em;
      text-transform: uppercase; font-weight: 700; color: var(--secondary-color);
      background: rgba(0, 180, 216, 0.1); padding: 4px 10px; border-radius: 4px;
    }
    .qual-status.gold { color: var(--accent-color); background: rgba(223, 158, 81, 0.1); }
    .qual-status.complete { color: #2a9d8f; background: rgba(42, 157, 143, 0.1); }
    .qual-card h3 { font-size: 1.2em; margin-bottom: 10px; }
    .qual-card p { color: var(--text-muted); font-size: 0.9em; line-height: 1.6; }

    /* --- Timeline Architecture --- */
    .timeline-tabs { display: flex; justify-content: center; gap: 20px; margin-bottom: 50px; }
    .tab-btn {
      padding: 10px 24px; border-radius: 30px; border: 1px solid var(--border-color);
      background: #fff; color: var(--text-main); font-weight: 600; cursor: pointer;
      transition: all var(--transition-speed);
    }
    .tab-btn.active, .tab-btn:hover { background-color: var(--primary-color); color: white; border-color: var(--primary-color); }
    .timeline-content { display: none; }
    .timeline-content.active { display: block; }
    .timeline { position: relative; max-width: 900px; margin: 0 auto; }
    .timeline::after { content: ''; position: absolute; width: 2px; background-color: var(--border-color); top: 0; bottom: 0; left: 50%; margin-left: -1px; }
    .timeline-item { padding: 10px 40px; position: relative; width: 50%; }
    .timeline-item.left { left: 0; }
    .timeline-item.right { left: 50%; }
    .timeline-dot {
      position: absolute; width: 16px; height: 16px; right: -8px;
      background-color: #fff; border: 4px solid var(--primary-color); top: 25px; border-radius: 50%; z-index: 1;
    }
    .timeline-item.right .timeline-dot { left: -8px; }
    .timeline-date { font-weight: 700; color: var(--accent-color); margin-bottom: 8px; }
    .timeline-card { padding: 24px; background-color: #fff; border-radius: 12px; border: 1px solid var(--border-color); }
    .timeline-card h3 { font-size: 1.2em; margin-bottom: 4px; }
    .timeline-card h4 { font-size: 0.95em; color: var(--secondary-color); font-weight: 500; margin-bottom: 10px; }
    .timeline-card p { font-size: 0.9em; color: var(--text-muted); line-height: 1.5; }

    /* --- Skills Matrix Mechanics --- */
    .skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 40px; }
    .skills-category { background: #fff; border: 1px solid var(--border-color); border-radius: 16px; padding: 30px; }
    .skills-category h3 { font-size: 1.3em; margin-bottom: 25px; color: var(--primary-color); display: flex; align-items: center; gap: 10px; }
    .skill-item { margin-bottom: 20px; }
    .skill-info { display: flex; justify-content: space-between; margin-bottom: 8px; font-size: 0.9em; font-weight: 500; }
    .progress-bar { width: 100%; height: 6px; background-color: #f3f4f6; border-radius: 3px; overflow: hidden; }
    .progress { height: 100%; background: linear-gradient(90deg, var(--primary-color), var(--secondary-color)); width: 0; transition: width 1.5s cubic-bezier(0.1, 1, 0.1, 1); }

    /* --- Certifications Strip --- */
    .certs-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); gap: 15px; }
    .cert-item-card { background: #fff; border: 1px solid var(--border-color); padding: 16px 20px; border-radius: 8px; display: flex; align-items: center; gap: 15px; font-size: 0.9em; font-weight: 500; }
    .cert-item-card i { color: var(--primary-color); font-size: 1.2em; }
    .cert-item-card i.gold-icon { color: var(--accent-color); }

    /* --- Portfolio Engine --- */
    .portfolio-filters { display: flex; justify-content: center; gap: 15px; margin-bottom: 35px; flex-wrap: wrap; }
    .filter-btn { padding: 8px 20px; border-radius: 20px; border: 1px solid var(--border-color); background: transparent; color: var(--text-main); cursor: pointer; transition: all var(--transition-speed); font-size: 0.9em; }
    .filter-btn.active, .filter-btn:hover { background-color: var(--primary-color); color: white; border-color: var(--primary-color); }
    .portfolio-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 25px; }
    .portfolio-item { position: relative; border-radius: 12px; overflow: hidden; cursor: pointer; border: 1px solid var(--border-color); aspect-ratio: 4/3; }
    .portfolio-item img { width: 100%; height: 100%; object-fit: cover; transition: transform 0.5s ease; }
    .portfolio-overlay { position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: linear-gradient(to top, rgba(147, 51, 234, 0.9), rgba(0, 180, 216, 0.6)); display: flex; flex-direction: column; justify-content: flex-end; padding: 24px; opacity: 0; transition: opacity 0.3s ease; }
    .portfolio-item:hover .portfolio-overlay { opacity: 1; }
    .portfolio-item:hover img { transform: scale(1.05); }
    .portfolio-overlay h4 { color: white; font-size: 1.2em; margin-bottom: 4px; }
    .portfolio-overlay p { color: rgba(255,255,255,0.8); font-size: 0.85em; }

    /* --- Research Section --- */
    .research-card { background: #fff; border: 1px solid var(--border-color); border-radius: 16px; padding: 40px; }
    .research-header { display: flex; align-items: center; gap: 20px; margin-bottom: 20px; border-bottom: 1px solid var(--border-color); padding-bottom: 20px; }
    .research-header i { font-size: 2.5em; color: var(--primary-color); }
    .research-header h3 { font-size: 1.5em; line-height: 1.4; }
    .research-body p { color: var(--text-muted); line-height: 1.6; margin-bottom: 20px; }
    .research-details { display: flex; flex-direction: column; gap: 12px; }
    .research-details span { font-size: 0.95em; line-height: 1.5; }

    /* --- Testimonials Framework --- */
    .slider-container { max-width: 800px; margin: 0 auto; text-align: center; padding: 20px; }
    .testimonial-slide .quote { font-size: 1.2em; font-style: italic; line-height: 1.7; margin-bottom: 15px; }
    .testimonial-slide h4 { color: var(--primary-color); font-weight: 600; }

    /* --- Contact Block & Elements --- */
    .contact-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 40px; }
    .contact-form { display: flex; flex-direction: column; gap: 15px; }
    .form-group input, .form-group textarea { width: 100%; padding: 14px 20px; border-radius: 8px; background: #fff; border: 1px solid var(--border-color); color: var(--text-main); font-family: inherit; font-size: 0.95em; transition: border-color var(--transition-speed); }
    .form-group input:focus, .form-group textarea:focus { outline: none; border-color: var(--primary-color); }

    /* --- Modal Overlay Design --- */
    .modal-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.5); backdrop-filter: blur(4px); z-index: 2000; display: flex; justify-content: center; align-items: center; opacity: 0; visibility: hidden; transition: all 0.3s ease; }
    .modal-overlay.active { opacity: 1; visibility: visible; }
    .modal-card { background: #fff; padding: 40px; border-radius: 16px; max-width: 500px; width: 90%; position: relative; box-shadow: 0 10px 30px rgba(0,0,0,0.1); }
    .close-modal { position: absolute; top: 20px; right: 25px; font-size: 2em; cursor: pointer; color: var(--text-muted); }

    /* --- Footer Area --- */
    .footer-section { background-color: #0b132b; color: #adbac7; padding: 60px 20px 20px; border-top: 1px solid rgba(255,255,255,0.05); border-radius: 0 0 32px 32px; margin-top: 40px; }
    .footer-grid { display: flex; justify-content: space-between; flex-wrap: wrap; gap: 40px; padding-bottom: 40px; border-bottom: 1px solid rgba(255,255,255,0.05); }
    .footer-info h3 { color: white; margin-bottom: 10px; }
    .footer-links h4 { color: white; margin-bottom: 15px; }
    .footer-links a { display: block; color: #adbac7; text-decoration: none; margin-bottom: 8px; font-size: 0.9em; }
    .footer-links a:hover { color: var(--secondary-color); }
    .footer-bottom { text-align: center; padding-top: 20px; font-size: 0.85em; }

    /* --- Global Scroll Components --- */
    .scroll-top-btn { position: fixed; bottom: 30px; right: 30px; width: 45px; height: 45px; border-radius: 50%; background-color: var(--primary-color); color: white; border: none; cursor: pointer; display: flex; justify-content: center; align-items: center; box-shadow: 0 4px 10px rgba(0,0,0,0.1); opacity: 0; visibility: hidden; transition: all 0.3s ease; z-index: 99; }
    .scroll-top-btn.visible { opacity: 1; visibility: visible; }
    .scroll-reveal { opacity: 0; transform: translateY(30px); transition: opacity 0.8s ease, transform 0.8s ease; }
    .scroll-reveal.reveal-active { opacity: 1; transform: translateY(0); }

    /* --- Responsive Adaptations --- */
    @media (max-width: 992px) {
      .portfolio-base-card { padding: 30px; }
      .picto-hero { grid-template-columns: 1fr; text-align: center; gap: 40px; }
      .picto-lead-text { margin: 0 auto 35px auto; }
      .picto-mini-stats { margin: 0 auto; justify-content: center; }
      .picto-hero-right { justify-content: center; }
      .timeline::after { left: 20px; }
      .timeline-item { width: 100%; padding-left: 50px; padding-right: 0; }
      .timeline-item.right { left: 0; }
      .timeline-dot { left: 12px !important; }
      .contact-grid { grid-template-columns: 1fr; }
    }

    @media (max-width: 768px) {
      .picto-nav-links {
        position: absolute; top: 100%; left: 0; width: 100%;
        background-color: #fff; flex-direction: column; text-align: center;
        padding: 20px 0; gap: 20px; border-bottom: 1px solid var(--border-color);
        display: none; z-index: 100;
      }
      .picto-nav-links.mobile-active { display: flex; }
      .hamburger { display: flex; }
      .picto-greeting { font-size: 2.8em; }
    }
  </style>
</head>
<body>

  <!-- Loading Animation Overlay -->
  <div id="loader" class="loader-container">
    <div class="loader"></div>
  </div>

  <!-- Primary Framed Layout Container -->
  <div class="portfolio-base-card">
    
    <!-- Embedded Header Navigation Bar -->
    <nav class="picto-navbar">
      <div class="picto-logo">
        <span class="logo-badge">W</span> Win Moe
      </div>
      <ul class="picto-nav-links">
        <li><a href="#home" class="active">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#qualifications">Qualifications</a></li>
        <li><a href="#experience">Experience</a></li>
        <li><a href="#portfolio">Portfolio</a></li>
        <li><a href="#contact" class="nav-contact-btn">Say Hello!</a></li>
        <li>
          <button id="theme-toggle" aria-label="Toggle theme" class="theme-btn">
            <i class="fas fa-moon"></i>
          </button>
        </li>
      </ul>
      <div class="hamburger" aria-label="Menu">
        <span></span><span></span><span></span>
      </div>
    </nav>

    <!-- Picto Custom Hero Content Section Split -->
    <header id="home" class="picto-hero">
      <div class="picto-hero-left">
        <h1 class="picto-greeting">Hello, I'm <br><span>Win Moe</span></h1>
        <h3 style="font-size: 1.2em; font-weight: 500; color: var(--primary-color); margin-bottom: 15px;">English Educator | Content Creator | Video Editor</h3>
        <p class="picto-lead-text">
          I'm an English <span class="highlight-purple">Educator</span>, <span class="highlight-pink">Content Creator</span>, and Video Editor based in Chiang Mai, Thailand. I strive to build immersive language experiences through student-centric methods and modern media workflows.
        </p>
        
        <a href="#contact" class="btn-picto-purple">Contact Me</a>

        <!-- Counter Metric Nodes directly under introduction text -->
        <div class="picto-mini-stats">
          <div class="mini-stat-item">
            <div class="counter" data-target="4" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Years Exp.</p>
          </div>
          <div class="mini-stat-item">
            <div class="counter" data-target="1000" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Students Taught</p>
          </div>
          <div class="mini-stat-item">
            <div class="counter" data-target="15" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Certificates</p>
          </div>
        </div>
      </div>

      <div class="picto-hero-right">
        <div class="picto-img-container">
          <!-- Configured directly to your provided filename -->
          <img src="winmoeprofile2.jpg" alt="Win Moe Portrait" onerror="this.src='https://via.placeholder.com/330x400'">
        </div>
      </div>
    </header>

    <!-- About Me Section -->
    <section id="about" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>About Me</h2>
        <div class="title-line"></div>
      </div>
      <div class="about-box">
        <h3>English Instructor & Content Creator</h3>
        <p>I am a dedicated and passionate English educator with over four years of teaching experience in both classroom and online learning environments. I am committed to creating engaging, student-centered lessons that foster confidence, critical thinking, and effective communication. I strive to build inclusive and supportive learning environments where students from diverse cultural backgrounds feel motivated to achieve their full potential.</p>
<p>Beyond teaching, I have a strong interest in educational technology and digital innovation. I enjoy creating educational content through video editing, photography, graphic design, and social media, transforming learning materials into engaging digital experiences. My leadership and volunteer experience have strengthened my communication, teamwork, and project management skills, enabling me to collaborate effectively with colleagues and contribute to educational initiatives both inside and outside the classroom. I am committed to continuous professional development and aspire to make a meaningful impact on education through innovative teaching and lifelong learning.</p>
        <div class="about-tags">
        <span><i class="fas fa-check"></i> Onsite & Online Instruction</span>
<span><i class="fas fa-check"></i> Lesson Planning</span>
<span><i class="fas fa-check"></i> Curriculum Development</span>
<span><i class="fas fa-check"></i> Classroom Management</span>
<span><i class="fas fa-check"></i> Student Assessment</span>
<span><i class="fas fa-check"></i> Young Learners Teaching</span>
<span><i class="fas fa-check"></i> Adult English Instruction</span>
<span><i class="fas fa-check"></i> English for Academic Purposes (EAP)</span>
<span><i class="fas fa-check"></i> Grammar & Writing Instruction</span>
<span><i class="fas fa-check"></i> Educational Technology</span>
          <span><i class="fas fa-check"></i> Content Creation</span>
          <span><i class="fas fa-check"></i> Social Media Management</span>
          <span><i class="fas fa-check"></i> Digital Marketing</span>
        </div>
      </div>
    </section>

    <!-- Qualifications Section -->
<section id="qualifications" class="container-box scroll-reveal">
  <div class="section-title">
    <h2>Qualifications</h2>
    <div class="title-line"></div>
  </div>

  <div class="qual-grid">

    <div class="qual-card">
      <div class="qual-icon"><i class="fas fa-university"></i></div>
      <span class="qual-status gold">Candidate</span>
      <h3>Master of Arts in Public Affairs</h3>
      <p>Currently pursuing advanced studies in public policy, governance, leadership, and sustainable community development.</p>
    </div>

    <div class="qual-card">
      <div class="qual-icon"><i class="fas fa-graduation-cap"></i></div>
      <span class="qual-status">Current</span>
      <h3>Bachelor of Arts in English Communication</h3>
      <p>Payap University, Thailand. Developing expertise in English communication, intercultural communication, public speaking, and professional writing.</p>
    </div>

    <div class="qual-card">
      <div class="qual-icon"><i class="fas fa-award"></i></div>
      <span class="qual-status complete">Graduated</span>
      <h3>Associate Degree in Education</h3>
      <p>Mon National College, Myanmar. Studied teaching methodologies, curriculum development, educational psychology, classroom management, and student assessment.</p>
    </div>

    <div class="qual-card">
      <div class="qual-icon"><i class="fas fa-file-alt"></i></div>
      <span class="qual-status complete">Graduated</span>
      <h3>Diploma in Social Science</h3>
      <p>National University of Zoland. Studied sociology, political science, community development, and social research.</p>
    </div>
<div class="qual-card">
  <div class="qual-icon"><i class="fas fa-chalkboard-teacher"></i></div>
  <span class="qual-status complete">Certified</span>
  <h3>TEFL/TESOL Certification</h3>
  <p>Certified to teach English as a Foreign Language with training in communicative teaching methods, lesson planning, classroom management, and learner assessment.</p>
</div>

<div class="qual-card">
  <div class="qual-icon"><i class="fab fa-google"></i></div>
  <span class="qual-status complete">Certified</span>
  <h3>Google Digital Marketing & E-Commerce</h3>
  <p>Professional training in digital marketing, content creation, social media strategy, search engine optimization (SEO), analytics, and e-commerce.</p>
</div>
      </div>
    </section>

    <!-- Experience & Leadership Tabbed Timelines -->
<section id="experience" class="container-box scroll-reveal">
  <div class="section-title">
    <h2>Professional Experience</h2>
    <div class="title-line"></div>
  </div>

  <div class="timeline-tabs">
    <button class="tab-btn active" data-tab="work">Teaching & Media</button>
    <button class="tab-btn" data-tab="leadership">Leadership & Volunteering</button>
  </div>

  <!-- Teaching Experience -->
  <div id="work-timeline" class="timeline-content active">
    <div class="timeline">

      <!-- English Teacher -->
      <div class="timeline-item left">
        <div class="timeline-dot"></div>
        <div class="timeline-date">2023 – 2024</div>
        <div class="timeline-card">
          <h3>English Teacher</h3>
          <h4>Mon National Primary School, Myanmar</h4>
          <p>
            Taught English to primary school students through engaging, student-centered lessons that developed listening, speaking, reading, and writing skills. Planned lessons, prepared learning materials, assessed student progress, and created a positive classroom environment that encouraged active participation and confidence.
          </p>
        </div>
      </div>

      <!-- Online Teacher -->
      <div class="timeline-item right">
        <div class="timeline-dot"></div>
        <div class="timeline-date">2019 – Present</div>
        <div class="timeline-card">
          <h3>Online English Instructor</h3>
          <h4>Poy English Program</h4>
          <p>
            Deliver online English lessons for young learners and adult students using Zoom and Google Meet. Design customized lesson plans, teach grammar, pronunciation, speaking, reading, and writing, and support learners in achieving their academic and personal language goals through interactive instruction.
          </p>
        </div>
      </div>

      <!-- Content Creator -->
      <div class="timeline-item left">
        <div class="timeline-dot"></div>
        <div class="timeline-date">2019 – Present</div>
        <div class="timeline-card">
          <h3>Educational Content Creator</h3>
          <h4>Social Media Plaforms</h4>
          <p>
            Produce educational videos, English learning resources, graphics, and social media content for online audiences. Utilize video editing, photography, Canva, and digital marketing strategies to create engaging learning experiences and promote educational programs.
          </p>
        </div>
      </div>

      <!-- Freelance -->
      <div class="timeline-item right">
        <div class="timeline-dot"></div>
        <div class="timeline-date">2022 – Present</div>
        <div class="timeline-card">
          <h3>Freelance English Tutor</h3>
          <h4>All Scholars Educational Program</h4>
          <p>
            Provide one-on-one and small-group English lessons tailored to learners' individual goals, including conversational English, grammar, academic writing, pronunciation, and exam preparation.
          </p>
        </div>
      </div>

      <!-- AI Educational Content -->
<div class="timeline-item left">
  <div class="timeline-dot"></div>
  <div class="timeline-date">2025 – Present</div>
  <div class="timeline-card">
    <h3>AI Educational Content Creator</h3>
    <h4>EthnoVerse (Facebook & Digital Platforms)</h4>
    <p>
      Create AI-assisted educational content, including short-form videos, historical storytelling, English learning materials, and digital visuals. Utilize AI tools, Canva, video editing software, and multimedia design to transform complex topics into engaging and accessible content for diverse online audiences while promoting education through social media.
          </p>
        </div>
      </div>

</div>
    </div>
      <!-- Leadership & Volunteer Timeline Content -->
<div id="leadership-timeline" class="timeline-content">
  <div class="timeline">

    <!-- Student Leader -->
    <div class="timeline-item left">
      <div class="timeline-dot"></div>
      <div class="timeline-date">2023 – 2024</div>
      <div class="timeline-card">
        <h3>Student leader</h3>
        <h4>Student Council, Hpa-An University, Myanmar</h4>
        <p>
          Led the Student Union by representing students' interests, organizing academic and community events, coordinating with faculty members, and promoting teamwork, leadership, and student engagement across the university.
        </p>
      </div>
    </div>

    <!-- Charity -->
    <div class="timeline-item right">
      <div class="timeline-dot"></div>
      <div class="timeline-date">Present</div>
      <div class="timeline-card">
        <h3>Chairman</h3>
        <h4>G60–99 Mon Charity Group</h4>
        <p>
          Coordinate community service initiatives, organize fundraising activities, manage volunteer teams, and support charitable projects that provide educational and humanitarian assistance to local communities.
        </p>
      </div>
    </div>

    <!-- Volunteer Teacher -->
    <div class="timeline-item left">
      <div class="timeline-dot"></div>
      <div class="timeline-date">2024 – 2025</div>
      <div class="timeline-card">
        <h3>Volunteer English Teacher</h3>
        <h4>Mon Internsive English Program</h4>
        <p>
          Taught English to refugee and migrant learners through interactive lessons designed to improve communication skills, confidence, and academic readiness in a supportive learning environment.
        </p>
      </div>
    </div>

    <!-- University Volunteer -->
    <div class="timeline-item right">
      <div class="timeline-dot"></div>
      <div class="timeline-date">2024 – Present</div>
      <div class="timeline-card">
        <h3>University Volunteer</h3>
        <h4>Payap University International College</h4>
        <p>
          Assisted in university events, orientation programs, intercultural activities, and student engagement projects while collaborating with students from diverse cultural backgrounds.
        </p>
      </div>
    </div>

    <!-- Educational Outreach -->
    <div class="timeline-item left">
      <div class="timeline-dot"></div>
      <div class="timeline-date">Ongoing</div>
      <div class="timeline-card">
        <h3>Educational Outreach & Content Creator</h3>
        <h4>Community Education</h4>
        <p>
          Create free educational resources, English learning content, and digital materials to support lifelong learning and improve access to quality education through online platforms and social media.
        </p>
      </div>
    </div>
    </div>
    </div>
    
    <!-- Skills Matrix Grid Section -->
    <section id="skills" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Skills Matrix</h2>
        <div class="title-line"></div>
      </div>
      <div class="skills-grid">
        <div class="skills-category">
          <h3><i class="fas fa-apple-alt"></i> Instructional Design</h3>
          <div class="skill-item">
            <div class="skill-info"><span>Lesson Architecture & Planning</span><span>95%</span></div>
            <div class="progress-bar"><div class="progress" data-width="95%"></div></div>
          </div>
          <div class="skill-item">
            <div class="skill-info"><span>Classroom Control Matrices</span><span>90%</span></div>
            <div class="progress-bar"><div class="progress" data-width="90%"></div></div>
          </div>
          <div class="skill-item">
            <div class="skill-info"><span>Curriculum & Material Adaptation</span><span>92%</span></div>
            <div class="progress-bar"><div class="progress" data-width="92%"></div></div>
          </div>
        </div>

        <div class="skills-category">
          <h3><i class="fas fa-laptop-code"></i> Technical Tools</h3>
          <div class="skill-item">
            <div class="skill-info"><span>Digital Media Tools (Canva, CapCut, Premiere)</span><span>88%</span></div>
            <div class="progress-bar"><div class="progress" data-width="88%"></div></div>
          </div>
          <div class="skill-item">
            <div class="skill-info"><span>E-Learning Interfaces (Zoom, Meet)</span><span>95%</span></div>
            <div class="progress-bar"><div class="progress" data-width="95%"></div></div>
          </div>
          <div class="skill-item">
            <div class="skill-info"><span>Frontend Web (HTML5, CSS3, GitHub)</span><span>75%</span></div>
            <div class="progress-bar"><div class="progress" data-width="75%"></div></div>
          </div>
        </div>
      </div>
    </section>

    <!-- Professional Certifications Grid -->
    <section class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Certifications</h2>
        <div class="title-line"></div>
      </div>
      <div class="certs-grid">
        <div class="cert-item-card"><i class="fas fa-medal gold-icon"></i> <span>TEFL/TESOL Professional (2026)</span></div>
        <div class="cert-item-card"><i class="fas fa-child"></i> <span>Teaching Young Learners (2026)</span></div>
        <div class="cert-item-card"><i class="fab fa-google text-blue"></i> <span>Google Digital Marketing & E-Commerce</span></div>
        <div class="cert-item-card"><i class="fas fa-language"></i> <span>English Four Skills Certification</span></div>
        <div class="cert-item-card"><i class="fas fa-globe"></i> <span>Localization in Humanitarian Aid</span></div>
        <div class="cert-item-card"><i class="fas fa-chalkboard-teacher"></i> <span>Mastering E-Learning Designs</span></div>
      </div>
    </section>

    <!-- Portfolio Filter Showcase Grid -->
    <section id="portfolio" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Portfolio Showcase</h2>
        <div class="title-line"></div>
      </div>
      <div class="portfolio-filters">
        <button class="filter-btn active" data-filter="all">All Projects</button>
        <button class="filter-btn" data-filter="teaching">Teaching</button>
        <button class="filter-btn" data-filter="media">Media & Content</button>
      </div>
      <div class="portfolio-grid">
        <div class="portfolio-item" data-category="teaching" onclick="openModal('modal-p1')">
          <img src="https://via.placeholder.com/400x300" alt="Teaching Project Asset">
          <div class="portfolio-overlay">
            <h4>Poy English Online Launch</h4>
            <p>Interactive Language Program Infrastructure</p>
          </div>
        </div>
        <div class="portfolio-item" data-category="media" onclick="openModal('modal-p2')">
          <img src="https://via.placeholder.com/400x300" alt="Media Asset">
          <div class="portfolio-overlay">
            <h4>Language Graphic Campaign</h4>
            <p>Infographics & Video Production Projects</p>
          </div>
        </div>
      </div>
    </section>

    <!-- Academic Research Section Focus -->
    <section id="research" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Academic Research Focus</h2>
        <div class="title-line"></div>
      </div>
      <div class="research-card">
        <div class="research-header">
          <i class="fas fa-book-reader"></i>
          <h3>Academic Challenges among English Communication Arts Students at Payap University</h3>
        </div>
        <div class="research-body">
          <p><strong>Abstract:</strong> Evaluating transactional linguistic barriers, adjustment timelines, and institutional delivery friction vectors facing international academic cohorts adjusting to premium English communication requirements within modern university modules.</p>
          <div class="research-details">
            <span><strong>Objectives:</strong> Isolate core socio-linguistic blocks impacting academic fluency.</span>
            <span><strong>Methods:</strong> Integrated mixed-method structural interviews, cohort questionnaires, and qualitative metrics.</span>
            <span><strong>Findings:</strong> Data highlights strategic technology integration and structural peer-to-peer communication matrices drastically optimize comprehension and confidence levels.</span>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact & Embedded Map Form Integration -->
    <section id="contact" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Get In Touch</h2>
        <div class="title-line"></div>
      </div>
      <div class="contact-grid">
        <form class="contact-form" action="https://formspree.io/f/YOUR_FORMSPREE_ID_HERE" method="POST">
          <div class="form-group"><input type="text" name="name" required placeholder="Your Name"></div>
          <div class="form-group"><input type="email" name="email" required placeholder="Your Email Address"></div>
          <div class="form-group"><input type="text" name="subject" required placeholder="Subject"></div>
          <div class="form-group"><textarea name="message" rows="5" required placeholder="Your Message Content Here..."></textarea></div>
          <button type="submit" class="btn-picto-purple" style="border:none; cursor:pointer;">Send Message</button>
        </form>
        <div class="map-container">
          <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d59587.94583110512!2d98.9490204781702!3d18.796143003056024!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1m3!1zQ2hpYW5nIE1haQ!5e0!3m2!1sen!2sth!4v1700000000000!5m2!1sen!2sth" width="100%" height="320" style="border:0; border-radius:12px;" allowfullscreen="" loading="lazy"></iframe>
        </div>
      </div>
    </section>

    <!-- Unified Footer Construction -->
    <footer class="footer-section">
      <div class="footer-grid">
        <div class="footer-info">
          <h3>Win Moe</h3>
          <p>English Educator & Digital Innovation Architect.</p>
        </div>
        <div class="footer-links">
          <h4>Quick Links</h4>
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#portfolio">Portfolio</a>
        </div>
      </div>
      <div class="footer-bottom">
        <p>&copy; 2026 Win Moe. All Rights Reserved. Professional Portfolio Site.</p>
      </div>
    </footer>

  </div>

  <!-- Scroll-to-Top Global Interactive Button -->
  <button id="scroll-top" aria-label="Scroll to top" class="scroll-top-btn"><i class="fas fa-chevron-up"></i></button>

  <!-- Interactive Project Modals Architecture -->
  <div id="modal-p1" class="modal-overlay" onclick="closeModal('modal-p1')">
    <div class="modal-card" onclick="event.stopPropagation()">
      <span class="close-modal" onclick="closeModal('modal-p1')">&times;</span>
      <h3>Poy English Online Launch</h3>
      <p style="margin-top: 15px; line-height: 1.6; color: #555;">Detailed documentation concerning curriculum build paths, student enrollment funnels, and performance outputs tracking online educational platforms.</p>
    </div>
  </div>
  
  <div id="modal-p2" class="modal-overlay" onclick="closeModal('modal-p2')">
    <div class="modal-card" onclick="event.stopPropagation()">
      <span class="close-modal" onclick="closeModal('modal-p2')">&times;</span>
      <h3>Language Graphic Campaign</h3>
      <p style="margin-top: 15px; line-height: 1.6; color: #555;">Exhibiting detailed layouts of instructional templates, video editing passes created in CapCut/Premiere Pro, and interactive assets.</p>
    </div>
  </div>

  <!-- Integrated Operational JavaScript -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      
      // --- Loading Overlay Controller ---
      const loader = document.getElementById("loader");
      window.addEventListener("load", () => {
        loader.style.opacity = "0";
        setTimeout(() => loader.style.display = "none", 500);
      });
      if (document.readyState === "complete") {
        loader.style.opacity = "0";
        setTimeout(() => loader.style.display = "none", 500);
      }

      // --- Theme Toggle Matrix ---
      const themeToggle = document.getElementById("theme-toggle");
      const icon = themeToggle.querySelector("i");
      
      themeToggle.addEventListener("click", () => {
        let theme = document.documentElement.getAttribute("data-theme");
        let newTheme = theme === "dark" ? "light" : "dark";
        document.documentElement.setAttribute("data-theme", newTheme);
        icon.classList.toggle("fa-moon");
        icon.classList.toggle("fa-sun");
      });

      // --- Mobile Navbar Controls ---
      const hamburger = document.querySelector(".hamburger");
      const navLinks = document.querySelector(".picto-nav-links");

      hamburger.addEventListener("click", () => {
        navLinks.classList.toggle("mobile-active");
      });

      document.querySelectorAll(".picto-nav-links a").forEach(link => {
        link.addEventListener("click", () => navLinks.classList.remove("mobile-active"));
      });

      // --- Timeline Switching ---
      const tabButtons = document.querySelectorAll(".tab-btn");
      const timelines = document.querySelectorAll(".timeline-content");

      tabButtons.forEach(btn => {
        btn.addEventListener("click", () => {
          tabButtons.forEach(b => b.classList.remove("active"));
          timelines.forEach(t => t.classList.remove("active"));
          btn.classList.add("active");
          document.getElementById(`${btn.dataset.tab}-timeline`).classList.add("active");
        });
      });

      // --- Portfolio Sorting Engine ---
      const filterButtons = document.querySelectorAll(".filter-btn");
      const portfolioItems = document.querySelectorAll(".portfolio-item");

      filterButtons.forEach(btn => {
        btn.addEventListener("click", () => {
          filterButtons.forEach(b => b.classList.remove("active"));
          btn.classList.add("active");
          const filterValue = btn.getAttribute("data-filter");
          
          portfolioItems.forEach(item => {
            if (filterValue === "all" || item.getAttribute("data-category") === filterValue) {
              item.style.display = "block";
            } else {
              item.style.display = "none";
            }
          });
        });
      });

      // --- Viewport Intersection Observer (Counters & Progress Bars) ---
      const counters = document.querySelectorAll(".counter");
      const progressBars = document.querySelectorAll(".progress");
      const revealElements = document.querySelectorAll(".scroll-reveal");

      const observer = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            if (entry.target.classList.contains("scroll-reveal")) {
              entry.target.classList.add("reveal-active");
            }
            if (entry.target.classList.contains("progress")) {
              entry.target.style.width = entry.target.dataset.width;
            }
            if (entry.target.classList.contains("counter")) {
              const updateCount = () => {
                const target = +entry.target.getAttribute("data-target");
                const count = +entry.target.innerText;
                const speed = target / 80;
                if (count < target) {
                  entry.target.innerText = Math.ceil(count + speed);
                  setTimeout(updateCount, 20);
                } else {
                  entry.target.innerText = target + "+";
                }
              };
              updateCount();
            }
          }
        });
      }, { threshold: 0.1 });

      revealElements.forEach(el => observer.observe(el));
      counters.forEach(c => observer.observe(c));
      progressBars.forEach(p => observer.observe(p));

      // --- Scroll Top Logic ---
      const scrollTopBtn = document.getElementById("scroll-top");
      window.addEventListener("scroll", () => {
        if (window.scrollY > 400) scrollTopBtn.classList.add("visible");
        else scrollTopBtn.classList.remove("visible");
      });
      scrollTopBtn.addEventListener("click", () => window.scrollTo({ top: 0, behavior: "smooth" }));
    });

    // --- Modal Management Global Hooks ---
    function openModal(id) { document.getElementById(id).classList.add("active"); }
    function closeModal(id) { document.getElementById(id).classList.remove("active"); }
  </script>

