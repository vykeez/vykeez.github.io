<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Vysakh Keezhedath</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --main-bg: #0f172a;
      --card-bg: #1e293b;
      --accent: #38bdf8;
      --text: #f8fafc;
      --muted: #94a3b8;
    }
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }
    body {
      font-family: 'Roboto', sans-serif;
      background: var(--main-bg);
      color: var(--text);
      line-height: 1.6;
    }
    header {
      background: url('https://source.unsplash.com/1600x600/?cybersecurity,network') no-repeat center/cover;
      text-align: center;
      padding: 6rem 2rem;
      color: white;
    }
    header h1 {
      font-size: 3rem;
    }
    header p {
      font-size: 1.25rem;
      color: #e2e8f0;
    }
    .container {
      max-width: 1000px;
      margin: auto;
      padding: 2rem;
    }
    h2 {
      color: var(--accent);
      margin-bottom: 1rem;
      border-bottom: 2px solid var(--accent);
      display: inline-block;
      padding-bottom: 0.25rem;
    }
    .card {
      background: var(--card-bg);
      padding: 1.5rem;
      border-radius: 8px;
      margin-bottom: 1.5rem;
    }
    .card h3 {
      color: var(--accent);
      margin-bottom: 0.5rem;
    }
    .skill-bar {
      height: 8px;
      background: var(--muted);
      border-radius: 4px;
      overflow: hidden;
      margin-top: 0.5rem;
    }
    .skill-fill {
      height: 100%;
      background: var(--accent);
      transition: width 1s ease-in-out;
    }
    .skill-label {
      display: flex;
      justify-content: space-between;
      margin-top: 0.25rem;
    }
    footer {
      text-align: center;
      margin-top: 4rem;
      color: var(--muted);
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>Vysakh Keezhedath</h1>
    <p>Systems Technician | Networking and Cybersecurity Specialist</p>
  </header>
  <div class="container">
    <section>
      <h2>About Me</h2>
      <p>Hi, I'm Vysakh Keezhedath. Welcome to my portfolio website! I am a Network and Systems Engineer. I am excited to share with you my work and experience in this field.</p>
      <p>I have always had a passion for Computer Systems and Networking and have pursued it throughout my education and career. I graduated from Informatics Academy with a degree in Network Engineering and have since gained valuable experience through Apprenticeship and job opportunities.</p>
    </section>

    <section>
      <h2>Education</h2>
      <div class="card">
        <h3>Diploma in Computer Systems Technician and Networking</h3>
        <p>Completed at Informatics Academy with focus on Networking and System Technologies.</p>
      </div>
      <div class="card">
        <h3>Cisco Cybersecurity Certificate</h3>
        <p>Credential earned as part of specialization in Network Security and Cyber Defense.</p>
      </div>
      <div class="card">
        <h3>Google Cybersecurity Certificate</h3>
        <p>Professional Certificate covering risk management, incident response, and tools.</p>
      </div>
      <div class="card">
        <h3>Apprenticeship – Algonquin College</h3>
        <p>Hands-on lab training during studies: Networking Lab, Linux Lab, Server Room, PC Troubleshooting, IT Service Center.</p>
      </div>
    </section>

    <section>
      <h2>Skills</h2>
      <div class="card">
        <div class="skill-label"><span>Routing</span><span>90%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 90%"></div></div>

        <div class="skill-label"><span>Firewalling</span><span>90%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 90%"></div></div>

        <div class="skill-label"><span>Windows Server</span><span>70%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 70%"></div></div>

        <div class="skill-label"><span>Linux Server</span><span>65%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 65%"></div></div>

        <div class="skill-label"><span>Load Balancer</span><span>70%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 70%"></div></div>

        <div class="skill-label"><span>Web Proxy</span><span>90%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 90%"></div></div>

        <div class="skill-label"><span>Virtualization</span><span>65%</span></div>
        <div class="skill-bar"><div class="skill-fill" style="width: 65%"></div></div>
      </div>
    </section>

    <section>
      <h2>Projects</h2>
      <div class="card">
        <h3>vSphere Datacenter Simulation</h3>
        <p>Deployed 14+ VMs including Jump Server, AD/DNS, Syslog, Proxy, iSCSI, DFS, HTTP, and Backup using OPNsense firewall, iSCSI storage, DFS replication, and Syslog monitoring.</p>
      </div>
    </section>

    <section>
      <h2>Experience</h2>
      <ul>
        <li><strong>Petro Canada</strong> – Manager (Present)</li>
        <li><strong>Loblaws</strong> – Employee (Present)</li>
        <li><strong>Amazon Warehouse</strong> – Associate</li>
        <li><strong>Cyber Systems, India</strong> – Technician (1 Year)</li>
      </ul>
    </section>

    <section>
      <h2>Contact</h2>
      <p>Email: <a href="mailto:vkeez0002@gmail.com">vkeez0002@gmail.com</a></p>
      <p>GitHub: <a href="https://github.com/vykeez" target="_blank">github.com/vykeez</a></p>
    </section>
  </div>
  <footer>
    <p>&copy; 2025 Vysakh Keezhedath</p>
  </footer>
</body>
</html>
