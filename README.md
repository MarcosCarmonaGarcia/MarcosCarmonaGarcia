<!--
  Perfil GitHub llamativo para Marcos Carmona García.
-->
<!doctype html>
<html lang="es">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Perfil — Marcos Carmona García</title>
  <style>
    :root{
      --bg1:#0f172a;
      --bg2:#071041;
      --accent1:#7c3aed;
      --accent2:#06b6d4;
      --glass: rgba(255,255,255,0.06);
      --glass-2: rgba(255,255,255,0.03);
      --text: #e6eef8;
      --muted: #9fb0d3;
      --card-radius:14px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(135deg,var(--bg1),var(--bg2));color:var(--text);padding:36px}
    .container{max-width:980px;margin:0 auto}

    .hero-bg{position:fixed;inset:0;z-index:0;filter:blur(60px);opacity:0.55;pointer-events:none}
    .blob{position:absolute;width:40vmax;height:40vmax;border-radius:50%;background:radial-gradient(circle at 30% 30%, var(--accent1), transparent 40%), radial-gradient(circle at 70% 70%, var(--accent2), transparent 40%);mix-blend-mode:screen;animation:float 12s ease-in-out infinite}
    .blob.b1{left:-10%;top:-20%;transform:rotate(10deg)}
    .blob.b2{right:-10%;bottom:-20%;transform:rotate(-10deg);animation-duration:16s;opacity:0.9}
    @keyframes float{0%{transform:translateY(0) scale(1)}50%{transform:translateY(-8%) scale(1.06)}100%{transform:translateY(0) scale(1)}}

    header.card{position:relative;background:linear-gradient(180deg,var(--glass),var(--glass-2));box-shadow:0 8px 30px rgba(2,6,23,0.6);border-radius:var(--card-radius);padding:26px;display:flex;gap:20px;align-items:center;z-index:1}
    .avatar{width:120px;height:120px;border-radius:22px;flex:0 0 120px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:grid;place-items:center;font-weight:700;font-size:28px;color:white}
    .title{flex:1}
    h1{margin:0;font-size:22px}
    p.lead{margin:6px 0 0;color:var(--muted)}

    .badges{margin-top:12px;display:flex;gap:8px;flex-wrap:wrap}
    .badge{background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;font-size:13px;border:1px solid rgba(255,255,255,0.03)}

    main.grid{display:grid;grid-template-columns:1fr 360px;gap:18px;margin-top:18px;z-index:1}
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:12px;border:1px solid rgba(255,255,255,0.02);box-shadow:0 6px 18px rgba(2,6,23,0.45)}

    .about small{color:var(--muted)}
    .skills{display:flex;flex-direction:column;gap:10px}
    .skill{display:flex;flex-direction:column}
    .skill .meta{display:flex;justify-content:space-between;font-size:13px;color:var(--muted)}
    .bar{height:10px;background:rgba(255,255,255,0.04);border-radius:999px;margin-top:6px;overflow:hidden}
    .bar > i{display:block;height:100%;border-radius:999px;background:linear-gradient(90deg,var(--accent1),var(--accent2));width:60%}

    .projects{display:grid;grid-template-columns:1fr 1fr;gap:12px}
    .project{padding:12px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02));border:1px solid rgba(255,255,255,0.02)}
    .project h4{margin:0 0 8px}
    .project p{margin:0;font-size:13px;color:var(--muted)}

    .right .widget{margin-bottom:12px}
    .links{display:flex;gap:10px;flex-wrap:wrap}
    a.link{display:inline-flex;align-items:center;gap:8px;padding:8px 12px;border-radius:10px;background:rgba(255,255,255,0.02);text-decoration:none;color:var(--text);font-weight:600;border:1px solid rgba(255,255,255,0.02)}

    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}

    @media (max-width:920px){main.grid{grid-template-columns:1fr} .projects{grid-template-columns:1fr} .avatar{width:96px;height:96px}}
  </style>
</head>
<body>
  <div class="hero-bg" aria-hidden>
    <div class="blob b1"></div>
    <div class="blob b2"></div>
  </div>

  <div class="container">
    <header class="card" role="banner">
      <div class="avatar">MC</div>
      <div class="title">
        <h1>Marcos Carmona García — Programador aficionado & aprendiz de pentesting</h1>
        <p class="lead">Interesado en el mundo del hacking ético. Aprendo, automatizo y construyo herramientas con Python y Bash.</p>

        <div class="badges" aria-hidden>
          <span class="badge">🏷️ Hacking ético</span>
          <span class="badge">🐍 Python</span>
          <span class="badge">🐚 Bash</span>
          <span class="badge">⚙️ Automations</span>
          <span class="badge">📡 Recon / OSINT</span>
        </div>
      </div>
    </header>

    <main class="grid">
      <section class="card about">
        <h3>Sobre mí</h3>
        <p><small>Soy un programador aficionado en proceso de aprendizaje, interesado en el mundo del pentesting (hacking ético). Mi objetivo: dominar scripting, explotación y automatización para auditorías de seguridad.</small></p>

        <hr style="margin:14px 0;border:none;border-top:1px solid rgba(255,255,255,0.03)">

        <h4>Habilidades</h4>
        <div class="skills">
          <div class="skill">
            <div class="meta"><span>Python</span><span>75%</span></div>
            <div class="bar"><i style="width:75%"></i></div>
          </div>
          <div class="skill">
            <div class="meta"><span>Bash & Shell</span><span>65%</span></div>
            <div class="bar"><i style="width:65%"></i></div>
          </div>
          <div class="skill">
            <div class="meta"><span>Networking / Recon</span><span>55%</span></div>
            <div class="bar"><i style="width:55%"></i></div>
          </div>
          <div class="skill">
            <div class="meta"><span>Web Exploitation</span><span>45%</span></div>
            <div class="bar"><i style="width:45%"></i></div>
          </div>
        </div>

        <hr style="margin:14px 0;border:none;border-top:1px solid rgba(255,255,255,0.03)">

        <h4>Proyectos destacados</h4>
        <div class="projects">
          <div class="project">
            <h4>Recon scripts</h4>
            <p>Conjunto de scripts en Bash/Python para inventariado y recolección de información (subdominios, puertos, banners).</p>
          </div>
          <div class="project">
            <h4>Toolkit de pentest</h4>
            <p>Automatización de pruebas básicas: scanning, explotación y reportado en formato markdown.</p>
          </div>
        </div>
      </section>

      <aside class="right">
        <div class="card widget">
          <h4>Contacto</h4>
          <div class="links" style="margin-top:10px">
            <a class="link" href="mailto:marcos@example.com">✉️ Email</a>
            <a class="link" href="https://github.com/mcgarcia">🐙 GitHub</a>
            <a class="link" href="https://linkedin.com/in/mcgarcia">💼 LinkedIn</a>
          </div>
        </div>

        <div class="card widget">
          <h4>Estadísticas</h4>
          <div style="display:flex;flex-direction:column;gap:8px;margin-top:10px">
            <img alt="GitHub Stats" src="https://github-readme-stats.vercel.app/api?username=mcgarcia&show_icons=true&theme=dark" style="border-radius:10px;max-width:100%">
            <img alt="Top Languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=mcgarcia&layout=compact&theme=dark" style="border-radius:10px;max-width:100%">
          </div>
        </div>

        <div class="card widget">
          <h4>Último tweet / notas</h4>
          <p style="color:var(--muted);font-size:13px;margin-top:8px">Aprendiendo pentesting — today: scripting & CTFs</p>
        </div>
      </aside>
    </main>

    <footer>
      ✨ Perfil generado para Marcos Carmona García • Personalízalo con tus proyectos y enlaces.
    </footer>
  </div>
</body>
</html>


