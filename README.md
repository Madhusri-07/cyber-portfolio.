<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Madhusri S | Cybersecurity Student</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">
  <script src="https://kit.fontawesome.com/a2d9b6d9a1.js" crossorigin="anonymous"></script>

  <style>
    :root {
      --bg: #040b1a;
      --panel: #0a1428;
      --accent: #3b82f6; /* Blue glow */
      --accent-2: #60a5fa;
      --muted: #a9b8d4;
      --glass: rgba(255, 255, 255, 0.04);
      --glass-2: rgba(255, 255, 255, 0.03);
      font-family: 'Inter', system-ui, -apple-system, 'Segoe UI', Roboto, sans-serif;
      color-scheme: dark;
    }
    *{box-sizing:border-box}
    html, body {
      height: 100%;
      margin: 0;
      background: radial-gradient(circle at 20% 10%, rgba(59,130,246,0.1), transparent 10%), linear-gradient(180deg,#030817 0%, #01040b 100%);
      color: #dfeeff;
      overflow-x: hidden;
    }

    /* Background grid */
    .bg-grid {
      position: fixed;
      inset: 0;
      z-index: 0;
      pointer-events: none;
      background-image: linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px),
                        linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px);
      background-size: 120px 120px;
      animation: movegrid 40s linear infinite;
      opacity: 0.5;
    }
    @keyframes movegrid {
      from { background-position: 0 0, 0 0; }
      to { background-position: 120px 120px, 120px 120px; }
    }

    .container {
      position: relative;
      z-index: 2;
      max-width: 1100px;
      margin: 40px auto;
      padding: 32px;
    }

    header {
      display: flex;
      align-items: center;
      gap: 20px;
    }

    .logo {
      width: 72px;
      height: 72px;
      border-radius: 16px;
      background: linear-gradient(135deg, var(--accent), var(--accent-2));
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: 800;
      color: #020a18;
      box-shadow: 0 0 30px rgba(59,130,246,0.6);
      animation: floaty 4s ease-in-out infinite;
    }

    @keyframes floaty {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-6px); }
    }

    .name-block h1 { margin: 0; font-size: 30px; letter-spacing: 0.6px; }
    .name-block p { margin: 4px 0 0; color: var(--muted); }

    main { display: grid; grid-template-columns: 1fr 340px; gap: 28px; margin-top: 30px; }

    .card {
      background: var(--glass);
      border-radius: 14px;
      padding: 22px;
      backdrop-filter: blur(10px);
      box-shadow: 0 8px 40px rgba(0,0,0,0.7);
      transition: transform .3s ease, box-shadow .3s ease;
    }

    .card:hover { transform: translateY(-5px); box-shadow: 0 10px 40px rgba(0,0,0,0.9); }

    .intro { font-size: 15px; color: var(--muted); line-height: 1.6; margin-top: 10px; }

    .skills { display: flex; flex-wrap: wrap; gap: 10px; margin-top: 12px; }
    .skill {
      background: linear-gradient(180deg, rgba(255,255,255,0.05), rgba(255,255,255,0.02));
      border-radius: 999px;
      padding: 8px 14px;
      font-weight: 600;
      font-size: 13px;
      color: var(--accent-2);
      border: 1px solid rgba(255,255,255,0.05);
      transition: all 0.3s ease;
    }
    .skill:hover {
      background: var(--accent);
      color: #fff;
      box-shadow: 0 0 10px var(--accent);
    }

    h3 { margin-top: 16px; margin-bottom: 8px; color: var(--accent-2); }

    .projects { display: grid; gap: 12px; margin-top: 8px; }
    .project {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 12px;
      border-radius: 10px;
      background: linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));
      border: 1px solid rgba(255,255,255,0.05);
    }
    .project h4 { margin: 0; font-size: 15px; color: #fff; }
    .project p { margin: 4px 0 0; color: var(--muted); font-size: 13px; }
    .project div:last-child { color: var(--accent-2); font-weight: 700; }

    /* Contact section */
    .socials { display: flex; gap: 10px; flex-wrap: wrap; margin-top: 8px; }
    .socials a {
      text-decoration: none;
      color: var(--muted);
      background: var(--glass);
      padding: 8px 12px;
      border-radius: 10px;
      transition: all 0.3s ease;
    }
    .socials a:hover {
      color: #fff;
      background: var(--accent);
      box-shadow: 0 0 12px var(--accent);
    }

    .btn {
      display: inline-block;
      padding: 10px 16px;
      background: linear-gradient(90deg, var(--accent), var(--accent-2));
      border-radius: 10px;
      color: #fff;
      font-weight: 700;
      text-decoration: none;
      transition: all .3s;
    }
    .btn:hover { box-shadow: 0 0 20px var(--accent-2); }

    footer {
      margin-top: 30px;
      text-align: center;
      color: var(--muted);
      font-size: 13px;
    }

    @media (max-width: 900px) {
      main { grid-template-columns: 1fr; }
    }
  </style>
</head>

<body>
  <div class="bg-grid"></div>
  <div class="container">
    <header>
      <div class="logo">MS</div>
      <div class="name-block">
        <h1>Madhusri S</h1>
        <p>Cybersecurity Student • Building safer systems</p>
      </div>
    </header>

    <main>
      <section class="card">
        <h3>About Me</h3>
        <p class="intro">I'm a passionate Cybersecurity student with an interest in ethical hacking, network defense, and digital forensics. I love exploring attack patterns, securing networks, and applying blue-team strategies in real-world simulations.</p>

        <h3>Skills</h3>
        <div class="skills">
          <div class="skill">Python</div>
          <div class="skill">Linux</div>
          <div class="skill">Wireshark</div>
          <div class="skill">Burp Suite</div>
          <div class="skill">Networking</div>
          <div class="skill">Penetration Testing</div>
          <div class="skill">Git & GitHub</div>
        </div>

        <h3>Projects</h3>
        <div class="projects">
          <div class="project">
            <div class="meta">
              <h4>BlueSentinel: AI Phishing Detector</h4>
              <p>Machine learning model that detects phishing websites using URL and metadata analysis.</p>
            </div>
            <div>Demo</div>
          </div>
          <div class="project">
            <div class="meta">
              <h4>VulnScanX</h4>
              <p>Python-based vulnerability scanner for local network assessments.</p>
            </div>
            <div>Code</div>
          </div>
          <div class="project">
            <div class="meta">
              <h4>LockdownVault</h4>
              <p>Encrypted password manager with AES-256 encryption and key rotation.</p>
            </div>
            <div>View</div>
          </div>
          <div class="project">
            <div class="meta">
              <h4>PacketEye</h4>
              <p>Custom packet analyzer tool built using Scapy for learning network traffic inspection.</p>
            </div>
            <div>Code</div>
          </div>
          <div class="project">
            <div class="meta">
              <h4>CyberShield Dashboard</h4>
              <p>Interactive dashboard showing simulated attack logs and security alerts.</p>
            </div>
            <div>Live</div>
          </div>
        </div>

        <h3>Certificates</h3>
        <div class="skills">
          <div class="skill">Ethical Hacking – Coursera</div>
          <div class="skill">Introduction to Cybersecurity – Cisco</div>
          <div class="skill">Python for Security – edX</div>
        </div>

        <footer>Made with 💙 by Madhusri • Stay ethical, stay secure 🛡️</footer>
      </section>

      <aside class="card">
        <h3>Contact</h3>
        <p>Let's collaborate or discuss cybersecurity! Reach out 👇</p>
        <div class="socials">
          <a href="https://github.com/madhusri-sec" target="_blank"><i class="fab fa-github"></i> GitHub</a>
          <a href="https://linkedin.com/in/madhusri-sec" target="_blank"><i class="fab fa-linkedin"></i> LinkedIn</a>
          <a href="mailto:madhusri.cyber@example.com"><i class="fas fa-envelope"></i> Email</a>
        </div>
        <div style="margin-top:16px;">
          <a class="btn" href="https://github.com/madhusri-sec" target="_blank">View GitHub</a>
        </div>
      </aside>
    </main>
  </div>

  <script>
    // Floating blue particles
    (function createDots(){
      const container = document.createElement('div');
      container.style.position = 'fixed';
      container.style.inset = '0';
      container.style.zIndex = '1';
      container.style.pointerEvents = 'none';
      for(let i=0;i<15;i++){
        const d = document.createElement('div');
        d.style.width = d.style.height = (6+Math.random()*18)+'px';
        d.style.borderRadius = '50%';
        d.style.position = 'absolute';
        d.style.left = Math.random()*100+'%';
        d.style.top = Math.random()*100+'%';
        d.style.opacity = 0.05+Math.random()*0.3;
        d.style.background = 'radial-gradient(circle, rgba(59,130,246,0.9), rgba(96,165,250,0.5))';
        d.style.filter = 'blur(8px)';
        d.style.transform = 'translate(-50%, -50%)';
        d.style.animation = `floaty ${8+Math.random()*10}s ease-in-out ${Math.random()*5}s infinite`;
        container.appendChild(d);
      }
      document.body.appendChild(container);
    })();
  </script>
</body>
</html>
