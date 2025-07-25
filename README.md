<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vysakh Keezhedath</title>
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
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      background: var(--bg);
      color: var(--fg);
      font-family: system-ui, sans-serif;
      line-height: 1.5;
      transition: background 0.3s, color 0.3s;
    }
    .container {
      max-width:1000px;
      margin: auto;
      padding:2rem;
    }
    h1 { font-size:2.5rem; margin-bottom:0.5rem; }
    h2 { font-size:1.5rem; color: var(--accent); margin-top:2rem; margin-bottom:0.5rem; }
    ul { padding-left:1.2rem; }
    li { margin-bottom:0.5rem; }
    a { color: var(--accent); text-decoration:none; }
    a:hover { text-decoration:underline; }
    hr { border:none; border-top:1px solid var(--hr); margin:2rem 0; }
    #theme-toggle {
      position: fixed;
      top:1rem;
      right:1rem;
      background:none;
      border:none;
      font-size:1.5rem;
      cursor:pointer;
      color: var(--fg);
      transition: color 0.3s;
    }
    section {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.6s ease-out, transform 0.6s ease-out;
    }
    section.visible {
      opacity:1;
      transform:translateY(0);
    }
    .skills-container, .cards-container {
      display: grid;
      gap: 1rem;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    }
    .card {
      background: #111;
      padding: 1rem;
      border-radius: 0.5rem;
      border-top: 5px solid var(--accent);
    }
    .progress-bar {
      background: #222;
      height: 8px;
      border-radius: 5px;
      margin-top: 5px;
      overflow: hidden;
    }
    .progress-bar span {
      display: block;
      height: 100%;
      background: var(--accent);
    }
    @media (max-width:600px) {
      .container { padding:1rem; }
    }
  </style>
</head>
<body>
  <button id="theme-toggle" aria-label="Toggle theme">🌞</button>
  <div class="container">
    <h1>Vysakh Keezhedath</h1>
    <p>Systems Technician, Networking and Cybersecurity Specialist</p>
    <hr>

    <section>
      <h2>About Me</h2>
      <p>Hi, I'm Vysakh Keezhedath. Welcome to my portfolio website! I am a Network and Systems Engineer excited to share my work and experience. I've always had a passion for computer systems and networking, which I pursued through formal education and hands-on experience. I am committed to advancing in the field through continuous learning and practical application.</p>
    </section>

    <hr>
    <section>
      <h2>Job Experience</h2>
      <ul>
        <li><strong>Petro Canada</strong> – Manager (Present)<br>Supervising store operations and resolving tech issues (POS, network)</li>
        <li><strong>Loblaws</strong> – Employee (Present)<br>Supporting backend systems and logistics operations</li>
        <li><strong>Amazon Warehouse</strong> – Associate<br>Logistics and scanning systems, hands-on tech troubleshooting</li>
        <li><strong>Cyber Systems – India</strong> – Technician (1 Year)<br>Worked on SOHO routers, PC repair, NAS setup, and Raspberry Pi deployments</li>
        <li><strong>Apprenticeship – Algonquin College (Student Placement)</strong><br>Worked in Networking Labs, Linux Labs, Server Rooms, and IT Service Desk troubleshooting PCs and configuring enterprise infrastructure</li>
      </ul>
    </section>

    <hr>
    <section>
      <h2>Education & Certifications</h2>
      <ul>
        <li><strong>Diploma:</strong> Computer Systems Technician – Networking (Canada)</li>
        <li><strong>Certificates:</strong> Cisco Cybersecurity, Google Cybersecurity</li>
      </ul>
    </section>

    <hr>
    <section>
      <h2>Skills</h2>
      <div class="skills-container">
        <div>
          <strong>Routing</strong>
          <div class="progress-bar"><span style="width: 90%"></span></div>
        </div>
        <div>
          <strong>Switching</strong>
          <div class="progress-bar"><span style="width: 80%; background: #f44"></span></div>
        </div>
        <div>
          <strong>Firewalling</strong>
          <div class="progress-bar"><span style="width: 90%; background: gold"></span></div>
        </div>
        <div>
          <strong>Web Security - Proxy</strong>
          <div class="progress-bar"><span style="width: 90%; background: violet"></span></div>
        </div>
        <div>
          <strong>Mail Security</strong>
          <div class="progress-bar"><span style="width: 90%; background: teal"></span></div>
        </div>
        <div>
          <strong>E-Mail Encryption</strong>
          <div class="progress-bar"><span style="width: 85%; background: #66f"></span></div>
        </div>
        <div>
          <strong>Windows Server</strong>
          <div class="progress-bar"><span style="width: 70%"></span></div>
        </div>
        <div>
          <strong>Linux Server</strong>
          <div class="progress-bar"><span style="width: 65%"></span></div>
        </div>
        <div>
          <strong>Load-Balancer</strong>
          <div class="progress-bar"><span style="width: 70%"></span></div>
        </div>
        <div>
          <strong>Virtualisation</strong>
          <div class="progress-bar"><span style="width: 65%"></span></div>
        </div>
      </div>
    </section>

    <hr>
    <section>
      <h2>Specialties</h2>
      <div class="cards-container">
        <div class="card">
          <h3>Routing</h3>
          <p>Configured, managed and replaced 42+ Cisco WAN routers, with IKEv2 VPN tunnels.</p>
        </div>
        <div class="card">
          <h3>Switching</h3>
          <p>Experience with Spanning Tree, vPC, VXLAN, and L2/L3 switching configuration.</p>
        </div>
        <div class="card">
          <h3>Information Security</h3>
          <p>Firewalling, Mail Security, Web Security, Encryption, VPN, SSL, and RSA integration.</p>
        </div>
        <div class="card">
          <h3>Windows & Linux</h3>
          <p>Administered AD, DNS, DHCP and file systems in both Windows and Linux environments.</p>
        </div>
        <div class="card">
          <h3>Load-Balancer</h3>
          <p>Application Layer balancing (L4–L7), Citrix ADC, and High-Availability design.</p>
        </div>
        <div class="card">
          <h3>System Administration</h3>
          <p>Maintaining servers, backups, syslog, proxy, monitoring tools, and patching infrastructure.</p>
        </div>
      </div>
    </section>

    <hr>
    <section>
      <h2>Contact</h2>
      <p>Email: <a href="mailto:vkeez0002@gmail.com">vkeez0002@gmail.com</a></p>
      <p>GitHub: <a href="https://github.com/vykeez" target="_blank">github.com/vykeez</a></p>
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
    document.addEventListener('DOMContentLoaded', () => {
      const sections = document.querySelectorAll('section');
      const obs = new IntersectionObserver((entries) => {
        entries.forEach(entry => {
          if (entry.isIntersecting) {
            entry.target.classList.add('visible');
            obs.unobserve(entry.target);
          }
        });
      }, { threshold: 0.1 });
      sections.forEach(sec => obs.observe(sec));
    });
  </script>
</body>
</html>
