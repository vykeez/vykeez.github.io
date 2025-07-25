<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vysakh Keezhedath</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg: #000;
      --fg: #fff;
      --accent: #38bdf8;
      --hr: #333;
    }
    [data-theme="light"] {
      --bg: #fff;
      --fg: #000;
      --accent: #0066cc;
      --hr: #ddd;
    }
    * {
      margin: 0; padding: 0; box-sizing: border-box;
    }
    body {
      background: var(--bg);
      color: var(--fg);
      font-family: 'Poppins', sans-serif;
      line-height: 1.6;
      transition: background 0.3s, color 0.3s;
    }
    .container {
      max-width: 1100px;
      margin: auto;
      padding: 2rem;
    }
    h1, h2 {
      font-weight: 600;
      margin-bottom: 1rem;
    }
    .about, .skills, .education {
      margin-bottom: 3rem;
    }
    .skills-bar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin: 0.5rem 0;
    }
    .skills-bar .label {
      flex: 1;
    }
    .skills-bar .bar {
      flex: 3;
      height: 8px;
      background: #333;
      margin-left: 1rem;
      position: relative;
      border-radius: 4px;
    }
    .skills-bar .bar::after {
      content: '';
      position: absolute;
      height: 8px;
      border-radius: 4px;
      background: var(--accent);
      width: var(--value);
    }
    .education-card {
      background: #111;
      border-left: 6px solid var(--accent);
      padding: 1rem;
      margin: 1rem 0;
      border-radius: 8px;
    }
    #theme-toggle {
      position: fixed;
      top: 1rem;
      right: 1rem;
      background: none;
      border: none;
      font-size: 1.5rem;
      cursor: pointer;
      color: var(--fg);
    }
  </style>
</head>
<body>
  <button id="theme-toggle" aria-label="Toggle theme">🌞</button>
  <div class="container">
    <section class="about">
      <h1>Vysakh Keezhedath</h1>
      <p>Systems Technician, Networking and Cybersecurity Specialist</p>
      <p>Hi I'm Vysakh Keezhedath. Welcome to my portfolio website! I am a Network and Systems Engineer. I am excited to share with you my work and experience in this field.</p>
      <p>I have always had a passion for Computer Systems and Networking and have pursued it throughout my education and career. I graduated with a diploma in Computer Systems Technician and Networking and have since gained valuable experience through apprenticeship and job opportunities.</p>
    </section>

    <section class="skills">
      <h2>Skills</h2>
      <div class="skills-bar"><span class="label">Routing</span><div class="bar" style="--value: 90%;"></div></div>
      <div class="skills-bar"><span class="label">Switching</span><div class="bar" style="--value: 80%;"></div></div>
      <div class="skills-bar"><span class="label">Firewalling</span><div class="bar" style="--value: 90%;"></div></div>
      <div class="skills-bar"><span class="label">Mail Security</span><div class="bar" style="--value: 90%;"></div></div>
      <div class="skills-bar"><span class="label">Windows Server</span><div class="bar" style="--value: 70%;"></div></div>
      <div class="skills-bar"><span class="label">Load-Balancer</span><div class="bar" style="--value: 70%;"></div></div>
      <div class="skills-bar"><span class="label">Web Security - Proxy</span><div class="bar" style="--value: 90%;"></div></div>
      <div class="skills-bar"><span class="label">E-Mail Encryption</span><div class="bar" style="--value: 85%;"></div></div>
      <div class="skills-bar"><span class="label">Linux Server</span><div class="bar" style="--value: 65%;"></div></div>
      <div class="skills-bar"><span class="label">Virtualisation</span><div class="bar" style="--value: 65%;"></div></div>
    </section>

    <section class="education">
      <h2>Education & Certifications</h2>
      <div class="education-card">
        <h3>Diploma in Computer Systems Technician and Networking</h3>
        <p>Completed in Canada with focus on Systems, Networking and Cybersecurity. Gained hands-on training in network lab, Linux lab, server room, and IT service center.</p>
      </div>
      <div class="education-card">
        <h3>Cisco Cybersecurity Certificate</h3>
        <p>Completed training on threat detection, security fundamentals, and access control.</p>
      </div>
      <div class="education-card">
        <h3>Google Cybersecurity Certificate</h3>
        <p>Learned practical security operations and risk management techniques.</p>
      </div>
      <div class="education-card">
        <h3>Apprenticeship at Algonquin College</h3>
        <p>Practical exposure in Network Labs, Linux labs, PC troubleshooting, and service center operations during diploma program.</p>
      </div>
    </section>
  </div>
  <script>
    const toggle = document.getElementById('theme-toggle');
    function updateIcon() {
      const theme = document.documentElement.getAttribute('data-theme');
      toggle.textContent = theme === 'light' ? '🌜' : '🌞';
    }
    toggle.addEventListener('click', () => {
      const current = document.documentElement.getAttribute('data-theme');
      const target = current === 'light' ? 'dark' : 'light';
      document.documentElement.setAttribute('data-theme', target);
      localStorage.setItem('theme', target);
      updateIcon();
    });
    const saved = localStorage.getItem('theme') || 'dark';
    document.documentElement.setAttribute('data-theme', saved);
    updateIcon();
  </script>
</body>
</html>
