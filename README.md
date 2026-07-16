
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=1200, initial-scale=1.0">
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
      border: 1px solid var(--border-color);
      padding: 30px 50px 60px 50px;
      overflow: hidden;
      transition: background var(--transition-speed);
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
      color: var(--text-main);
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
      background-color: var(--bg-main);
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
      color: var(--text-muted);
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

    .highlight-purple { color: #9333ea; border-bottom: 1px dashed #c084fc; font-weight: 500; }
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
      background-color: var(--border-color);
      border: 4px solid var(--card-bg);
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
      background: var(--card-bg); border: 1px solid var(--border-color);
      padding: 8px 16px; border-radius: 30px; font-size: 0.9em;
      color: var(--text-main);
    }
    .about-tags span i { color: var(--accent-color); margin-right: 5px; }

    /* --- New Languages & Awards Layout Adjustments --- */
.awards-list {
  list-style: none;
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.awards-list li {
  display: flex;
  align-items: start;
  gap: 15px;
}

.awards-list li i {
  font-size: 1.2em;
  color: var(--accent-color);
  margin-top: 4px;
  width: 24px;
  text-align: center;
}

.awards-list li strong {
  display: block;
  font-size: 1.05em;
  color: var(--text-main);
  margin-bottom: 2px;
}

.awards-list li p {
  font-size: 0.9em;
  color: var(--text-muted);
  line-height: 1.4;
}

    /* --- Qualifications Cards --- */
    .qual-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(240px, 1fr)); gap: 25px; }
    .qual-card {
      background-color: var(--card-bg); border: 1px solid var(--border-color);
      border-radius: 16px; padding: 30px; position: relative;
      transition: transform 0.3s ease, box-shadow 0.3s ease, background var(--transition-speed);
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
      background: var(--card-bg); color: var(--text-main); font-weight: 600; cursor: pointer;
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
      background-color: var(--card-bg); border: 4px solid var(--primary-color); top: 25px; border-radius: 50%; z-index: 1;
    }
    .timeline-item.right .timeline-dot { left: -8px; }
    .timeline-date { font-weight: 700; color: var(--accent-color); margin-bottom: 8px; }
    .timeline-card { padding: 24px; background-color: var(--card-bg); border-radius: 12px; border: 1px solid var(--border-color); transition: background var(--transition-speed); }
    .timeline-card h3 { font-size: 1.2em; margin-bottom: 4px; }
    .timeline-card h4 { font-size: 0.95em; color: var(--secondary-color); font-weight: 500; margin-bottom: 10px; }
    .timeline-card p { font-size: 0.9em; color: var(--text-muted); line-height: 1.5; }

    /* --- Skills Matrix Mechanics --- */
    .skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(320px, 1fr)); gap: 40px; }
    .skills-category { background: var(--card-bg); border: 1px solid var(--border-color); border-radius: 16px; padding: 30px; transition: background var(--transition-speed); }
    .skills-category h3 { font-size: 1.3em; margin-bottom: 25px; color: var(--primary-color); display: flex; align-items: center; gap: 10px; }
    .skill-item { margin-bottom: 20px; }
    .skill-info { display: flex; justify-content: space-between; margin-bottom: 8px; font-size: 0.9em; font-weight: 500; }
    .progress-bar { width: 100%; height: 6px; background-color: var(--border-color); border-radius: 3px; overflow: hidden; }
    .progress { height: 100%; background: linear-gradient(90deg, var(--primary-color), var(--secondary-color)); width: 0; transition: width 1.5s cubic-bezier(0.1, 1, 0.1, 1); }

    /* --- Certifications Strip --- */
    .certs-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(260px, 1fr)); gap: 15px; }
    .cert-item-card { background: var(--card-bg); border: 1px solid var(--border-color); padding: 16px 20px; border-radius: 8px; display: flex; align-items: center; gap: 15px; font-size: 0.9em; font-weight: 500; transition: background var(--transition-speed); }
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
    .research-card { background: var(--card-bg); border: 1px solid var(--border-color); border-radius: 16px; padding: 40px; transition: background var(--transition-speed); }
    .research-header { display: flex; align-items: center; gap: 20px; margin-bottom: 20px; border-bottom: 1px solid var(--border-color); padding-bottom: 20px; }
    .research-header i { font-size: 2.5em; color: var(--primary-color); }
    .research-header h3 { font-size: 1.5em; line-height: 1.4; }
    .research-body p { color: var(--text-muted); line-height: 1.6; margin-bottom: 20px; }
    .research-details { display: flex; flex-direction: column; gap: 12px; }
    .research-details span { font-size: 0.95em; line-height: 1.5; }

    /* --- Premium Picto Contact Section Styles --- */
    .picto-contact-section {
      position: relative;
      width: 100%;
      margin-top: 60px;
      border-radius: 24px;
      overflow: hidden;
      box-shadow: 0 10px 30px rgba(0, 0, 0, 0.02);
    }

    /* Purple Top Header Section */
    .contact-header-bg {
      background: linear-gradient(135deg, #a855f7 0%, #7e22ce 100%);
      color: white;
      text-align: center;
      padding: 60px 20px 60px 20px; 
      position: relative; 
      z-index: 2; 
    }

    .contact-main-title,
    .contact-subtitle {
      position: relative;
      z-index: 2; 
    }

    .contact-main-title {
      font-size: 3em;
      font-weight: 700;
      margin-bottom: 15px;
      color: #fff !important;
    }

    .contact-subtitle {
      font-size: 1.1em;
      max-width: 650px;
      margin: 0 auto;
      opacity: 0.9;
      line-height: 1.6;
    }

    /* White Bottom Background Container */
    .contact-split-container {
      background-color: var(--card-bg);
      position: relative;
      margin-top: 0; 
      z-index: 2;
      padding: 50px 50px 80px 50px; 
      transition: background var(--transition-speed);
    }

    /* Controls Side-by-Side Grid Layout balance */
    .contact-grid-wrapper {
      position: relative;
      z-index: 3;
      display: grid;
      grid-template-columns: 1.15fr 0.85fr; 
      gap: 50px;
      align-items: start; 
      max-width: 1100px;
      margin: 0 auto;
    }

    /* Mock Browser Container Style */
    .mock-browser-window {
      background: var(--card-bg);
      border: 2px solid var(--text-main);
      border-radius: 16px;
      overflow: hidden;
      box-shadow: 0 15px 35px rgba(0, 0, 0, 0.05);
      transition: border-color var(--transition-speed), background var(--transition-speed);
    }

    /* Browser Window Top Bar */
    .browser-header {
      background-color: rgba(147, 51, 234, 0.12);
      border-bottom: 2px solid var(--text-main);
      padding: 12px 24px;
      display: flex;
      justify-content: flex-end;
      align-items: center;
      transition: border-color var(--transition-speed);
    }

    .browser-controls {
      display: flex;
      gap: 12px;
      font-size: 1.2em;
      font-weight: 600;
      color: var(--text-main);
      cursor: default;
    }

    .browser-controls span {
      display: inline-block;
      line-height: 1;
    }

    /* Browser Window Form Content Box */
    .browser-body {
      padding: 40px; 
      display: flex;
      flex-direction: column;
      gap: 24px;
    }

    /* Form Input Layout Fields */
    .form-row {
      display: flex;
      align-items: center;
      gap: 20px;
    }

    .form-row label {
      font-size: 1.05em;
      font-weight: 600;
      color: var(--text-main);
      width: 110px; 
      flex-shrink: 0;
    }

    .form-row input, .message-row textarea {
      width: 100%;
      padding: 12px 18px;
      border: 1.5px solid var(--border-color);
      border-radius: 10px;
      font-family: inherit;
      font-size: 0.95em;
      color: #1e2530; 
      background-color: #fff;
      transition: border-color 0.25s ease;
    }

    .form-row input:focus, .message-row textarea:focus {
      outline: none;
      border-color: var(--primary-color);
      box-shadow: 0 0 0 3px rgba(147, 51, 234, 0.1);
    }

    .message-row {
      align-items: flex-start;
    }

    .message-row label {
      margin-top: 10px;
    }

    .message-row textarea {
      resize: none;
    }

    .form-submit-row {
      display: flex;
      justify-content: center;
      margin-top: 10px;
    }

    /* Modern Rounded Pill Button */
    .btn-browser-send {
      background-color: var(--primary-color);
      color: #ffffff;
      border: none;
      padding: 12px 40px;
      border-radius: 50px;
      font-family: inherit;
      font-weight: 600;
      font-size: 0.95em;
      cursor: pointer;
      box-shadow: 0 4px 15px rgba(147, 51, 234, 0.2);
      transition: all 0.25s ease;
      width: 100%; 
    }

    .btn-browser-send:hover {
      background-color: var(--primary-hover);
      transform: translateY(-2px);
      box-shadow: 0 6px 20px rgba(147, 51, 234, 0.3);
    }

    .contact-info-panel {
      padding-left: 20px;
    }

    .info-list {
      display: flex;
      flex-direction: column;
      gap: 25px;
      margin-bottom: 40px;
    }

    .info-item {
      display: flex;
      align-items: center;
      gap: 20px;
      font-size: 1.1em;
    }

    .info-item i {
      font-size: 1.4em;
      color: var(--primary-color);
      width: 30px;
      text-align: center;
    }

    .info-item span, .info-item a {
      color: var(--text-main);
      text-decoration: none;
      font-weight: 500;
    }

    .info-item a:hover {
      color: var(--primary-color);
    }

    .info-social-row {
      display: flex;
      gap: 14px;
      padding-left: 8px;
      flex-wrap: wrap;
    }

    .info-social-row a {
      width: 45px;
      height: 45px;
      border-radius: 50%;
      background-color: var(--border-color);
      color: var(--text-main);
      display: flex;
      justify-content: center;
      align-items: center;
      text-decoration: none;
      transition: all 0.25s ease;
      font-size: 1.2em;
    }

    .info-social-row a:hover {
      background-color: var(--primary-color);
      color: white;
      transform: translateY(-3px);
    }

    /* Dark mode configurations */
    [data-theme="dark"] .contact-split-container,
    [data-theme="dark"] .mock-browser-window {
      background-color: #1e293b;
    }

    [data-theme="dark"] .mock-browser-window {
      border-color: #fff;
    }

    [data-theme="dark"] .browser-header {
      border-bottom-color: #fff;
    }

    [data-theme="dark"] .form-row input, 
    [data-theme="dark"] .message-row textarea {
      background-color: #0f172a;
      border-color: rgba(255, 255, 255, 0.15);
      color: #f8fafc; 
    }

    [data-theme="dark"] .form-row input::placeholder, 
    [data-theme="dark"] .message-row textarea::placeholder {
      color: #64748b; 
    }

    /* --- Responsive Adjustments --- */
    @media (max-width: 992px) {
      .contact-grid-wrapper {
        grid-template-columns: 1fr;
        gap: 40px;
      }
      .contact-split-container {
        padding: 0 20px 60px 20px;
      }
      .contact-info-panel {
        padding-left: 0;
        display: flex;
        flex-direction: column;
        align-items: center;
        text-align: center;
      }
      .info-list {
        align-items: center;
      }
    }

    @media (max-width: 576px) {
      .browser-body {
        padding: 25px 20px;
      }
      .form-row {
        flex-direction: column;
        align-items: flex-start;
        gap: 8px;
      }
      .form-row label {
        width: auto;
      }
      .contact-main-title {
        font-size: 2.2em;
      }
    }

    /* --- Modal Overlay Design --- */
    .modal-overlay { position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.5); backdrop-filter: blur(4px); z-index: 2000; display: flex; justify-content: center; align-items: center; opacity: 0; visibility: hidden; transition: all 0.3s ease; }
    .modal-overlay.active { opacity: 1; visibility: visible; }
    .modal-card { background: var(--card-bg); padding: 40px; border-radius: 16px; max-width: 500px; width: 90%; position: relative; box-shadow: 0 10px 30px rgba(0,0,0,0.1); color: var(--text-main); }
    .close-modal { position: absolute; top: 20px; right: 25px; font-size: 2em; cursor: pointer; color: var(--text-muted); }

    /* --- Premium Picto Footer Styles --- */
    .picto-footer {
      margin-top: 80px;
      width: 100%;
    }

    .footer-divider {
      width: 100%;
      height: 1px;
      background-color: var(--border-color);
      margin-bottom: 40px;
    }

    .picto-footer-grid {
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
      gap: 30px;
      padding-bottom: 30px;
    }

    .picto-footer-info h3 {
      font-size: 1.4em;
      font-weight: 700;
      color: var(--text-main);
      margin-bottom: 5px;
    }

    .picto-footer-info p {
      font-size: 0.9em;
      color: var(--text-muted);
      margin: 0;
    }

    .picto-footer-links {
      display: flex;
      gap: 30px;
    }

    .picto-footer-links a {
      text-decoration: none;
      color: var(--text-muted);
      font-weight: 500;
      font-size: 0.92em;
      transition: color 0.25s ease;
    }

    .picto-footer-links a:hover {
      color: var(--primary-color);
    }

    .picto-footer-bottom {
      border-top: 1px solid var(--border-color);
      padding-top: 20px;
      text-align: center;
    }

    .picto-footer-bottom p {
      font-size: 0.85em;
      color: var(--text-muted);
      margin: 0;
    }

    @media (max-width: 768px) {
      .picto-footer-grid {
        flex-direction: column;
        text-align: center;
        gap: 20px;
      }
      .picto-footer-links {
        justify-content: center;
        gap: 20px;
      }
    }

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
    }

    @media (max-width: 768px) {
      .picto-nav-links {
        position: absolute; top: 100%; left: 0; width: 100%;
        background-color: var(--card-bg); flex-direction: column; text-align: center;
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
         I'm an English <span class="highlight-purple">Educator</span>, <span class="highlight-pink">Content Creator</span>, and Video Editor based in Chiang Mai, Thailand. Passionate about education and innovation, I create engaging learning experiences that combine communicative teaching, educational technology, and creative digital content. My mission is to empower learners with the confidence and skills they need to succeed in today's global world.
        </p>
        
        <a href="#contact" class="btn-picto-purple">Contact Me</a>

        <!-- Counter Metric Nodes directly under introduction text -->
        <div class="picto-mini-stats">
          <div class="mini-stat-item">
            <div class="counter" data-target="4" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Years Exp.</p>
          </div>
          <div class="mini-stat-item">
            <div class="counter" data-target="2000" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Students Taught</p>
          </div>
          <div class="mini-stat-item">
            <div class="counter" data-target="85" style="font-size: 1.6em; font-weight: 700;">0</div>
            <p>Certificates</p>
          </div>
        </div>
      </div>

      <div class="picto-hero-right">
        <div class="picto-img-container">
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

    <!-- Languages & Awards Section Split -->
<section id="languages-awards" class="container-box scroll-reveal">
  <div class="skills-grid">

    <!-- Left Column: Language Proficiencies -->
    <div class="skills-category">
      <h3><i class="fas fa-globe"></i> Languages</h3>

      <div class="skill-item">
        <div class="skill-info">
          <span>English</span>
          <span>Fluent / Academic</span>
        </div>
        <div class="progress-bar">
          <div class="progress" data-width="95%"></div>
        </div>
      </div>

      <div class="skill-item">
        <div class="skill-info">
          <span>Myanmar (Burmese)</span>
          <span>Native / Bilingual</span>
        </div>
        <div class="progress-bar">
          <div class="progress" data-width="100%"></div>
        </div>
      </div>

      <div class="skill-item">
        <div class="skill-info">
          <span>Mon</span>
          <span>Native / Bilingual</span>
        </div>
        <div class="progress-bar">
          <div class="progress" data-width="100%"></div>
        </div>
      </div>

      <div class="skill-item">
        <div class="skill-info">
          <span>Thai</span>
          <span>Conversational</span>
        </div>
        <div class="progress-bar">
          <div class="progress" data-width="65%"></div>
        </div>
      </div>
    </div>

    <!-- Right Column: Awards & Recognitions -->
<div class="skills-category">
  <h3><i class="fas fa-trophy" style="color: var(--accent-color);"></i> Achievements & Awards</h3>
  
  <ul class="awards-list">
    <li>
      <i class="fas fa-graduation-cap"></i>
      <div>
        <strong>Scholarships</strong>
        <p style="line-height: 1.6; margin-top: 4px;">
          • United Board Scholar (Fully Funded)<br>
          • Former IIE Scholar (2025)<br>
          • Former DISP Scholar (2024)<br>
          • Former National University of Zoland Scholar
        </p>
      </div>
    </li>
    <li>
      <i class="fas fa-medal"></i>
      <div>
        <strong>Competitions</strong>
        <p>Recognition achieved in public speaking, creative content, or academic skill events.</p>
      </div>
    </li>
    <li>
      <i class="fas fa-certificate"></i>
      <div>
        <strong>Official Recognition</strong>
        <p>Special commendations from university leadership, council boards, or voluntary groups.</p>
      </div>
    </li>
    <li>
      <i class="fas fa-award"></i>
      <div>
        <strong>Academic Awards</strong>
        <p>Top performance honors received during outstanding degree pathways and diploma milestones.</p>
      </div>
    </li>
  </ul>
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
          <div class="qual-icon"><i class="fas fa-square-root-alt"></i></div>
          <span class="qual-status complete">Completed</span>
          <h3>Mathematics Studies (Second Year)</h3>
          <p>Completed two years of undergraduate study in Mathematics at Hpa-An University, Myanmar, developing strong analytical, logical reasoning, and problem-solving skills.</p>
        </div>

        <div class="qual-card">
          <div class="qual-icon"><i class="fas fa-school"></i></div>
          <span class="qual-status complete">Graduated</span>
          <h3>High School Education</h3>
          <p>Completed Basic Education High School in Myanmar, building a strong academic foundation in mathematics, science, languages, and social studies.</p>
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
              <h4>Social Media Platforms</h4>
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
              <h3>Student Leader</h3>
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
              <h4>Mon Intensive English Program</h4>
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
            <div class="timeline-date">2025</div>
            <div class="timeline-card">
              <h3>Community Service Volunteer</h3>
              <h4>Ban San San School, Chiang Mai</h4>
              <p>
                Participated in a community outreach program organized by Payap University. Supported young learners through educational activities, creative art sessions, and donations while promoting an engaging and inclusive learning environment.
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>
      
    <!-- Skills Section -->
    <section id="skills" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Professional Skills</h2>
        <div class="title-line"></div>
      </div>

      <div class="skills-grid">
        <!-- Teaching Skills -->
        <div class="skills-category">
          <h3><i class="fas fa-chalkboard-teacher"></i> Teaching & Education</h3>

          <div class="skill-item">
            <div class="skill-info">
              <span>Lesson Planning & Instruction</span>
              <span>95%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="95%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Classroom Management</span>
              <span>92%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="92%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Curriculum Development</span>
              <span>90%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="90%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Online Teaching</span>
              <span>96%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="96%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Student Assessment & Feedback</span>
              <span>90%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="90%"></div>
            </div>
          </div>
        </div>

        <!-- Digital Skills -->
        <div class="skills-category">
          <h3><i class="fas fa-laptop-code"></i> Digital & Creative Skills</h3>

          <div class="skill-item">
            <div class="skill-info">
              <span>Canva & Graphic Design</span>
              <span>95%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="95%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Video Editing (CapCut & Premiere Pro)</span>
              <span>90%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="90%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Zoom & Google Workspace</span>
              <span>95%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="95%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Content Creation & Social Media</span>
              <span>94%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="94%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>Photography</span>
              <span>85%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="85%"></div>
            </div>
          </div>

          <div class="skill-item">
            <div class="skill-info">
              <span>AI Tools for Education</span>
              <span>90%</span>
            </div>
            <div class="progress-bar">
              <div class="progress" data-width="90%"></div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Professional Certifications Grid -->
    <section id="certifications" class="container-box scroll-reveal">
      <div class="section-title">
        <h2>Professional Certifications</h2>
        <div class="title-line"></div>
      </div>

      <div class="certs-grid">
        <!-- Teaching -->
        <div class="cert-item-card">
          <i class="fas fa-medal gold-icon"></i>
          <span>TEFL/TESOL Certification (2026)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-child"></i>
          <span>Teaching English to Young Learners (2026)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-hands-helping"></i>
          <span>Teaching English to Refugees and Displaced Learners</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-volume-up"></i>
          <span>Teaching English: How to Teach Pronunciation</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-clipboard-check"></i>
          <span>Teaching English: Assessing Learning</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-book-open"></i>
          <span>Teaching English: How to Adapt Resources</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-laptop-house"></i>
          <span>Teaching Online</span>
        </div>

        <!-- Education -->
        <div class="cert-item-card">
          <i class="fas fa-graduation-cap"></i>
          <span>English Four Skills (2018)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-brain"></i>
          <span>Exploring Learning Disabilities</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-language"></i>
          <span>Teaching English in Primary Classrooms</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-comments"></i>
          <span>Teaching English: Communicative Tasks</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-headphones"></i>
          <span>Teaching English: How to Teach Listening</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-laptop"></i>
          <span>Teaching English: Integrating Technology</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-book-reader"></i>
          <span>Teaching English: Understanding Language Systems</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-user-graduate"></i>
          <span>Teaching English: Helping Teachers to Learn</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-bullhorn"></i>
          <span>Foundations of Digital Marketing & E-Commerce</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-users"></i>
          <span>Attract and Engage Customers with Digital Marketing</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-handshake"></i>
          <span>Interact with Customers Online</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-heart"></i>
          <span>Develop Customer Loyalty Online</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-chart-line"></i>
          <span>Marketing Analytics and Measurement</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-share-alt"></i>
          <span>Social Media Marketing</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-envelope"></i>
          <span>Email Marketing</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-shopping-cart"></i>
          <span>Make the Sale</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-school"></i>
          <span>Inclusive Education</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-venus-mars"></i>
          <span>Gender in Language Education</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-child"></i>
          <span>Supporting Children's Mental Health and Well-being</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-users-cog"></i>
          <span>Leadership and Followership</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-star"></i>
          <span>Effective Leadership</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-comments"></i>
          <span>Effective Communication in the Workplace</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-chalkboard"></i>
          <span>Effective Presentations</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-user-friends"></i>
          <span>Professional Networking for Career Growth</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-users"></i>
          <span>Working in Teams</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-hands-helping"></i>
          <span>Working in the Voluntary Sector</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-robot"></i>
          <span>Job Search with AI</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-balance-scale"></i>
          <span>Becoming an Ethical Researcher</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-gavel"></i>
          <span>Introduction to Human Rights Standards</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-shield-alt"></i>
          <span>Child Protection Advocacy</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-book"></i>
          <span>Child Rights Toolkit</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-briefcase"></i>
          <span>English for Career Development</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-plane"></i>
          <span>English for Tourism Professionals</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-desktop"></i>
          <span>Digital Skills: Succeeding in a Digital World</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-users"></i>
          <span>Introduction to Social Sciences</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-user-friends"></i>
          <span>Diversity and Inclusion in the Workplace</span>
        </div>

        <!-- Technology -->
        <div class="cert-item-card">
          <i class="fab fa-google text-blue"></i>
          <span>Google Digital Marketing & E-Commerce (2025)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-laptop-code"></i>
          <span>I-Office Computer (2019)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-chalkboard-teacher"></i>
          <span>Mastering E-Learning Designs for Modern Educators (2025)</span>
        </div>

        <!-- Professional Development -->
        <div class="cert-item-card">
          <i class="fas fa-chart-line"></i>
          <span>Career Advancement (2024)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-heart"></i>
          <span>Stress Management and Self-Care (2025)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-globe"></i>
          <span>Localization in Humanitarian Aid (2025)</span>
        </div>

        <div class="cert-item-card">
          <i class="fas fa-coins"></i>
          <span>Financial Literacy (2018)</span>
        </div>
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
    
    <!-- ITEM 1 (2026) - Media & Content -->
    <div class="portfolio-item" data-category="media" onclick="openModal('modal-p1')">
      <!-- REPLACE with your actual image file (e.g., info_graphic.jpg) -->
      <img src="english_infographic.jpg" alt="English Learning Infographic" onerror="this.src='https://via.placeholder.com/400x300?text=English+Infographic'">
      <div class="portfolio-overlay">
        <h4>Instructional Media Campaign</h4>
        <p>2026 • Graphic design & infographic assets for advanced language learning modules.</p>
      </div>
    </div>

    <!-- ITEM 2 (2026) - Teaching -->
    <div class="portfolio-item" data-category="teaching" onclick="openModal('modal-p2')">
      <!-- REPLACE with your actual image file (e.g., class_launch.jpg) -->
      <img src="poy_english_launch.jpg" alt="Poy English Course Announcement" onerror="this.src='https://via.placeholder.com/400x300?text=Poy+English+Launch'">
      <div class="portfolio-overlay">
        <h4>Poy English Level 4 Launch</h4>
        <p>2026 • Interactive digital infrastructure and class announcement management systems.</p>
      </div>
    </div>

    <!-- ITEM 3 (2025) - Media & Content -->
    <div class="portfolio-item" data-category="media" onclick="openModal('modal-p3')">
      <!-- REPLACE with your actual image file (e.g., video_edit.jpg) -->
      <img src="ethnoverse_content.jpg" alt="EthnoVerse Digital Content" onerror="this.src='https://via.placeholder.com/400x300?text=EthnoVerse+Media'">
      <div class="portfolio-overlay">
        <h4>AI-Assisted Educational Media</h4>
        <p>2025 • Short-form video editing and multimedia historical storytelling pipelines for EthnoVerse.</p>
      </div>
    </div>

    <!-- ITEM 4 (2019-Present) - Teaching -->
    <div class="portfolio-item" data-category="teaching" onclick="openModal('modal-p4')">
      <!-- REPLACE with your actual image file (e.g., online_class.jpg) -->
      <img src="online_instruction.jpg" alt="Online English Class Setup" onerror="this.src='https://via.placeholder.com/400x300?text=Online+Instruction'">
      <div class="portfolio-overlay">
        <h4>Poy English Program Delivery</h4>
        <p>2019 – Present • Student-centered online language instruction architectures via Zoom and Google Meet.</p>
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

    <!-- Contact Section -->
    <section id="contact" class="picto-contact-section scroll-reveal">
      
      <!-- Top Title Block inside the Purple Background -->
      <div class="contact-header-bg">
        <h2 class="contact-main-title">Connect with Me</h2>
        <p class="contact-subtitle">Have a project, a job opening, or just want to say hello? Drop me a message below!</p>
      </div>

      <!-- Lower Split Area containing Form and Info -->
      <div class="contact-split-container">
        <div class="contact-grid-wrapper">
          
          <!-- Left Side: Mock Browser Form Window -->
          <form class="mock-browser-window" action="https://formspree.io/f/mqereerd" method="POST">
            <!-- Window Control Header Bar -->
            <div class="browser-header">
              <div class="browser-controls">
                <span>&minus;</span>
                <span>&#9634;</span>
                <span>&times;</span>
              </div>
            </div>
            
            <!-- Form Content Fields Area -->
            <div class="browser-body">
              <div class="form-row">
                <label for="name">Your Name:</label>
                <input type="text" id="name" name="name" required placeholder="Enter your full name">
              </div>
              
              <div class="form-row">
                <label for="email">Your Gmail:</label>
                <input type="email" id="email" name="email" required placeholder="Enter your mail id">
              </div>
              
              <div class="form-row message-row">
                <label for="message">Message:</label>
                <textarea id="message" name="message" rows="5" required placeholder="Enter your message"></textarea>
              </div>

              <div class="form-submit-row">
                <button type="submit" class="btn-browser-send">Send</button>
              </div>
            </div>
          </form>

          <!-- Right Side: Clean Contact Info & Socials -->
          <div class="contact-info-panel">
            <div class="info-list">
              <div class="info-item">
                <i class="fas fa-phone-alt"></i>
                <span>0924854332</span>
              </div>
              <div class="info-item">
                <i class="fas fa-envelope"></i>
                <a href="mailto:minwinmoe123@gmail.com">minwinmoe123@gmail.com</a>
              </div>
              <div class="info-item">
                <i class="fas fa-map-marker-alt"></i>
                <span>Chiang Mai, Thailand</span>
              </div>
            </div>

            <!-- Horizontal Social Icons Row -->
            <div class="info-social-row">
              <a href="https://www.linkedin.com/in/win-moe-73b006395" target="_blank" aria-label="LinkedIn">
                <i class="fab fa-linkedin-in"></i>
              </a>
              <a href="https://facebook.com/winmoe.wmwm" target="_blank" aria-label="Facebook Personal">
                <i class="fab fa-facebook-f"></i>
              </a>
              <a href="https://www.facebook.com/share/1DCQUzoTtw/?mibextid=wwXIfr" target="_blank" aria-label="Facebook Page">
                <i class="fab fa-facebook"></i>
              </a>
              <a href="https://tiktok.com/@poyenglish" target="_blank" aria-label="TikTok">
                <i class="fab fa-tiktok"></i>
              </a>
              <a href="https://www.youtube.com/@hongsarpoy" target="_blank" aria-label="YouTube">
                <i class="fab fa-youtube"></i>
              </a>
            </div>
          </div>

        </div>
      </div>
    </section>
      
    <!-- Unified Footer Construction -->
    <footer class="picto-footer">
      <div class="footer-divider"></div>
      <div class="picto-footer-grid">
        <div class="picto-footer-info">
          <h3>Win Moe</h3>
          <p>English Instructor & Content Creator</p>
        </div>
        <div class="picto-footer-links">
          <a href="#home">Home</a>
          <a href="#about">About</a>
          <a href="#portfolio">Portfolio</a>
          <a href="#contact">Contact</a>
        </div>
      </div>
      <div class="picto-footer-bottom">
        <p>&copy; 2026 Win Moe. All Rights Reserved. Portfolio Site.</p>
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
