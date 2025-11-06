<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Your Name — Developer & Engineer</title>
  <meta name="description" content="Professional profile and resume for [Your Name] — Developer, Engineer. Contact, resume, and skillset." />

  <!-- Simple modern styling -->
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#9aa4b2;
      --accent1:#5eead4; /* teal */
      --accent2:#60a5fa; /* blue */
      --glass: rgba(255,255,255,0.04);
      --glass-2: rgba(255,255,255,0.03);
      --radius:14px;
      --max-width:980px;
      font-family: Inter, ui-sans-serif, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      color-scheme: dark;
    }
    html,body{height:100%}
    body{
      margin:0;
      background: linear-gradient(180deg, #071028 0%, #071222 60%);
      color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      display:flex;
      justify-content:center;
      padding:40px 18px;
      box-sizing:border-box;
    }

    .wrapper{
      width:100%;
      max-width:var(--max-width);
      display:grid;
      grid-template-columns: 1fr 360px;
      gap:28px;
      align-items:start;
    }

    /* Responsive: stack */
    @media (max-width:920px){
      .wrapper{grid-template-columns:1fr; padding-bottom:40px}
    }

    .card{
      background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border-radius:var(--radius);
      padding:26px;
      box-shadow: 0 6px 30px rgba(2,6,23,0.6);
      border: 1px solid rgba(255,255,255,0.03);
    }

    /* Left column */
    .hero{
      display:flex;
      gap:20px;
      align-items:center;
    }
    .avatar{
      width:96px;
      height:96px;
      border-radius:18px;
      background:linear-gradient(135deg,var(--accent1),var(--accent2));
      display:flex;
      align-items:center;
      justify-content:center;
      font-weight:700;
      font-size:30px;
      color:#04202a;
      box-shadow: 0 8px 30px rgba(8,13,20,0.55), inset 0 -6px 12px rgba(255,255,255,0.03);
      flex:0 0 96px;
    }
    .hero h1{
      margin:0 0 4px 0;
      font-size:22px;
      letter-spacing:-0.2px;
    }
    .subtitle{color:var(--muted); margin:0; font-size:13px}
    .tagline{margin-top:10px; color:var(--muted); font-size:14px; line-height:1.5}

    /* Resume timeline / summary */
    .section-title{
      display:flex;
      align-items:center;
      gap:12px;
      margin:10px 0 16px;
    }
    .section-title h2{font-size:16px; margin:0}
    .badge{
      font-size:12px;
      padding:6px 8px;
      border-radius:999px;
      background:linear-gradient(90deg,var(--accent1),var(--accent2));
      color:#022028;
      font-weight:600;
    }

    .summary{
      margin-top:6px;
      font-size:14px;
      color:var(--muted);
    }

    .resume-item{
      margin:10px 0 18px;
      padding:12px;
      border-radius:10px;
      background: linear-gradient(180deg, rgba(255,255,255,0.01), transparent);
      border: 1px solid rgba(255,255,255,0.025);
    }
    .resume-item h3{margin:0; font-size:15px}
    .muted-line{color:var(--muted); font-size:13px; margin-top:4px}

    /* Right column: contact & skills */
    .sidebar{
      display:flex;
      flex-direction:column;
      gap:18px;
      position:relative;
    }
    .contact-list{display:flex;flex-direction:column;gap:10px}
    .contact-row{
      display:flex;
      gap:12px;
      align-items:center;
      padding:10px;
      border-radius:10px;
      background:var(--glass);
      border:1px solid rgba(255,255,255,0.02);
    }
    .contact-row a{color:inherit; text-decoration:none}
    .icon{
      width:36px;height:36px;border-radius:8px;background:rgba(255,255,255,0.03);display:flex;align-items:center;justify-content:center;font-weight:600;
      color:var(--accent2); flex:0 0 36px;
    }

    .skills-grid{
      display:grid;
      grid-template-columns:repeat(2,1fr);
      gap:10px;
    }
    .skill{
      padding:10px;
      border-radius:10px;
      background:var(--glass-2);
      border: 1px solid rgba(255,255,255,0.02);
      font-size:13px;
      display:flex;
      gap:10px;
      align-items:center;
    }
    .skill .dot{
      width:10px;height:10px;border-radius:50%;
      background:linear-gradient(90deg,var(--accent1),var(--accent2));
      box-shadow: 0 4px 14px rgba(96,165,250,0.12);
      flex:0 0 10px;
    }

    .actions{
      display:flex;
      gap:10px;
      margin-top:8px;
    }
    .btn{
      display:inline-flex;
      align-items:center;
      gap:8px;
      padding:10px 12px;
      border-radius:10px;
      font-weight:600;
      text-decoration:none;
      color:#01202a;
      background:linear-gradient(90deg,var(--accent1),var(--accent2));
      border:none;
      cursor:pointer;
    }
    .btn.ghost{
      background:transparent;
      color:var(--accent2);
      border:1px solid rgba(96,165,250,0.12);
      box-shadow:none;
    }

    footer{
      margin-top:18px;
      color:var(--muted);
      font-size:13px;
    }

    /* small utility */
    .row{display:flex;gap:12px;align-items:center}
    .pill{background:rgba(255,255,255,0.02);padding:6px 8px;border-radius:999px;font-size:13px;color:var(--muted)}
  </style>
</head>
<body>
  <div class="wrapper" role="main" aria-label="Profile">
    <!-- Left column -->
    <div class="card" aria-labelledby="nameHeading">
      <div class="hero" id="nameHeading">
        <div class="avatar" aria-hidden="true">YN</div>
        <div style="flex:1">
          <h1>YOUR NAME <span style="font-weight:500; color:var(--muted); font-size:14px">— Senior Software Engineer</span></h1>
          <p class="subtitle">Building fast, reliable web & desktop applications. Strong focus on TypeScript, Node.js, and developer tooling.</p>
          <p class="tagline">I design and implement pragmatic, well-tested systems—shipping production-grade software, mentoring engineers, and improving developer experience.</p>
        </div>
      </div>

      <!-- Quick summary / resume snapshot -->
      <div style="margin-top:20px">
        <div class="section-title">
          <h2>Resume</h2>
          <span class="badge">Open to opportunities</span>
        </div>

        <p class="summary">
          Experienced full-stack engineer with 8+ years delivering complex projects across desktop, backend services, and cloud deployments. Skilled at designing APIs, building developer tools, and running resilient production systems.
        </p>

        <!-- Sample resume items -->
        <div class="resume-item" aria-labelledby="role1">
          <h3 id="role1">Staff Engineer — Acme Software</h3>
          <div class="muted-line">2022 — Present · Remote</div>
          <p style="margin-top:8px; color:var(--muted); font-size:14px">
            Led efforts to modernize the release pipeline, improved CI throughput by 4x, and architected a TypeScript microservices pattern used across multiple teams.
          </p>
        </div>

        <div class="resume-item" aria-labelledby="role2">
          <h3 id="role2">Senior Developer — Widget Labs</h3>
          <div class="muted-line">2018 — 2022 · Denver, CO</div>
          <p style="margin-top:8px; color:var(--muted); font-size:14px">
            Built and maintained cross-platform Electron apps, backend services in Node.js, and integrated observability tooling and E2E testing infrastructure.
          </p>
        </div>

        <div class="resume-item" aria-labelledby="edu">
          <h3 id="edu">Education & Credentials</h3>
          <div class="muted-line">B.S. Computer Science — University Name · 2016</div>
        </div>

        <div style="margin-top:6px" class="row">
          <a class="btn" href="resume.pdf" download aria-label="Download resume (replace resume.pdf)">
            <!-- simple download icon -->
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" aria-hidden="true"><path d="M12 3v10" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/><path d="M8 11l4 4 4-4" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/><path d="M21 21H3" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/></svg>
            Download Resume
          </a>
          <a class="btn ghost" href="#contact">Contact</a>
        </div>
      </div>

      <!-- Optional: short list of highlights -->
      <div style="margin-top:18px">
        <div class="section-title"><h2>Selected highlights</h2></div>
        <ul style="margin:0; padding-left:18px; color:var(--muted);">
          <li>Designed and shipped desktop tools used by 10k+ customers.</li>
          <li>Reduced CI cost by automating caching and parallelization.</li>
          <li>Mentored engineers on architecture and testing best practices.</li>
        </ul>
      </div>

      <footer>
        <div style="display:flex; justify-content:space-between; align-items:center; gap:12px; flex-wrap:wrap;">
          <div class="muted-line">Available for consulting & full-time roles</div>
          <div class="pill">Location: Denver, CO (remote-friendly)</div>
        </div>
      </footer>
    </div>

    <!-- Right column (sidebar) -->
    <aside class="sidebar">
      <div class="card contact" id="contact" aria-labelledby="contactHeading">
        <div class="section-title"><h2 id="contactHeading">Contact</h2></div>

        <div class="contact-list">
          <div class="contact-row">
            <div class="icon" aria-hidden="true">📧</div>
            <div>
              <div style="font-weight:700">Email</div>
              <div style="color:var(--muted); font-size:13px">
                <a href="mailto:you@example.com">you@example.com</a>
              </div>
            </div>
          </div>

          <div class="contact-row">
            <div class="icon" aria-hidden="true">🔗</div>
            <div>
              <div style="font-weight:700">LinkedIn</div>
              <div style="color:var(--muted); font-size:13px">
                <a href="https://www.linkedin.com/in/yourprofile" target="_blank" rel="noopener">linkedin.com/in/yourprofile</a>
              </div>
            </div>
          </div>

          <div class="contact-row">
            <div class="icon" aria-hidden="true">🐙</div>
            <div>
              <div style="font-weight:700">GitHub</div>
              <div style="color:var(--muted); font-size:13px">
                <a href="https://github.com/yourusername" target="_blank" rel="noopener">github.com/yourusername</a>
              </div>
            </div>
          </div>

          <div class="contact-row">
            <div class="icon" aria-hidden="true">💼</div>
            <div>
              <div style="font-weight:700">Portfolio</div>
              <div style="color:var(--muted); font-size:13px">
                <a href="https://your-portfolio.example.com" target="_blank" rel="noopener">your-portfolio.example.com</a>
              </div>
            </div>
          </div>
        </div>

        <div class="actions" style="margin-top:12px;">
          <a class="btn" href="mailto:you@example.com?subject=Opportunity">Get in touch</a>
          <a class="btn ghost" href="resume.pdf" download>Download PDF</a>
        </div>
      </div>

      <div class="card" aria-labelledby="skillsHeading">
        <div class="section-title">
          <h2 id="skillsHeading">Technologies & Skills</h2>
          <span class="pill">Core</span>
        </div>

        <div style="margin-bottom:10px; color:var(--muted); font-size:13px">Languages, frameworks, platforms I use daily.</div>

        <div class="skills-grid" role="list">
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>TypeScript & JavaScript</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Node.js & Express</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>React & Vite</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Electron & Desktop Apps</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Docker & CI/CD</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>MongoDB & PostgreSQL</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Observability: Prometheus / Grafana</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Testing: Jest, Playwright</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Type-safe APIs (OpenAPI / GraphQL)</div></div>
          <div class="skill" role="listitem"><div class="dot" aria-hidden="true"></div><div>Developer Experience & Tooling</div></div>
        </div>

        <div style="margin-top:12px; color:var(--muted); font-size:13px">
          <strong>Also familiar with:</strong> Rust basics, Go, AWS, Terraform, Nx / Monorepos.
        </div>
      </div>

      <div class="card" aria-labelledby="moreHeading">
        <div class="section-title">
          <h2 id="moreHeading">Open Source & Projects</h2>
        </div>

        <p style="color:var(--muted); margin:0 0 8px">
          I maintain several developer-focused projects. Highlights:
        </p>

        <ul style="margin:0 0 8px 18px; color:var(--muted);">
          <li><strong>mapped-har-opener</strong> — Desktop utility for HAR inspection (Electron + TypeScript).</li>
          <li><strong>ci-speedup</strong> — CI caching strategies for monorepos.</li>
        </ul>

        <div style="display:flex; gap:8px; margin-top:10px;">
          <a class="btn ghost" href="https://github.com/yourusername?tab=repositories" target="_blank" rel="noopener">View repos</a>
          <a class="btn" href="https://github.com/yourusername" target="_blank" rel="noopener">GitHub</a>
        </div>
      </div>
    </aside>
  </div>

  <!-- Simple accessibility helpers (no JS required) -->
</body>
</html>
