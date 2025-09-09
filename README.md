<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Sridivya's Portfolio</title>
  <meta name="description" content="A clean, simple personal portfolio of Sridivya." />
  <style>
    :root{
      --bg:#0f172a;
      --panel:#111827;
      --muted:#94a3b8;
      --text:#e5e7eb;
      --brand:#22d3ee;
      --accent:#38bdf8;
      --ring:#22d3ee55;
      --radius:16px;
    }
    *{box-sizing:border-box}
    html,body{margin:0; padding:0; background: radial-gradient(1200px 600px at 80% -10%, #0b1225 0%, var(--bg) 45%), var(--bg); color:var(--text); font: 16px/1.6 system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, Noto Sans, Helvetica, Arial}
    a{color:var(--brand); text-decoration:none}
    a:hover{text-decoration:underline}
    .container{width:min(1100px, 92%); margin-inline:auto}
    .nav{position:sticky; top:0; backdrop-filter:saturate(180%) blur(8px); background:#0f172acc; border-bottom:1px solid #33415566; z-index:10}
    .nav_inner{display:flex; align-items:center; justify-content:space-between; padding:12px 0}
    .logo{display:flex; gap:10px; align-items:center; font-weight:700}
    .logo_badge{width:28px; height:28px; border-radius:8px; background:linear-gradient(135deg,var(--brand),var(--accent)); box-shadow:0 6px 20px #22d3ee44}
    .nav a{color:var(--text); opacity:.9}
    .nav a:hover{opacity:1}
    .nav_links{display:flex; gap:18px}
    header.hero{padding:84px 0 48px}
    .hero_grid{display:grid; grid-template-columns: 1.2fr .8fr; gap:28px}
    @media (max-width: 900px){.hero_grid{grid-template-columns: 1fr}}
    h1{font-size: clamp(30px, 6vw, 56px); line-height:1.1; margin: 0 0 12px}
    .lead{color:var(--muted); font-size: clamp(16px, 2.2vw, 18px)}
    .cta{display:flex; gap:12px; margin-top:22px; flex-wrap:wrap}
    .btn{appearance:none; border:1px solid #334155; padding:10px 14px; border-radius:12px; background:linear-gradient(180deg,#0b1325,#0f172a); color:var(--text); cursor:pointer}
    .btn.primary{background:linear-gradient(135deg,var(--brand),var(--accent)); color:#001827; font-weight:700; border:0}
    .btn:focus{outline:2px solid var(--ring); outline-offset:2px}
    .panel{background: linear-gradient(180deg,#0b1220,#0c152a); border:1px solid #33415566; border-radius: var(--radius); padding:18px}
    .panel h3{margin:0 0 8px}
    section{padding:32px 0}
    section h2{font-size: clamp(22px, 3.6vw, 32px); margin:0 0 16px}
    .grid{display:grid; gap:16px}
    .grid.cols-3{grid-template-columns: repeat(3, 1fr)}
    .grid.cols-2{grid-template-columns: repeat(2, 1fr)}
    @media (max-width: 900px){.grid.cols-3,.grid.cols-2{grid-template-columns: 1fr}}
    .card{background: linear-gradient(180deg,#0b1220,#0b1424); border:1px solid #33415555; border-radius: var(--radius); overflow:hidden; transition: transform .15s ease, border-color .15s ease; display:flex; flex-direction:column}
    .card:hover{transform: translateY(-2px); border-color:#475569aa}
    .card .body{padding:14px 14px 16px}
    .tag{font-size:12px; color:var(--muted); border:1px solid #33415599; border-radius:999px; padding:2px 8px; display:inline-block}
    .skills{display:flex; gap:10px; flex-wrap:wrap}
    .chip{padding:6px 10px; border:1px solid #33415588; border-radius:999px; font-size:13px; color:#e2e8f0}
    .footer{padding:40px 0 60px; color:var(--muted); font-size:14px}
    .socials{display:flex; gap:14px}
    .socials a{display:inline-flex; align-items:center; gap:8px; padding:8px 10px; border:1px solid #33415566; border-radius:12px}
    .sr-only{position:absolute; width:1px; height:1px; padding:0; margin:-1px; overflow:hidden; clip:rect(0,0,0,0); border:0}
  </style>
</head>
<body>
  <nav class="nav" aria-label="Primary">
    <div class="container nav_inner">
      <div class="logo" aria-label="Home">
        <span class="logo_badge" aria-hidden="true"></span>
        <span>SRIDIVYA</span>
      </div>
      <div class="nav_links">
        <a href="#about">About</a>
        <a href="#projects">Projects</a>
        <a href="#skills">Skills</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </nav>

  <header class="hero">
    <div class="container hero_grid">
      <div>
        <h1>Hello, I'm <span style="color:var(--brand)">Sridivya</span>.</h1>
        <p class="lead">I design and build clean, accessible web experiences. Here's a quick look at my work and skills.</p>
        <div class="cta">
          <a class="btn primary" href="#projects">View Projects</a>
          <a class="btn" href="#contact">Get in Touch</a>
        </div>
      </div>
      <div class="panel" aria-label="Quick facts">
        <h3>Quick Facts</h3>
        <ul>
          <li>📍 Based in City, Country</li>
          <li>💼 Currently: Role @ Company</li>
          <li>🎯 Looking for: Frontend roles</li>
          <li>✉️ Email: sridivyakosalaraman@gmail.com</li>
          <li>📞 Contact: 9342537346</li>
        </ul>
      </div>
    </div>
  </header>

  <main class="container">
    <section id="about" aria-labelledby="about-heading">
      <h2 id="about-heading">About</h2>
      <div class="card">
        <div class="body">
          <p>I'm a developer with a passion for crafting delightful user interfaces and performant web apps. I care about clean design, accessibility, and maintainable code.</p>
          <p>Outside of work, I enjoy reading, learning new tools, and contributing to open-source projects.</p>
        </div>
      </div>
    </section>

    <section id="projects" aria-labelledby="projects-heading">
      <h2 id="projects-heading">Projects</h2>
      <div class="grid cols-3">
        <article class="card">
          <div class="body">
            <h3>Analytics Dashboard</h3>
            <p class="tag">React • Charts</p>
            <p>A responsive analytics dashboard with real-time data and keyboard navigation.</p>
          </div>
        </article>
        <article class="card">
          <div class="body">
            <h3>Task Manager</h3>
            <p class="tag">Vue • PWA</p>
            <p>A minimalist task app with offline support and fast search.</p>
          </div>
        </article>
        <article class="card">
          <div class="body">
            <h3>UI Components</h3>
            <p class="tag">Design System</p>
            <p>A set of accessible, reusable components with docs and examples.</p>
          </div>
        </article>
      </div>
    </section>

    <section id="skills" aria-labelledby="skills-heading">
      <h2 id="skills-heading">Skills</h2>
      <div class="card">
        <div class="body">
          <div class="skills">
            <span class="chip">HTML</span>
            <span class="chip">CSS</span>
            <span class="chip">JavaScript</span>
            <span class="chip">React</span>
            <span class="chip">Node.js</span>
            <span class="chip">Accessibility</span>
            <span class="chip">Testing</span>
            <span class="chip">Figma</span>
          </div>
        </div>
      </div>
    </section>

    <section id="contact" aria-labelledby="contact-heading">
      <h2 id="contact-heading">Contact</h2>
      <div class="grid cols-2">
        <form class="card" onsubmit="event.preventDefault(); alert('Thanks! I\'ll reply soon.');" aria-describedby="contact-help">
          <div class="body">
            <label for="name">Name</label><br />
            <input id="name" name="name" required placeholder="Your name" style="width:100%; padding:10px; border-radius:10px; border:1px solid #334155; background:#0b1424; color:var(--text); margin:6px 0 12px" />
            <label for="email">Email</label><br />
            <input id="email" name="email" type="email" required placeholder="sridivyakosalaraman@gmail.com" style="width:100%; padding:10px; border-radius:10px; border:1px solid #334155; background:#0b1424; color:var(--text); margin:6px 0 12px" />
            <label for="msg">Message</label><br />
            <textarea id="msg" name="message" rows="4" required placeholder="Say hello..." style="width:100%; padding:10px; border-radius:10px; border:1px solid #334155; background:#0b1424; color:var(--text); margin:6px 0 12px"></textarea>
            <p id="contact-help" class="sr-only">All fields are required.</p>
            <button class="btn primary" type="submit">Send Message</button>
          </div>
        </form>
        <div class="card">
          <div class="body">
            <p>Prefer email? Reach me at <a href="mailto:sridivyakosalaraman@gmail.com">sridivyakosalaraman@gmail.com</a>.</p>
            <p>📞 Or call me: <strong>9342537346</strong></p>
            <div class="socials" aria-label="Social links">
              <a href="#">🐙 GitHub</a>
              <a href="#">💼 LinkedIn</a>
              <a href="#">🐦 Twitter</a>
              <a href="#">🏀 Dribbble</a>
            </div>
          </div>
        </div>
      </div>
    </section>
  </main>

  <footer class="footer">
    <div class="container">
      <div style="display:flex; justify-content:space-between; gap:16px; flex-wrap:wrap">
        <span>© <span id="year"></span> Sridivya</span>
        <a href="#top">Back to top ↑</a>
      </div>
    </div>
  </footer>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();
    document.querySelectorAll('a[href^="#"]').forEach(a => {
      a.addEventListener('click', e => {
        const id = a.getAttribute('href').slice(1);
        const el = document.getElementById(id);
        if(el){ e.preventDefault(); el.scrollIntoView({behavior:'smooth', block:'start'}); }
      });
    });
  </script>
</body>
</html>
