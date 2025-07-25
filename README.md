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
      max-width:800px;
      margin: auto;
      padding:2rem;
    }
    h1 { font-size:2rem; margin-bottom:1rem; }
    h2 { font-size:1.25rem; color: var(--accent); margin-top:2rem; margin-bottom:0.5rem; }
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
    @media (max-width:600px) {
      .container { padding:1rem; }
    }
  </style>
</head>
<body>
  <button id="theme-toggle" aria-label="Toggle theme">🌞</button>
  <div class="container">
    <h1>Vysakh Keezhedath</h1>
    <p>Computer Networks graduate specializing in networking, cybersecurity, and systems administration.</p>
    <hr>
    <section>
      <h2>Skills</h2>
      <ul>
        <li>Networking: OSPF, VLANs, NAT, DHCP, Subnetting, VPN, DNS</li>
        <li>Cybersecurity: Cisco Cybersecurity Certificate, Firewall (ZPF), ACLs, SSH Hardening, Syslog Monitoring</li>
        <li>Systems & Servers: VMware vSphere, Windows Server, Linux (Ubuntu, Rocky), AD/DNS, File Services, DHCP, Veeam</li>
        <li>Hardware & Devices: Raspberry Pi, NAS setup, home server configuration, router troubleshooting</li>
      </ul>
    </section>
    <hr>
    <section>
      <h2>Education &amp; Certifications</h2>
      <ul>
        <li>Diploma in Computer Networking – Canada</li>
        <li>Cisco Cybersecurity Certification</li>
      </ul>
    </section>
    <hr>
    <section>
      <h2>Experience</h2>
      <ul>
        <li><strong>Petro Canada</strong> – Manager (Present)</li>
        <li><strong>Loblaws</strong> – Employee (Present)</li>
        <li><strong>Amazon Warehouse</strong> – Associate</li>
        <li><strong>Cyber Systems, India</strong> – Technician (1 Year)</li>
      </ul>
    </section>
    <hr>
    <section>
      <h2>Projects</h2>
      <ul>
        <li><strong>vSphere Datacenter Simulation (Capstone)</strong></li>
        <li>14+ VMs including Jump Server, AD/DNS, Syslog, Proxy, iSCSI, DFS, HTTP, and Backup</li>
        <li>Configured VLAN segmentation using OPNsense firewall</li>
        <li>Enabled thin provisioning, iSCSI storage, Syslog monitoring, Proxy filtering, and DFS replication</li>
      </ul>
    </section>
    <hr>
    <section>
      <h2>Contact</h2>
      <p>Email: <a href="mailto:vkeez0002@gmail.com">vkeez0002@gmail.com</a></p>
      <p>GitHub: <a href="https://github.com/vykeez" target="_blank">github.com/vykeez</a></p>
    </section>
  </div>
  <script>
    // Theme toggle
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
    // Load saved theme
    const saved = localStorage.getItem('theme') || 'dark';
    document.documentElement.setAttribute('data-theme', saved);
    updateIcon();
    // Fade-in on scroll
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
