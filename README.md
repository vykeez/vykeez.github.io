<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Vysakh Keezhedath | Portfolio</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <script src="https://kit.fontawesome.com/a076d05399.js" crossorigin="anonymous"></script>
  <style>
    :root {
      --bg: #0f172a;
      --fg: #f1f5f9;
      --accent: #38bdf8;
      --card-bg: #1e293b;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Inter', sans-serif;
      background-color: var(--bg);
      color: var(--fg);
      line-height: 1.6;
    }
    header {
      background: var(--card-bg);
      padding: 2rem 1rem;
      text-align: center;
    }
    header h1 {
      font-size: 2.5rem;
      margin-bottom: 0.5rem;
    }
    header p {
      color: #94a3b8;
    }
    .profile-pic {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid var(--accent);
      margin-bottom: 1rem;
    }
    main {
      max-width: 960px;
      margin: auto;
      padding: 2rem 1rem;
    }
    section {
      margin-bottom: 2rem;
      background: var(--card-bg);
      padding: 1.5rem;
      border-radius: 0.75rem;
      box-shadow: 0 2px 8px rgba(0,0,0,0.2);
    }
    h2 {
      color: var(--accent);
      margin-bottom: 1rem;
    }
    ul {
      padding-left: 1.5rem;
    }
    a {
      color: var(--accent);
      text-decoration: none;
    }
    .resume-btn {
      display: inline-block;
      margin-top: 1rem;
      padding: 0.5rem 1rem;
      background-color: var(--accent);
      color: #0f172a;
      font-weight: bold;
      border-radius: 0.5rem;
      text-decoration: none;
      transition: background 0.3s;
    }
    .resume-btn:hover {
      background-color: #0ea5e9;
    }
    footer {
      text-align: center;
      padding: 2rem 1rem;
      font-size: 0.9rem;
      color: #94a3b8;
    }
  </style>
</head>
<body>
  <header>
    <img src="profile.jpg" alt="Profile Photo" class="profile-pic" />
    <h1>Vysakh Keezhedath</h1>
    <p>Computer Network Graduate | Cybersecurity & Systems Admin</p>
    <a href="resume.pdf" class="resume-btn" download><i class="fas fa-download"></i> Download Resume</a>
  </header>
  <main>
    <section>
      <h2>✨ Skills</h2>
      <ul>
        <li>Networking: OSPF, VLANs, NAT, DHCP, VPN, DNS</li>
        <li>Cybersecurity: Cisco Cybersecurity Certificate, Firewall (ZPF), ACLs, Syslog, SSH</li>
        <li>Servers & Tools: VMware vSphere, Veeam, Windows/Linux Servers, Git, Packet Tracer</li>
        <li>Hardware: Raspberry Pi, NAS, home servers, routers, troubleshooting</li>
      </ul>
    </section>
    <section>
      <h2>🎓 Education & Certifications</h2>
      <ul>
        <li>Diploma in Computer Networking – Canada</li>
        <li>Cisco Cybersecurity Certification</li>
      </ul>
    </section>
    <section>
      <h2>💼 Experience</h2>
      <ul>
        <li><strong>Petro Canada</strong> – Manager (Present)</li>
        <li><strong>Loblaws</strong> – Employee (Present)</li>
        <li><strong>Amazon Warehouse</strong> – Associate</li>
        <li><strong>Cyber Systems, India</strong> – Technician (1 Year) – Router setup, PC repair, NAS, Raspberry Pi</li>
      </ul>
    </section>
    <section>
      <h2>📁 Projects</h2>
      <p><strong>vSphere Datacenter Simulation</strong> – Capstone Project</p>
      <ul>
        <li>14+ VMs including AD, DNS, DHCP, Syslog, iSCSI, DFS, HTTP, Proxy</li>
        <li>Used OPNsense for VLAN routing and firewall</li>
        <li>Configured backup (Veeam), DFS replication, thin provisioning</li>
      </ul>
    </section>
    <section>
      <h2>📧 Contact</h2>
      <p><i class="fas fa-envelope"></i> Email: <a href="mailto:vkeez0002@gmail.com">vkeez0002@gmail.com</a></p>
      <p><i class="fab fa-github"></i> GitHub: <a href="https://github.com/vykeez" target="_blank">github.com/vykeez</a></p>
    </section>
  </main>
  <footer>
    &copy; 2025 Vysakh Keezhedath. All rights reserved.
  </footer>
</body>
</html>
