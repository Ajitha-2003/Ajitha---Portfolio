# Ajitha---Portfolio
Portfolio
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ajitha L — AI Developer & ML Engineer | LLM Integration | Python | Flask</title>
<meta name="description" content="Ajitha L — AI Developer and Machine Learning Engineer. Expert in LLM integration, Python, Flask, RAG pipelines, prompt engineering, and AI-powered automation. Based in Coimbatore, India.">
<meta name="keywords" content="AI Developer, Machine Learning Engineer, LLM Integration, Python Developer, Flask, OpenAI API, LangChain, Prompt Engineering, RAG, Vector Database, FAISS, NLP, Generative AI, MLOps, QA Automation, Coimbatore">
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500;600&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --black: #0d0d0d;
    --white: #fafaf8;
    --accent: #2563eb;
    --accent2: #1d4ed8;
    --muted: #6b7280;
    --border: rgba(0,0,0,0.08);
    --card-bg: #ffffff;
    --page-bg: #f6f5f2;
    --tag-bg: #eff6ff;
    --tag-color: #1d4ed8;
  }
  * { margin: 0; padding: 0; box-sizing: border-box; }
  html { scroll-behavior: smooth; }
  body { font-family: 'DM Sans', sans-serif; background: var(--page-bg); color: var(--black); font-size: 16px; line-height: 1.6; -webkit-font-smoothing: antialiased; }

  /* ══ NAVBAR ══ */
  nav {
    position: fixed; top: 0; left: 0; right: 0; z-index: 100;
    background: rgba(246,245,242,0.88);
    backdrop-filter: blur(18px); -webkit-backdrop-filter: blur(18px);
    border-bottom: 1px solid rgba(37,99,235,0.10);
    padding: 0 5%;
    display: flex; align-items: center; justify-content: space-between;
    height: 60px;
  }
  nav::before {
    content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
    background: linear-gradient(90deg, #2563eb 0%, #7c3aed 50%, #db2777 100%);
  }
  .nav-logo { display: flex; align-items: center; gap: 10px; text-decoration: none; }
  .nav-logo-mark {
    width: 34px; height: 34px; border-radius: 9px;
    background: linear-gradient(135deg, #2563eb, #7c3aed);
    display: flex; align-items: center; justify-content: center;
    color: #fff; font-family: 'DM Serif Display', serif; font-size: 1rem;
    box-shadow: 0 2px 8px rgba(37,99,235,0.28);
  }
  .nav-name { font-family: 'DM Serif Display', serif; font-size: 1.1rem; color: var(--black); letter-spacing: -0.02em; }
  .nav-links { display: flex; gap: 0.2rem; list-style: none; }
  .nav-links li a {
    color: var(--muted); text-decoration: none; font-size: 0.84rem;
    font-weight: 500; padding: 6px 13px; border-radius: 8px;
    transition: color 0.2s, background 0.2s;
    display: flex; align-items: center;
  }
  .nav-links li a:hover { color: var(--black); background: rgba(37,99,235,0.06); }
  .nav-links li a.active { color: var(--accent); background: var(--tag-bg); }
  .nav-cta {
    background: var(--accent) !important; color: #fff !important;
    box-shadow: 0 2px 8px rgba(37,99,235,0.3);
    transition: background 0.2s, transform 0.15s !important;
  }
  .nav-cta:hover { background: var(--accent2) !important; transform: translateY(-1px) !important; color: #fff !important; }

  /* ══ SECTIONS — tighter spacing ══ */
  section { padding: 60px 5%; max-width: 1120px; margin: 0 auto; }

  /* ══ HERO — full 50/50 split ══ */
  .hero {
    display: grid; grid-template-columns: 1fr 1fr;
    min-height: 100vh; max-width: 100%; overflow: hidden;
  }
  .hero-left {
    display: flex; flex-direction: column; justify-content: center;
    padding: 100px 6% 60px 8%; position: relative; z-index: 2;
  }
  .hero-right {
    position: relative;
    background: linear-gradient(148deg, #dbeafe 0%, #ede9fe 48%, #fce7f3 100%);
    overflow: hidden;
  }
  .hero-right::before {
    content: ''; position: absolute; inset: 0;
    background: radial-gradient(ellipse at 65% 35%, rgba(37,99,235,0.14) 0%, transparent 60%),
                radial-gradient(ellipse at 30% 75%, rgba(124,58,237,0.12) 0%, transparent 55%);
  }
  .hero-right::after {
    content: ''; position: absolute; inset: 0;
    background-image: radial-gradient(circle, rgba(37,99,235,0.2) 1px, transparent 1px);
    background-size: 26px 26px; opacity: 0.55;
  }
  #avatar-canvas { position: absolute; inset: 0; width: 100% !important; height: 100% !important; z-index: 1; }

  .hero-badge {
    position: absolute; z-index: 2;
    background: rgba(255,255,255,0.93);
    border: 1px solid rgba(255,255,255,0.65);
    border-radius: 11px; padding: 9px 15px;
    backdrop-filter: blur(10px);
    box-shadow: 0 4px 18px rgba(0,0,0,0.09);
    font-size: 0.77rem; font-weight: 600; color: var(--black);
    display: flex; align-items: center; gap: 7px;
    animation: floatBadge 4s ease-in-out infinite;
    white-space: nowrap;
  }
  .hero-badge .dot { width: 7px; height: 7px; border-radius: 50%; flex-shrink: 0; }
  .hero-badge:nth-of-type(1) { top: 16%; left: 7%; animation-delay: 0s; }
  .hero-badge:nth-of-type(2) { top: 36%; right: 7%; animation-delay: 1s; }
  .hero-badge:nth-of-type(3) { bottom: 30%; left: 10%; animation-delay: 2s; }
  .hero-badge:nth-of-type(4) { bottom: 13%; right: 9%; animation-delay: 0.6s; }
  @keyframes floatBadge { 0%,100%{transform:translateY(0)} 50%{transform:translateY(-8px)} }

  .hero-tag {
    display: inline-flex; align-items: center; gap: 6px;
    background: var(--tag-bg); color: var(--tag-color);
    padding: 4px 14px; border-radius: 100px;
    font-size: 0.73rem; font-weight: 600; letter-spacing: 0.08em;
    text-transform: uppercase; margin-bottom: 1.2rem;
    border: 1px solid rgba(37,99,235,0.15); width: fit-content;
  }
  .hero-tag::before {
    content: ''; width: 6px; height: 6px; border-radius: 50%;
    background: var(--accent); animation: pulse 2s infinite;
  }
  @keyframes pulse { 0%,100%{opacity:1;transform:scale(1)} 50%{opacity:0.35;transform:scale(0.72)} }

  h1 {
    font-family: 'DM Serif Display', serif;
    font-size: clamp(2.6rem, 4.8vw, 5rem);
    line-height: 1.0; letter-spacing: -0.03em;
    margin-bottom: 1rem; color: var(--black);
  }
  h1 em { color: var(--accent); font-style: normal; }

  .hero-sub {
    font-size: 1.02rem; color: var(--muted);
    max-width: 460px; margin-bottom: 1.875rem;
    font-weight: 300; line-height: 1.78;
  }
  .hero-btns { display: flex; gap: 0.75rem; flex-wrap: wrap; }
  .btn-primary {
    background: var(--black); color: #fff;
    padding: 11px 26px; border-radius: 8px;
    text-decoration: none; font-weight: 500; font-size: 0.875rem;
    transition: transform 0.15s, box-shadow 0.15s;
  }
  .btn-primary:hover { transform: translateY(-2px); box-shadow: 0 8px 24px rgba(0,0,0,0.18); }
  .btn-outline {
    background: transparent; color: var(--black);
    padding: 11px 26px; border-radius: 8px;
    text-decoration: none; font-weight: 500; font-size: 0.875rem;
    border: 1.5px solid rgba(0,0,0,0.2);
    transition: border-color 0.15s, background 0.15s;
  }
  .btn-outline:hover { border-color: var(--black); background: rgba(0,0,0,0.03); }

  .hero-contacts { display: flex; flex-wrap: wrap; gap: 0.45rem; margin-top: 1.4rem; }
  .hero-contact-item {
    display: inline-flex; align-items: center; gap: 5px;
    font-size: 0.74rem; color: var(--muted); text-decoration: none;
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 7px; padding: 5px 10px;
    transition: border-color 0.2s, color 0.2s, transform 0.15s, box-shadow 0.15s;
    font-weight: 500;
  }
  .hero-contact-item:hover { color: var(--accent); border-color: rgba(37,99,235,0.35); transform: translateY(-2px); box-shadow: 0 4px 12px rgba(37,99,235,0.09); }
  .hero-contact-item svg { color: var(--muted); transition: color 0.2s; }
  .hero-contact-item:hover svg { color: var(--accent); }

  /* ══ SECTION HEADERS ══ */
  .section-label { font-size: 0.68rem; font-weight: 700; letter-spacing: 0.14em; text-transform: uppercase; color: var(--accent); margin-bottom: 0.45rem; }
  h2 { font-family: 'DM Serif Display', serif; font-size: clamp(1.65rem, 2.8vw, 2.4rem); letter-spacing: -0.02em; line-height: 1.15; margin-bottom: 1.2rem; color: var(--black); }

  /* ══ ABOUT ══ */
  .about-grid { display: grid; grid-template-columns: 1fr 1.55fr; gap: 3rem; align-items: start; }
  .about-stat-row { display: flex; flex-direction: column; gap: 0.875rem; }
  .stat-card {
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 12px; padding: 1.1rem 1.4rem;
    transition: transform 0.2s, box-shadow 0.2s;
    border-left: 3px solid var(--accent);
  }
  .stat-card:hover { transform: translateY(-3px); box-shadow: 0 8px 22px rgba(0,0,0,0.07); }
  .stat-num { font-family: 'DM Serif Display', serif; font-size: 2.1rem; color: var(--accent); line-height: 1; margin-bottom: 2px; }
  .stat-desc { font-size: 0.82rem; color: var(--muted); }
  .about-text p { color: #374151; line-height: 1.8; margin-bottom: 0.825rem; font-size: 0.925rem; }
  .about-text p:last-child { margin-bottom: 0; }

  /* ══ SKILLS ══ */
  .skills-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(258px, 1fr)); gap: 1.1rem; margin-top: 1.6rem; }
  .skill-card {
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 12px; padding: 1.25rem;
    transition: transform 0.2s, box-shadow 0.2s;
    position: relative; overflow: hidden;
  }
  .skill-card::after {
    content: ''; position: absolute; top: 0; left: 0; right: 0; height: 2px;
    background: linear-gradient(90deg, var(--accent), #7c3aed);
    transform: scaleX(0); transform-origin: left; transition: transform 0.3s;
  }
  .skill-card:hover { transform: translateY(-4px); box-shadow: 0 10px 28px rgba(0,0,0,0.08); }
  .skill-card:hover::after { transform: scaleX(1); }
  .skill-icon { width: 36px; height: 36px; border-radius: 9px; background: var(--tag-bg); display: flex; align-items: center; justify-content: center; margin-bottom: 0.8rem; font-size: 1.05rem; }
  .skill-name { font-weight: 600; margin-bottom: 0.6rem; font-size: 0.88rem; }
  .skill-tags { display: flex; flex-wrap: wrap; gap: 5px; }
  .tag { background: var(--tag-bg); color: var(--tag-color); padding: 2px 9px; border-radius: 100px; font-size: 0.71rem; font-weight: 500; font-family: 'JetBrains Mono', monospace; }
  .tag.gray { background: #f3f4f6; color: #374151; }

  /* ══ EXPERIENCE ══ */
  .exp-card {
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 14px; padding: 1.6rem 1.75rem 1.6rem 2.1rem;
    margin-bottom: 1.1rem; position: relative;
  }
  .exp-card::before {
    content: ''; position: absolute; left: 0; top: 1.5rem; bottom: 1.5rem;
    width: 3px; border-radius: 2px;
    background: linear-gradient(180deg, #2563eb, #7c3aed);
  }
  .exp-header { display: flex; align-items: flex-start; justify-content: space-between; margin-bottom: 0.8rem; gap: 1rem; }
  .exp-title { font-weight: 600; font-size: 1rem; }
  .exp-company { color: var(--accent); font-size: 0.86rem; margin-top: 2px; }
  .exp-date { background: #f3f4f6; padding: 3px 11px; border-radius: 100px; font-size: 0.74rem; color: var(--muted); white-space: nowrap; font-weight: 500; }
  .exp-bullets { list-style: none; }
  .exp-bullets li { padding: 4px 0 4px 1.4rem; position: relative; font-size: 0.875rem; color: #374151; line-height: 1.6; }
  .exp-bullets li::before { content: '→'; position: absolute; left: 0; color: var(--accent); font-size: 0.76rem; top: 6px; }

  /* ══ PROJECTS ══ */
  .projects-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 1.1rem; margin-top: 1.6rem; }
  .project-card {
    background: var(--card-bg); border: 1px solid var(--border);
    border-radius: 14px; padding: 1.5rem;
    display: flex; flex-direction: column;
    transition: transform 0.2s, box-shadow 0.2s;
  }
  .project-card:hover { transform: translateY(-5px); box-shadow: 0 14px 36px rgba(0,0,0,0.1); }
  .project-card.featured { border-color: rgba(37,99,235,0.25); background: linear-gradient(135deg, #fff 0%, #eff6ff 100%); }
  .project-badge { display: inline-block; background: var(--accent); color: #fff; font-size: 0.63rem; font-weight: 700; letter-spacing: 0.1em; text-transform: uppercase; padding: 3px 9px; border-radius: 100px; margin-bottom: 0.8rem; width: fit-content; }
  .project-name { font-family: 'DM Serif Display', serif; font-size: 1.15rem; letter-spacing: -0.01em; margin-bottom: 0.55rem; line-height: 1.25; }
  .project-desc { font-size: 0.84rem; color: #4b5563; line-height: 1.7; margin-bottom: 0.8rem; flex: 1; }
  .project-highlights { list-style: none; margin-bottom: 0.9rem; }
  .project-highlights li { font-size: 0.79rem; color: #374151; padding: 3px 0 3px 1.1rem; position: relative; }
  .project-highlights li::before { content: '▸'; position: absolute; left: 0; color: var(--accent); font-size: 0.67rem; top: 5px; }
  .project-stack { display: flex; flex-wrap: wrap; gap: 4px; }

  /* ══ CONTACT ══ */
  .contact-card {
    background: var(--black); color: var(--white);
    border-radius: 20px; padding: 3.25rem;
    text-align: center; position: relative; overflow: hidden;
  }
  .contact-card::before {
    content: ''; position: absolute; top: 0; left: 0; right: 0; height: 3px;
    background: linear-gradient(90deg, #2563eb, #7c3aed, #db2777);
  }
  .contact-card h2 { color: var(--white); margin-bottom: 0.8rem; }
  .contact-card p { color: rgba(255,255,255,0.58); margin-bottom: 1.875rem; max-width: 480px; margin-left: auto; margin-right: auto; font-size: 0.92rem; }
  .contact-links { display: flex; justify-content: center; gap: 0.8rem; flex-wrap: wrap; }
  .contact-link {
    display: flex; align-items: center; gap: 8px;
    background: rgba(255,255,255,0.08); color: #fff;
    padding: 10px 19px; border-radius: 9px;
    text-decoration: none; font-size: 0.84rem; font-weight: 500;
    border: 1px solid rgba(255,255,255,0.12);
    transition: background 0.2s, transform 0.15s;
  }
  .contact-link:hover { background: rgba(255,255,255,0.15); transform: translateY(-2px); }

  /* ══ FOOTER ══ */
  footer { text-align: center; padding: 1.4rem 5%; font-size: 0.77rem; color: var(--muted); border-top: 1px solid var(--border); }

  /* ══ ANIMATIONS ══ */
  .fade-in { opacity: 0; transform: translateY(18px); transition: opacity 0.52s ease, transform 0.52s ease; }
  .fade-in.visible { opacity: 1; transform: translateY(0); }

  /* ══ RESPONSIVE ══ */
  @media (max-width: 900px) {
    .hero { grid-template-columns: 1fr; min-height: auto; }
    .hero-left { padding: 95px 6% 48px; }
    .hero-right { min-height: 58vw; }
    .about-grid { grid-template-columns: 1fr; gap: 2rem; }
    .about-stat-row { flex-direction: row; flex-wrap: wrap; }
    .stat-card { flex: 1; min-width: 130px; }
  }
  @media (max-width: 768px) {
    section { padding: 44px 1.25rem; }
    .contact-card { padding: 2rem 1.5rem; }
    .exp-header { flex-direction: column; }
    nav { padding: 0 1rem; }
    .nav-links { display: none; }
    .hero-left { padding: 88px 1.25rem 40px; }
  }
</style>
</head>
<body>

<!-- NAVBAR -->
<nav>
  <a href="#" class="nav-logo">
    <div class="nav-logo-mark">AL</div>
    <span class="nav-name">Ajitha L.</span>
  </a>
  <ul class="nav-links">
    <li><a href="#about">About</a></li>
    <li><a href="#skills">Skills</a></li>
    <li><a href="#experience">Experience</a></li>
    <li><a href="#projects">Projects</a></li>
    <li><a href="#contact" class="nav-cta">Hire Me</a></li>
  </ul>
</nav>

<!-- HERO -->
<div class="hero">
  <div class="hero-left">
    <div class="hero-tag">Open to AI &amp; ML Roles</div>
    <h1>Ajitha<br><em>Lakshmanan</em></h1>
    <p class="hero-sub">AI Developer &amp; ML Engineer specializing in LLM integration, generative AI pipelines, and intelligent automation — turning cutting-edge research into production-ready systems.</p>
    <div class="hero-btns">
      <a href="#projects" class="btn-primary">View Projects</a>
      <a href="#contact" class="btn-outline">Get in Touch</a>
    </div>
    <div class="hero-contacts">
      <a href="tel:+919361336871" class="hero-contact-item">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.61 3.42 2 2 0 0 1 3.6 1.25h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.87a16 16 0 0 0 6.08 6.08l.97-.97a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        +91 93613 36871
      </a>
      <a href="mailto:ajithal0904@gmail.com" class="hero-contact-item">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        ajithal0904@gmail.com
      </a>
      <a href="https://www.linkedin.com/in/ajitha-lakshmanan" target="_blank" class="hero-contact-item">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        LinkedIn
      </a>
      <a href="https://github.com/Ajitha-2003" target="_blank" class="hero-contact-item">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z"/></svg>
        GitHub
      </a>
      <a href="https://ajitha-l.vercel.app" target="_blank" class="hero-contact-item">
        <svg width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
        Portfolio
      </a>
    </div>
  </div>

  <div class="hero-right">
    <canvas id="avatar-canvas"></canvas>
    <div class="hero-badge"><span class="dot" style="background:#2563eb"></span>LLM Integration</div>
    <div class="hero-badge"><span class="dot" style="background:#7c3aed"></span>Python &middot; Flask</div>
    <div class="hero-badge"><span class="dot" style="background:#059669"></span>RAG Pipelines</div>
    <div class="hero-badge"><span class="dot" style="background:#db2777"></span>AI Automation</div>
  </div>
</div>

<!-- ABOUT -->
<section id="about">
  <div class="about-grid fade-in">
    <div class="about-stat-row">
      <div class="stat-card"><div class="stat-num">1+</div><div class="stat-desc">Years building production AI systems at Cartrabbit</div></div>
      <div class="stat-card"><div class="stat-num">30+</div><div class="stat-desc">REST API test cases automated with AI-generated edge cases</div></div>
      <div class="stat-card"><div class="stat-num">40%</div><div class="stat-desc">Reduction in QA review time via LLM-powered validation</div></div>
      <div class="stat-card"><div class="stat-num">300+</div><div class="stat-desc">Students served by AI semantic search platform</div></div>
    </div>
    <div class="about-text">
      <div class="section-label">About Me</div>
      <h2>Building AI systems that actually work.</h2>
      <p>I'm an <strong>AI Developer and Machine Learning Engineer</strong> based in Coimbatore, India, passionate about transforming LLM research into scalable, production-grade intelligent systems. I specialize in <strong>LLM integration, RAG pipelines, vector search, generative AI, and NLP-powered automation</strong> using Python, Flask, LangChain, and OpenAI APIs.</p>
      <p>At <strong>Cartrabbit Technologies</strong>, I've applied prompt engineering and LLM-based validation pipelines to automate QA workflows — cutting review cycles by 40% and boosting site performance by 25%. I design multi-user full-stack AI apps, build agentic task pipelines, and champion MLOps best practices for production deployments.</p>
      <p>Completing my B.E. in Computer Science (2025) and actively seeking <strong>AI Developer, ML Engineer, or NLP Engineer</strong> roles where I can design, ship, and scale intelligent products with measurable impact.</p>
    </div>
  </div>
</section>

<!-- SKILLS -->
<section id="skills">
  <div class="fade-in">
    <div class="section-label">Technical Skills</div>
    <h2>Tools &amp; technologies I use</h2>
  </div>
  <div class="skills-grid fade-in">
    <div class="skill-card">
      <div class="skill-icon">🤖</div>
      <div class="skill-name">AI / ML &amp; NLP</div>
      <div class="skill-tags">
        <span class="tag">OpenAI API</span><span class="tag">LangChain</span><span class="tag">Hugging Face</span><span class="tag">FAISS</span><span class="tag">Prompt Eng.</span><span class="tag">RAG</span><span class="tag">ChromaDB</span>
      </div>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🐍</div>
      <div class="skill-name">Backend &amp; APIs</div>
      <div class="skill-tags">
        <span class="tag">Python</span><span class="tag">Flask</span><span class="tag">FastAPI</span><span class="tag">REST APIs</span><span class="tag">Streamlit</span><span class="tag gray">Cron Jobs</span>
      </div>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🗄️</div>
      <div class="skill-name">Databases &amp; Storage</div>
      <div class="skill-tags">
        <span class="tag">MongoDB</span><span class="tag">MySQL</span><span class="tag">Vector DBs</span><span class="tag gray">JSON / CSV</span>
      </div>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🧪</div>
      <div class="skill-name">Testing &amp; QA</div>
      <div class="skill-tags">
        <span class="tag">Selenium</span><span class="tag">Postman</span><span class="tag">Pytest</span><span class="tag">JMeter</span><span class="tag gray">Manual Testing</span><span class="tag gray">API Testing</span>
      </div>
    </div>
    <div class="skill-card">
      <div class="skill-icon">⚙️</div>
      <div class="skill-name">MLOps &amp; DevOps</div>
      <div class="skill-tags">
        <span class="tag gray">Git / GitHub</span><span class="tag gray">CI/CD</span><span class="tag gray">Docker</span><span class="tag gray">VS Code</span><span class="tag gray">Jupyter</span>
      </div>
    </div>
    <div class="skill-card">
      <div class="skill-icon">🌐</div>
      <div class="skill-name">Platforms &amp; CMS</div>
      <div class="skill-tags">
        <span class="tag gray">HTML / CSS</span><span class="tag gray">WordPress</span><span class="tag gray">WooCommerce</span><span class="tag gray">Shopify</span>
      </div>
    </div>
  </div>
</section>

<!-- EXPERIENCE -->
<section id="experience">
  <div class="fade-in">
    <div class="section-label">Work Experience</div>
    <h2>Where I've built things</h2>
  </div>
  <div class="fade-in">
    <div class="exp-card">
      <div class="exp-header">
        <div>
          <div class="exp-title">AI-Enabled QA &amp; Automation Engineer</div>
          <div class="exp-company">Cartrabbit Technologies &middot; Coimbatore, India</div>
        </div>
        <div class="exp-date">July 2024 – Present</div>
      </div>
      <ul class="exp-bullets">
        <li>Architected AI-assisted test automation frameworks using Python and OpenAI APIs — integrating LLM-driven edge-case generation to raise test coverage and cut manual QA effort significantly.</li>
        <li>Deployed LLM-based content validation pipelines to auto-review product descriptions and email templates in WooCommerce plugins, cutting QA review cycles by <strong>40%</strong>.</li>
        <li>Engineered prompt engineering workflows for automated bug-report summarization and intelligent triage, reducing P1 response time and improving sprint velocity.</li>
        <li>Automated <strong>30+ REST API test cases</strong> in Postman; applied generative AI to produce adversarial and boundary scenarios from OpenAPI schemas.</li>
        <li>Led regression testing and AI-driven performance analysis, boosting production site speed scores by <strong>25%</strong>.</li>
        <li>Collaborated cross-functionally on MLOps standards and AI feature rollouts into CI/CD pipelines across Dev, Product, and Design teams.</li>
        <li>Received <strong>&#127942; Rising Star – Testing Award</strong> at Cartrabbit Annual Meet 2024.</li>
      </ul>
    </div>
  </div>
</section>

<!-- PROJECTS -->
<section id="projects">
  <div class="fade-in">
    <div class="section-label">Projects</div>
    <h2>Things I've shipped</h2>
  </div>
  <div class="projects-grid fade-in">
    <div class="project-card featured">
      <div class="project-badge">Featured</div>
      <div class="project-name">TaskFlow — AI Task Reminder System</div>
      <p class="project-desc">A full-stack, multi-user task management and automated reminder platform with role-based auth, intelligent email scheduling, and real-time team collaboration — built with Python and Flask.</p>
      <ul class="project-highlights">
        <li>Role-based auth (Admin / Employee) via Flask-Login &amp; Werkzeug</li>
        <li>Automated dual-wave email reminders with 12h / 24h scheduling engine</li>
        <li>Tomorrow Checklist feature for AI-assisted daily sprint planning</li>
        <li>Real-time dashboard with category filters, task comments &amp; CSV export</li>
        <li>Invite-link onboarding &amp; modular org management layer (org_store.py)</li>
      </ul>
      <div class="project-stack">
        <span class="tag">Python</span><span class="tag">Flask</span><span class="tag">Pandas</span><span class="tag gray">Flask-Login</span><span class="tag gray">Streamlit</span><span class="tag gray">Pytest</span>
      </div>
    </div>
    <div class="project-card">
      <div class="project-name">AI Study Material Management System</div>
      <p class="project-desc">Intelligent RAG-based document distribution platform for students and faculty — enabling semantic search over academic content using FAISS vector embeddings and MongoDB.</p>
      <ul class="project-highlights">
        <li>Semantic search via FAISS vector embeddings &amp; NLP query parsing</li>
        <li>Reduced manual distribution workload by <strong>40%</strong></li>
        <li>Served <strong>300+ students</strong> with instant relevant material retrieval</li>
        <li>LLM-assisted document tagging and auto-categorization pipeline</li>
      </ul>
      <div class="project-stack">
        <span class="tag">Python</span><span class="tag">FAISS</span><span class="tag">RAG</span><span class="tag gray">MongoDB</span><span class="tag gray">HTML / CSS</span>
      </div>
    </div>
    <div class="project-card">
      <div class="project-name">WPLoyalty &amp; YUKO — AI-Augmented QA</div>
      <p class="project-desc">Applied AI-assisted testing on WooCommerce plugins and YUKO SaaS using prompt-driven test case generation to validate complex reward logic and multi-environment discount rules.</p>
      <ul class="project-highlights">
        <li>LLM prompt-driven test case generation for WooCommerce reward flows</li>
        <li>Validated discount rules, loyalty logic &amp; Spark Email Editor</li>
        <li>UI + REST API regression testing for YUKO SaaS reward automation</li>
        <li>Improved test case diversity by 35% via generative AI scenarios</li>
      </ul>
      <div class="project-stack">
        <span class="tag gray">WordPress</span><span class="tag gray">WooCommerce</span><span class="tag gray">Postman</span><span class="tag gray">Selenium</span><span class="tag">OpenAI API</span>
      </div>
    </div>
  </div>
</section>

<!-- CONTACT -->
<section id="contact">
  <div class="contact-card fade-in">
    <div class="section-label" style="color:rgba(255,255,255,0.45)">Get In Touch</div>
    <h2>Let's build something<br>intelligent together.</h2>
    <p>Actively seeking AI Developer, ML Engineer, and NLP Engineer roles. Whether you have an opportunity, a project idea, or just want to connect — I'd love to hear from you.</p>
    <div class="contact-links">
      <a href="tel:+919361336871" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.61 3.42 2 2 0 0 1 3.6 1.25h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.87a16 16 0 0 0 6.08 6.08l.97-.97a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        +91 93613 36871
      </a>
      <a href="mailto:ajithal0904@gmail.com" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="m22 7-8.97 5.7a1.94 1.94 0 0 1-2.06 0L2 7"/></svg>
        ajithal0904@gmail.com
      </a>
      <a href="https://www.linkedin.com/in/ajitha-lakshmanan" target="_blank" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg>
        LinkedIn
      </a>
      <a href="https://github.com/Ajitha-2003" target="_blank" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.37 0 0 5.37 0 12c0 5.31 3.435 9.795 8.205 11.385.6.105.825-.255.825-.57 0-.285-.015-1.23-.015-2.235-3.015.555-3.795-.735-4.035-1.41-.135-.345-.72-1.41-1.23-1.695-.42-.225-1.02-.78-.015-.795.945-.015 1.62.87 1.845 1.23 1.08 1.815 2.805 1.305 3.495.99.105-.78.42-1.305.765-1.605-2.67-.3-5.46-1.335-5.46-5.925 0-1.305.465-2.385 1.23-3.225-.12-.3-.54-1.53.12-3.18 0 0 1.005-.315 3.3 1.23.96-.27 1.98-.405 3-.405s2.04.135 3 .405c2.295-1.56 3.3-1.23 3.3-1.23.66 1.65.24 2.88.12 3.18.765.84 1.23 1.905 1.23 3.225 0 4.605-2.805 5.625-5.475 5.925.435.375.81 1.095.81 2.22 0 1.605-.015 2.895-.015 3.3 0 .315.225.69.825.57A12.02 12.02 0 0 0 24 12c0-6.63-5.37-12-12-12z"/></svg>
        GitHub
      </a>
      <a href="https://ajitha-l.vercel.app" target="_blank" class="contact-link">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
        Portfolio
      </a>
    </div>
  </div>
</section>

<footer>
  <p>Designed &amp; built by Ajitha L &middot; AI Developer &middot; Coimbatore, India &middot; 2025</p>
</footer>

<script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
<script>
(function() {
  const canvas = document.getElementById('avatar-canvas');
  const col = canvas.parentElement;
  const renderer = new THREE.WebGLRenderer({ canvas, antialias: true, alpha: true });
  renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
  renderer.shadowMap.enabled = true;

  const scene = new THREE.Scene();
  const camera = new THREE.PerspectiveCamera(42, 1, 0.1, 100);
  camera.position.set(0, 0.6, 5.2);

  function resize() {
    const w = col.offsetWidth, h = col.offsetHeight;
    renderer.setSize(w, h, false);
    camera.aspect = w / h;
    camera.updateProjectionMatrix();
  }

  scene.add(new THREE.AmbientLight(0xffffff, 0.75));
  const sun = new THREE.DirectionalLight(0xffffff, 1.0); sun.position.set(4, 6, 5); scene.add(sun);
  const fill = new THREE.DirectionalLight(0xdbeafe, 0.5); fill.position.set(-4, 2, -3); scene.add(fill);
  const rim = new THREE.PointLight(0x7c3aed, 0.7, 12); rim.position.set(2, 4, -2); scene.add(rim);
  const front = new THREE.PointLight(0x2563eb, 0.4, 10); front.position.set(0, 2, 4); scene.add(front);

  const skin   = new THREE.MeshToonMaterial({ color: 0xf0b990 });
  const hair   = new THREE.MeshToonMaterial({ color: 0x1a0800 });
  const shirt  = new THREE.MeshToonMaterial({ color: 0x2563eb });
  const dark   = new THREE.MeshToonMaterial({ color: 0x111827 });
  const white_ = new THREE.MeshToonMaterial({ color: 0xffffff });
  const screenM= new THREE.MeshToonMaterial({ color: 0x1d4ed8, emissive: 0x2563eb, emissiveIntensity: 0.5 });
  const cheek  = new THREE.MeshToonMaterial({ color: 0xf9a8c9, transparent: true, opacity: 0.55 });

  const g = new THREE.Group(); scene.add(g);

  const head = new THREE.Mesh(new THREE.SphereGeometry(0.6, 32, 32), skin);
  head.position.y = 1.6; g.add(head);

  const hairCap = new THREE.Mesh(new THREE.SphereGeometry(0.62, 32, 16, 0, Math.PI*2, 0, Math.PI*0.52), hair);
  hairCap.position.y = 1.6; g.add(hairCap);
  const hairBack = new THREE.Mesh(new THREE.SphereGeometry(0.61, 32, 16, Math.PI*0.15, Math.PI*1.7, Math.PI*0.38, Math.PI*0.6), hair);
  hairBack.position.y = 1.6; g.add(hairBack);
  const bun = new THREE.Mesh(new THREE.SphereGeometry(0.22, 16, 16), hair);
  bun.position.set(0, 2.27, -0.38); g.add(bun);
  const bunRing = new THREE.Mesh(new THREE.TorusGeometry(0.14, 0.05, 8, 18), hair);
  bunRing.position.set(0, 2.12, -0.35); bunRing.rotation.x = 0.3; g.add(bunRing);

  [-0.22, 0.22].forEach(x => {
    const eye = new THREE.Mesh(new THREE.SphereGeometry(0.08, 14, 14), dark); eye.position.set(x, 1.62, 0.55); g.add(eye);
    const shine = new THREE.Mesh(new THREE.SphereGeometry(0.022, 8, 8), new THREE.MeshBasicMaterial({color:0xffffff})); shine.position.set(x+0.03, 1.655, 0.635); g.add(shine);
    const lash = new THREE.Mesh(new THREE.SphereGeometry(0.082, 14, 7, 0, Math.PI*2, 0, Math.PI*0.42), dark); lash.position.set(x, 1.635, 0.55); g.add(lash);
    const brow = new THREE.Mesh(new THREE.BoxGeometry(0.14, 0.025, 0.025), hair); brow.position.set(x, 1.76, 0.55); brow.rotation.z = x<0?0.12:-0.12; g.add(brow);
  });
  [-0.4, 0.4].forEach(x => { const ck = new THREE.Mesh(new THREE.SphereGeometry(0.11, 12, 12), cheek); ck.position.set(x, 1.5, 0.5); g.add(ck); });
  const nose = new THREE.Mesh(new THREE.SphereGeometry(0.045, 10, 10), skin); nose.position.set(0, 1.54, 0.61); g.add(nose);
  const smile = new THREE.Mesh(new THREE.TorusGeometry(0.14, 0.022, 8, 16, Math.PI), dark); smile.position.set(0, 1.43, 0.56); smile.rotation.z = Math.PI; g.add(smile);

  const neck = new THREE.Mesh(new THREE.CylinderGeometry(0.17, 0.20, 0.28, 16), skin); neck.position.y = 1.0; g.add(neck);
  const torso = new THREE.Mesh(new THREE.CylinderGeometry(0.42, 0.36, 1.0, 22), shirt); torso.position.y = 0.36; g.add(torso);
  const coll = new THREE.Mesh(new THREE.CylinderGeometry(0.2, 0.18, 0.18, 16), white_); coll.position.y = 0.9; g.add(coll);

  [[-0.58, 0.65, 0.08, 0.38], [0.58, 0.65, 0.08, -0.38]].forEach(([x,y,z,rz]) => {
    const arm = new THREE.Mesh(new THREE.CylinderGeometry(0.11, 0.10, 0.55, 14), shirt); arm.position.set(x,y,z); arm.rotation.z=rz; g.add(arm);
  });
  [[-0.68, 0.28, 0.22, 0.5], [0.68, 0.28, 0.22, -0.5]].forEach(([x,y,z,rz]) => {
    const fa = new THREE.Mesh(new THREE.CylinderGeometry(0.09, 0.085, 0.45, 14), skin); fa.position.set(x,y,z); fa.rotation.z=rz; fa.rotation.x=-0.3; g.add(fa);
  });
  [[-0.28, -0.04, 0.55], [0.28, -0.04, 0.55]].forEach(([x,y,z]) => {
    const hand = new THREE.Mesh(new THREE.SphereGeometry(0.11, 12, 12), skin); hand.scale.set(1.1, 0.7, 1.2); hand.position.set(x,y,z); g.add(hand);
  });

  const lapB = new THREE.Mesh(new THREE.BoxGeometry(0.82, 0.055, 0.55), dark); lapB.position.set(0,-0.08,0.44); g.add(lapB);
  const pad = new THREE.Mesh(new THREE.BoxGeometry(0.22, 0.008, 0.14), new THREE.MeshToonMaterial({color:0x374151})); pad.position.set(0,-0.05,0.6); g.add(pad);
  for(let r=0;r<3;r++){ const kr=new THREE.Mesh(new THREE.BoxGeometry(0.68,0.008,0.06),new THREE.MeshToonMaterial({color:0x4b5563})); kr.position.set(0,-0.05,0.25+r*0.08); g.add(kr); }
  const lapS = new THREE.Mesh(new THREE.BoxGeometry(0.80, 0.52, 0.035), dark); lapS.position.set(0,0.33,0.18); lapS.rotation.x=-0.42; g.add(lapS);
  const scrG = new THREE.Mesh(new THREE.BoxGeometry(0.72, 0.44, 0.012), screenM); scrG.position.set(0,0.335,0.165); scrG.rotation.x=-0.42; g.add(scrG);
  [0.13, 0.06, -0.01, -0.08].forEach((y,i)=>{
    const ln=new THREE.Mesh(new THREE.BoxGeometry(i===0?0.42:0.55,0.018,0.005),new THREE.MeshToonMaterial({color:0x93c5fd})); ln.position.set(i===0?-0.1:0,0.335+y,0.173); ln.rotation.x=-0.42; g.add(ln);
  });

  // Particles
  const pGeo = new THREE.BufferGeometry();
  const pN = 80, pPos = new Float32Array(pN*3), pCol = new Float32Array(pN*3);
  const pal = [[0.15,0.38,0.92],[0.49,0.23,0.93],[0.86,0.15,0.47],[0.02,0.6,0.42]];
  for(let i=0;i<pN;i++){
    pPos[i*3]=(Math.random()-.5)*5; pPos[i*3+1]=(Math.random()-.5)*5+0.5; pPos[i*3+2]=(Math.random()-.5)*3-1;
    const c=pal[Math.floor(Math.random()*4)]; pCol[i*3]=c[0]; pCol[i*3+1]=c[1]; pCol[i*3+2]=c[2];
  }
  pGeo.setAttribute('position',new THREE.BufferAttribute(pPos,3));
  pGeo.setAttribute('color',new THREE.BufferAttribute(pCol,3));
  const particles = new THREE.Points(pGeo, new THREE.PointsMaterial({size:0.042,vertexColors:true,transparent:true,opacity:0.65}));
  scene.add(particles);

  const ring1 = new THREE.Mesh(new THREE.TorusGeometry(1.65,0.012,8,80), new THREE.MeshBasicMaterial({color:0x2563eb,transparent:true,opacity:0.22}));
  ring1.rotation.x = Math.PI/2.5; scene.add(ring1);
  const ring2 = new THREE.Mesh(new THREE.TorusGeometry(2.05,0.008,8,80), new THREE.MeshBasicMaterial({color:0x7c3aed,transparent:true,opacity:0.16}));
  ring2.rotation.x = Math.PI/3; ring2.rotation.z = 0.4; scene.add(ring2);

  const ground = new THREE.Mesh(new THREE.CircleGeometry(1.2,40), new THREE.MeshBasicMaterial({color:0x2563eb,transparent:true,opacity:0.06}));
  ground.rotation.x = -Math.PI/2; ground.position.y = -1.15; scene.add(ground);

  g.position.y = -0.4;
  resize();
  window.addEventListener('resize', resize);

  let mx=0, my=0;
  document.addEventListener('mousemove', e => { mx=(e.clientX/window.innerWidth-.5)*2; my=(e.clientY/window.innerHeight-.5)*2; });

  let t=0;
  function animate(){
    requestAnimationFrame(animate); t+=0.011;
    g.rotation.y = Math.sin(t*0.35)*0.22 + mx*0.07;
    camera.position.x = mx*0.1; camera.position.y = 0.6 - my*0.05;
    camera.lookAt(0,0.3,0);
    head.position.y = 1.6 + Math.sin(t)*0.022;
    bun.position.y  = 2.27 + Math.sin(t)*0.022;
    bunRing.position.y = 2.12 + Math.sin(t)*0.022;
    hairCap.position.y = 1.6 + Math.sin(t)*0.022;
    hairBack.position.y = 1.6 + Math.sin(t)*0.022;
    ring1.rotation.z += 0.004; ring2.rotation.z -= 0.003;
    particles.rotation.y += 0.0024; particles.rotation.x += 0.0007;
    renderer.render(scene, camera);
  }
  animate();
})();

// Navbar active link on scroll
const sections = document.querySelectorAll('section[id]');
const navLinks = document.querySelectorAll('.nav-links a');
new IntersectionObserver(entries => {
  entries.forEach(e => {
    if(e.isIntersecting){
      navLinks.forEach(a=>a.classList.remove('active'));
      const a = document.querySelector(`.nav-links a[href="#${e.target.id}"]`);
      if(a) a.classList.add('active');
    }
  });
},{threshold:0.4}).observe && sections.forEach(s => {
  new IntersectionObserver(entries=>{
    entries.forEach(e=>{ if(e.isIntersecting){ navLinks.forEach(a=>a.classList.remove('active')); const a=document.querySelector(`.nav-links a[href="#${e.target.id}"]`); if(a)a.classList.add('active'); }});
  },{threshold:0.4}).observe(s);
});

// Scroll fade-in
new IntersectionObserver(entries=>{
  entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('visible'); });
},{threshold:0.07}).observe && document.querySelectorAll('.fade-in').forEach(el=>{
  new IntersectionObserver(entries=>{ entries.forEach(e=>{ if(e.isIntersecting) e.target.classList.add('visible'); }); },{threshold:0.07}).observe(el);
});
</script>
</body>
</html>
