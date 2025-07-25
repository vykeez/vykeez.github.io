<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Vysakh Keezhedath | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet" />
  <style>
    :root {
      --primary: #0a192f;
      --accent: #38bdf8;
      --text: #e0e0e0;
      --bg: #f5f5f5;
      --dark-bg: #020c1b;
    }
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      font-family: 'Inter', sans-serif;
      background: var(--dark-bg);
      color: var(--text);
      line-height: 1.6;
    }
    nav {
      display:flex;
      justify-content:center;
      gap:1.5rem;
      padding:1rem;
      background: rgba(10,25,47,0.85);
      position:sticky;
      top:0;
      z-index:100;
    }
    nav a {
      color: var(--text);
      text-decoration:none;
      font-weight:600;
    }
    nav a:hover {
      color: var(--accent);
    }
    .hero {
      text-align:center;
      padding:6rem 1rem;
      background: url('header-bg.jpg') center/cover no-repeat;
    }
    .hero h1 {
      font-size:2.5rem;
      margin-bottom:0.5rem;
    }
    .hero p {
      font-size:1.25rem;
      color:#8892b0;
    }
    section {
      padding:4rem 1rem;
      max-width:900px;
      margin:auto;
    }
    h2 {
      font-size:1.75rem;
      color: var(--accent);
      margin-bottom:1rem;
      text-align:center;
    }
    ul, p { margin-bottom: 1rem; }
    .grid {
      display: grid;
      gap: 2rem;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    }
    .card {
      background: rgba(10,25,47,0.6);
      padding: 1.5rem;
      border-radius: 0.5rem;
    }
    .card h3 {
      margin-bottom: 0.5rem;
    }
    .timeline {
      list-style: none;
      padding-left: 1rem;
      border-left: 2px solid var(--accent);
    }
    .timeline li {
      margin-bottom: 1.5rem;
      padding-left: 1rem;
      position: relative;
    }
    .timeline li::before {
      content: '';
      position: absolute;
      left: -0.55rem;
      top: 0.35rem;
      width: 0.75rem;
      height: 0.75rem;
      background: var(--accent);
      border-radius: 50%;
    }
    a {
      color: var(--accent);
      text-decoration: none;
    }
    a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <nav>
    <a href="#home">Home</a>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#experience">Experience</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="home" class="hero">
    <h1>Hi! I'm Vysakh</h1>
    <p>Computer Networks Graduate | Systems and Cybersecurity Enthusiast</p>
  </section>

  <section id="about">
    <h2>About Me</h2>
    <p>I'm Vysakh Keezhedath, a Computer Networks graduate with a strong foundation in networking, cybersecurity, and systems administration. I’ve worked on routers, firewalls, Linux/Windows servers, and enjoy hands-on problem-solving.</p>
    <p>I currently work at Petro Canada and Loblaws, and previously gained tech experience at Amazon and as a Technician in India working with NAS and Raspberry Pi setups.</p>
  </section>

  <section id="skills">
    <h2>Skills</h2>
    <div class="grid">
      <div class="card"><h3>Networking</h3><p>OSPF, VLAN, NAT, VPN, DHCP, DNS</p></div>
      <div class="card"><h3>Cybersecurity</h3><p>Cisco Cert, ACLs, Syslog, SSH Hardening, ZPF Firewall</p></div>
      <div class="card"><h3>Systems</h3><p>Windows/Linux servers, Veeam, File Services, AD/DNS</p></div>
      <div class="card"><h3>Tools</h3><p>Wireshark, GNS3, Packet Tracer, VS Code, Git</p></div>
      <div class="card"><h3>Hardware</h3><p>NAS, Raspberry Pi, Routers, Server Builds</p></div>
    </div>
  </section>

  <section id="projects">
    <h2>Projects</h2>
    <div class="card">
      <h3>vSphere Datacenter Simulation (Capstone)</h3>
      <ul>
        <li>Deployed 14+ VMs with VLAN segmentation using OPNsense</li>
        <li>Configured AD, DNS, DHCP, iSCSI, Syslog, Proxy, HTTP, DFS</li>
        <li>Enabled Veeam backup, DFS replication, and thin provisioning</li>
      </ul>
    </div>
  </section>

  <section id="experience">
    <h2>Experience</h2>
    <ul class="timeline">
      <li><strong>Petro Canada</strong> – Manager (Present)</li>
      <li><strong>Loblaws</strong> – Employee (Present)</li>
      <li><strong>Amazon Warehouse</strong> – Associate (Past)</li>
      <li><strong>Cyber Systems, India</strong> – Technician (1 Year)</li>
    </ul>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Email: <a href="mailto:vkeez0002@gmail.com">vkeez0002@gmail.com</a></p>
    <p>GitHub: <a href="https://github.com/vykeez" target="_blank">github.com/vykeez</a></p>
  </section>
</body>
</html>
