<!--
  Sushmita Portfolio - single-file website (dark theme)
  Instructions:
   - Save this file as index.html
   - Optional: create an "assets" folder for images and update paths
   - To publish on GitHub Pages: create a repository and push this file as the root (index.html)
-->

<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Sushmita M Angadi — Portfolio</title>
  <meta name="description" content="Sushmita M Angadi — ECE student, aspiring software engineer. Projects in Python, Verilog, MATLAB.">
  <style>
    :root{
      --bg:#0b0f12; --card:#0f1720; --muted:#9aa4ad; --accent:#7dd3fc; --glass: rgba(255,255,255,0.04);
      --radius:14px; --maxw:1000px; --mono: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,var(--bg),#061018);font-family:var(--mono);color:#e6eef6;line-height:1.5}
    .container{max-width:var(--maxw);margin:30px auto;padding:24px}
    header{display:flex;align-items:center;justify-content:space-between}
    .brand{display:flex;gap:14px;align-items:center}
    .avatar{width:68px;height:68px;border-radius:12px;background:linear-gradient(135deg,#e6eef6, #9be7ff);display:flex;align-items:center;justify-content:center;color:#062129;font-weight:700}
    h1{margin:0;font-size:22px}
    p.tag{margin:4px 0 0;color:var(--muted)}
    nav a{color:var(--muted);text-decoration:none;margin-left:18px}

    .hero{display:grid;grid-template-columns:1fr 360px;gap:24px;margin-top:26px}
    .card{background:linear-gradient(180deg,var(--card), #07101a);padding:20px;border-radius:var(--radius);box-shadow:0 6px 18px rgba(0,0,0,0.6)}
    .intro h2{margin:0 0 8px;font-size:20px}
    .intro p{color:var(--muted)}
    .cta{margin-top:18px}
    .btn{background:var(--accent);color:#042028;padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:600}

    .skills{display:flex;flex-wrap:wrap;gap:8px;margin-top:10px}
    .skill{background:var(--glass);padding:8px 12px;border-radius:10px;color:var(--muted);font-weight:600}

    .projects{margin-top:20px;display:grid;gap:12px}
    .project{padding:14px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent)}
    .project h3{margin:0 0 6px}
    .meta{color:var(--muted);font-size:13px}

    footer{margin-top:28px;text-align:center;color:var(--muted);font-size:14px}

    /* responsive */
    @media(max-width:900px){.hero{grid-template-columns:1fr}} 

    /* contact */
    .contact-row{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
    .chip{background:rgba(255,255,255,0.03);padding:10px 12px;border-radius:10px}

    /* resume button */
    .resume{display:inline-block;padding:10px 14px;border-radius:10px;border:1px solid rgba(125,211,252,0.12);color:var(--accent);text-decoration:none;font-weight:600}

    /* small > look */
    small{color:var(--muted)}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">
        <div class="avatar">SA</div>
        <div>
          <h1>Sushmita M Angadi</h1>
          <p class="tag">ECE Student • Aspiring Software Engineer</p>
        </div>
      </div>
      <nav>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <section class="hero">
      <div class="card intro">
        <h2>Hello — I build projects & learn every day</h2>
        <p>I'm an ECE student with a strong interest in software development. I work with Python, C, Verilog and MATLAB. Currently building projects to improve problem solving and full-stack skills.</p>
        <div class="cta">
          <a class="btn" href="#projects">See Projects</a>
          <a class="resume" href="resume.pdf" download style="margin-left:12px">Download Resume</a>
        </div>

        <div id="skills" style="margin-top:18px">
          <small>Skills</small>
          <div class="skills">
            <div class="skill">Python</div>
            <div class="skill">C</div>
            <div class="skill">Verilog</div>
            <div class="skill">MATLAB</div>
            <div class="skill">Problem Solving</div>
            <div class="skill">Git & GitHub</div>
          </div>
        </div>
      </div>

      <div class="card" style="display:flex;flex-direction:column;gap:12px;align-items:flex-start">
        <h3 style="margin:0">Contact</h3>
        <div class="meta">Email</div>
        <div class="chip"> <a href="mailto:sushmitaangadi8055@gmail.com" style="color:inherit;text-decoration:none">sushmitaangadi8055@gmail.com</a></div>

        <div style="margin-top:10px;width:100%">
          <h4 style="margin:0">Quick Links</h4>
          <div style="margin-top:8px;display:flex;gap:8px;flex-wrap:wrap">
            <a class="btn" href="#projects">Projects</a>
            <a class="resume" href="https://github.com/sushmitaangadi8055" target="_blank" rel="noopener">GitHub</a>
          </div>
        </div>

        <div style="margin-top:auto;width:100%;text-align:center;color:var(--muted);font-size:13px">
          <small>Profile Status: Preparing for Placement</small>
        </div>
      </div>
    </section>

    <section id="about" style="margin-top:22px">
      <div class="card">
        <h2>About</h2>
        <p class="meta">I am an Electronics & Communication student passionate about coding and building practical projects. I enjoy solving problems using Python and exploring hardware description with Verilog. I am improving my web development skills to present my work professionally.</p>
      </div>
    </section>

    <section id="projects" style="margin-top:18px">
      <div class="card">
        <h2>Projects</h2>
        <div class="projects">
          <article class="project">
            <h3>Alcohol Detection with Entry Gate Access</h3>
            <div class="meta">Role: Team Lead • Tools: Verilog, Embedded C, Sensors</div>
            <p>Designed a system to detect alcohol level and control gate access for safety. Implemented sensor interfacing and decision logic using Verilog and microcontroller firmware. <a href="#" style="color:var(--accent);text-decoration:none">View code</a></p>
          </article>

          <article class="project">
            <h3>Portfolio Website (This site)</h3>
            <div class="meta">Role: Developer • Tools: HTML, CSS, GitHub Pages</div>
            <p>Built a responsive dark theme portfolio website to showcase projects, skills and contact information. Hosted using GitHub Pages. <a href="#" style="color:var(--accent);text-decoration:none">View live</a></p>
          </article>

          <article class="project">
            <h3>MATLAB Signal Processing Experiments</h3>
            <div class="meta">Role: Research • Tools: MATLAB</div>
            <p>Worked on filtering and analysis of signals using MATLAB. Prepared reports and visualizations for coursework and mini-projects. <a href="#" style="color:var(--accent);text-decoration:none">View report</a></p>
          </article>
        </div>
      </div>
    </section>

    <section id="contact" style="margin-top:18px">
      <div class="card">
        <h2>Contact Me</h2>
        <p class="meta">Email me for collaborations, internships or placement opportunities.</p>
        <div style="margin-top:12px">
          <a class="btn" href="mailto:sushmitaangadi8055@gmail.com">Email: sushmitaangadi8055@gmail.com</a>
        </div>
      </div>
    </section>

    <footer>
      <p>Made with ❤ • Sushmita M Angadi • <small>Dark theme</small></p>
    </footer>
  </div>
</body>
</html>
