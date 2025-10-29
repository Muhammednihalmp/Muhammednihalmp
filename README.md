<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Muhammed Nihal MP — Ethical Hacker & Hardware Innovator</title>
  <link href="https://fonts.googleapis.com/css2?family=Fira+Code:wght@400;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"/>
  <style>
    :root {
      --bg: #0D1117;
      --text: #FFFFFF;
      --accent: #00F7FF;
      --card: #161B22;
      --border: #30363D;
      --fire: #FF6B6B;
    }
    * { margin:0; padding:0; box-sizing:border-box; }
    body {
      background: var(--bg);
      color: var(--text);
      font-family: 'Fira Code', monospace;
      line-height: 1.7;
      overflow-x: hidden;
    }
    .container { max-width: 1000px; margin: auto; padding: 2rem; }
    header { text-align:center; padding: 3rem 0; position:relative; }
    .glitch {
      font-size: 2.5rem;
      font-weight: 600;
      color: var(--accent);
      animation: glitch 2s infinite;
      text-shadow: 0 0 10px var(--accent);
    }
    @keyframes glitch {
      0%,100% { text-shadow: 2px 2px 0 #ff00ff, -2px -2px 0 #00ffff; }
      50% { text-shadow: -2px -2px 0 #ff00ff, 2px 2px 0 #00ffff; }
    }
    .typing {
      font-size: 1.4rem;
      color: var(--accent);
      margin: 1.5rem 0;
      overflow: hidden;
      white-space: nowrap;
      border-right: 3px solid var(--accent);
      animation: typing 4s steps(40) infinite, blink .75s step-end infinite;
    }
    @keyframes typing {
      0%,100% { width: 0; }
      50% { width: 100%; }
    }
    @keyframes blink { 50% { border-color:transparent; } }
    .badges { margin: 1.5rem 0; }
    .badge {
      display: inline-block;
      padding: .5rem 1rem;
      margin: .3rem;
      background: var(--card);
      border: 1px solid var(--border);
      border-radius: 2rem;
      color: var(--text);
      text-decoration: none;
      transition: .3s;
    }
    .badge:hover { transform: translateY(-3px); box-shadow: 0 5px 15px rgba(0,247,255,.2); }
    .badge i { margin-right: .5rem; color: var(--accent); }
    .divider {
      height: 1px;
      background: linear-gradient(90deg, transparent, var(--accent), transparent);
      margin: 3rem 0;
    }
    section { margin-bottom: 4rem; }
    h2 {
      font-size: 1.8rem;
      color: var(--accent);
      margin-bottom: 1rem;
      position: relative;
      display: inline-block;
    }
    h2::after {
      content: '';
      position: absolute;
      bottom: -8px;
      left: 0;
      width: 50%;
      height: 3px;
      background: var(--accent);
      border-radius: 2px;
    }
    .code-block {
      background: var(--card);
      padding: 1.5rem;
      border-radius: .8rem;
      border: 1px solid var(--border);
      overflow-x: auto;
      font-family: 'Fira Code', monospace;
      color: #7FFFD4;
    }
    .code-block .comment { color: #6A9955; }
    .code-block .string { color: #CE9178; }
    .code-block .keyword { color: #569CD6; }
    .projects {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
    }
    .project-card {
      background: var(--card);
      padding: 1.5rem;
      border-radius: .8rem;
      border: 1px solid var(--border);
      transition: .3s;
    }
    .project-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 10px 25px rgba(0,247,255,.15);
      border-color: var(--accent);
    }
    .tech-tags {
      margin-top: 1rem;
      display: flex;
      flex-wrap: wrap;
      gap: .5rem;
    }
    .tag {
      background: rgba(0,247,255,.1);
      color: var(--accent);
      padding: .3rem .7rem;
      border-radius: .5rem;
      font-size: .8rem;
      border: 1px solid var(--accent);
    }
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(auto-fill, minmax(80px, 1fr));
      gap: .8rem;
      margin: 1.5rem 0;
    }
    .skill-icon {
      background: var(--card);
      padding: .8rem;
      border-radius: .8rem;
      text-align: center;
      border: 1px solid var(--border);
      transition: .3s;
    }
    .skill-icon:hover {
      background: rgba(0,247,255,.1);
      border-color: var(--accent);
      transform: scale(1.1);
    }
    .skill-icon img { width: 40px; height: 40px; filter: brightness(0) invert(1); }
    .os-badges {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      gap: .8rem;
      margin: 1.5rem 0;
    }
    .os-badge {
      background: var(--card);
      padding: .5rem 1rem;
      border-radius: 2rem;
      border: 1px solid var(--border);
      font-size: .9rem;
    }
    .stats {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 1.5rem;
      margin: 2rem 0;
    }
    .stats img {
      width: 100%;
      border-radius: .8rem;
      border: 1px solid var(--border);
    }
    .mermaid {
      background: var(--card);
      padding: 1.5rem;
      border-radius: .8rem;
      border: 1px solid var(--border);
      overflow: auto;
    }
    .goals table {
      width: 100%;
      border-collapse: collapse;
      margin: 1.5rem 0;
    }
    .goals td {
      padding: 1rem;
      border: 1px solid var(--border);
      text-align: center;
    }
    .goals .in-progress { color: #FFA500; }
    .goals .planning { color: #9370DB; }
    .philosophy {
      background: linear-gradient(135deg, rgba(0,247,255,.1), rgba(255,0,255,.1));
      padding: 2rem;
      border-radius: 1rem;
      border: 1px solid var(--accent);
      text-align: center;
      margin: 2rem 0;
      font-style: italic;
      color: var(--accent);
    }
    .connect {
      text-align: center;
      padding: 3rem 0;
    }
    .btn {
      display: inline-block;
      background: var(--accent);
      color: var(--bg);
      padding: .8rem 1.8rem;
      margin: .5rem;
      border-radius: 2rem;
      text-decoration: none;
      font-weight: 600;
      transition: .3s;
      box-shadow: 0 0 20px rgba(0,247,255,.4);
    }
    .btn:hover {
      transform: scale(1.05);
      box-shadow: 0 0 30px rgba(0,247,255,.6);
    }
    .views {
      display: inline-block;
      background: var(--card);
      padding: .5rem 1rem;
      border-radius: 2rem;
      border: 1px solid var(--accent);
      color: var(--accent);
      font-size: .9rem;
      margin-top: 1rem;
    }
    footer {
      text-align: center;
      padding: 2rem 0;
      color: var(--accent);
      font-size: .9rem;
    }
    .matrix-rain {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      pointer-events: none;
      z-index: -1;
      opacity: 0.05;
    }
    @media (max-width: 768px) {
      .glitch { font-size: 2rem; }
      .typing { font-size: 1.1rem; }
      .projects { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>

<canvas class="matrix-rain" id="matrix"></canvas>

<div class="container">

  <header>
    <h1 class="glitch">🛡️ Muhammed Nihal MP</h1>
    <p>💻 Computer Engineer | 🔐 Ethical Hacker | 🔧 Hardware Innovator</p>
    <div class="typing">Cybersecurity Specialist • IoT & Hardware Hacker • Full Stack Developer • Penetration Testing Expert</div>

    <div class="badges">
      <a href="mailto:muhammadnihalmp955@gmail.com" class="badge"><i class="fas fa-envelope"></i> Email</a>
      <a href="https://www.linkedin.com/in/muhammed-nihal-mp-96a346283/" class="badge"><i class="fab fa-linkedin"></i> LinkedIn</a>
      <a href="https://t.me/Muhammed_Nihal_MP" class="badge"><i class="fab fa-telegram"></i> Telegram</a>
    </div>
  </header>

  <div class="divider"></div>

  <section id="about">
    <h2>🎯 About Me</h2>
    <div class="code-block">
      <span class="keyword">class</span> <span style="color:#4EC9B0">EthicalHacker</span>:<br>
      &nbsp;&nbsp;<span class="keyword">def</span> <span style="color:#DCDCAA">__init__</span>(self):<br>
      &nbsp;&nbsp;&nbsp;&nbsp;self.name = <span class="string">"Muhammed Nihal MP"</span><br>
      &nbsp;&nbsp;&nbsp;&nbsp;self.role = <span class="string">"Computer Engineer & Security Researcher"</span><br>
      &nbsp;&nbsp;&nbsp;&nbsp;self.education = <span class="string">"Diploma in Computer Engineering"</span><br>
      &nbsp;&nbsp;&nbsp;&nbsp;self.institution = <span class="string">"Ma'din College of Engineering, Kerala, India"</span><br>
      &nbsp;&nbsp;&nbsp;&nbsp;self.location = <span class="string">"Kerala, India 🇮🇳"</span><br><br>
      &nbsp;&nbsp;<span class="keyword">def</span> <span style="color:#DCDCAA">current_focus</span>(self):<br>
      &nbsp;&nbsp;&nbsp;&nbsp;<span class="keyword">return</span> [<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="string">"ESP32-based Penetration Testing Devices"</span>,<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="string">"Telegram Bot Automation for IoT"</span>,<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="string">"Wi-Fi & Bluetooth Exploitation Tools"</span>,<br>
      &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<span class="string">"Hardware Hacking & Reverse Engineering"</span><br>
      &nbsp;&nbsp;&nbsp;&nbsp;]<br><br>
      &nbsp;&nbsp;<span class="keyword">def</span> <span style="color:#DCDCAA">life_motto</span>(self):<br>
      &nbsp;&nbsp;&nbsp;&nbsp;<span class="keyword">return</span> <span class="string">"Understanding systems deeply to make them better"</span>
    </div>
  </section>

  <section id="projects">
    <h2>🚀 Current Projects</h2>
    <div class="projects">
      <div class="project-card">
        <h3>🔧 ESP32 Hacking Suite</h3>
        <p>Building advanced ESP32-based pentesting gadgets for wireless security auditing and IoT exploitation.</p>
        <div class="tech-tags">
          <span class="tag">ESP32</span>
          <span class="tag">C++</span>
          <span class="tag">Arduino</span>
          <span class="tag">Wi-Fi</span>
          <span class="tag">BLE</span>
        </div>
      </div>
      <div class="project-card">
        <h3>🤖 Telegram IoT Bots</h3>
        <p>Developing intelligent automation bots for remote IoT control and penetration testing workflows.</p>
        <div class="tech-tags">
          <span class="tag">Python</span>
          <span class="tag">Telegram API</span>
          <span class="tag">IoT Protocols</span>
        </div>
      </div>
    </div>
  </section>

  <section id="tech">
    <h2>💻 Tech Arsenal</h2>

    <h3>Programming Languages</h3>
    <div class="skills-grid">
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=python&theme=dark" alt="Python"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=cpp&theme=dark" alt="C++"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=c&theme=dark" alt="C"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=java&theme=dark" alt="Java"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=php&theme=dark" alt="PHP"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=bash&theme=dark" alt="Bash"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=go&theme=dark" alt="Go"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=rust&theme=dark" alt="Rust"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=js&theme=dark" alt="JavaScript"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=html&theme=dark" alt="HTML"/></div>
      <div class="skill-icon"><img src="https://skillicons.dev/icons?i=css&theme=dark" alt="CSS"/></div>
    </div>

    <h3>Hardware & IoT</h3>
    <div class="os-badges">
      <span class="os-badge">ESP32</span>
      <span class="os-badge">Arduino</span>
      <span class="os-badge">Raspberry Pi</span>
      <span class="os-badge">IoT</span>
    </div>

    <h3>Operating Systems</h3>
    <div class="os-badges">
      <span class="os-badge">Kali Linux</span>
      <span class="os-badge">Parrot OS</span>
      <span class="os-badge">Ubuntu</span>
      <span class="os-badge">Windows</span>
    </div>
  </section>

  <section id="stats">
    <h2>📊 GitHub Analytics</h2>
    <div class="stats">
      <img src="https://github-readme-stats.vercel.app/api?username=Muhammednihalmp&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true&bg_color=0D1117&title_color=00F7FF&icon_color=00F7FF&text_color=FFFFFF" alt="GitHub Stats"/>
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Muhammednihalmp&layout=compact&langs_count=8&theme=tokyonight&hide_border=true&bg_color=0D1117&title_color=00F7FF&text_color=FFFFFF" alt="Top Languages"/>
    </div>
    <div class="stats">
      <img src="https://github-readme-streak-stats.herokuapp.com/?user=Muhammednihalmp&theme=tokyonight&hide_border=true&background=0D1117&stroke=00F7FF&ring=00F7FF&fire=FF6B6B&currStreakLabel=00F7FF" alt="Streak"/>
      <img src="https://github-readme-activity-graph.vercel.app/graph?username=Muhammednihalmp&theme=tokyo-night&hide_border=true&bg_color=0D1117&color=00F7FF&line=00F7FF&point=FFFFFF" alt="Activity Graph"/>
    </div>
  </section>

  <section id="learning">
    <h2>🎓 Learning Journey</h2>
    <div class="mermaid">
      <pre>graph LR
    A[Computer Engineering] --> B[Cybersecurity]
    A --> C[IoT Development]
    B --> D[Ethical Hacking]
    B --> E[Hardware Exploitation]
    C --> F[ESP32 Projects]
    C --> G[Automation Bots]
    D --> H[Penetration Testing]
    E --> H
    F --> I[All-in-One Hacking Device]
    G --> I
    H --> I</pre>
    </div>

    <h3>🌱 Currently Mastering</h3>
    <ul style="list-style:none; padding-left:0;">
      <li>🔐 Advanced Penetration Testing Techniques</li>
      <li>🔧 Hardware Reverse Engineering & Exploitation</li>
      <li>🤖 Robotics & Automation Systems</li>
      <li>📡 Wireless Communication Protocols</li>
      <li>🛡️ Network Security Architecture</li>
    </ul>
  </section>

  <section id="goals">
    <h2>🏆 Achievements & Goals</h2>
    <div class="goals">
      <table>
        <tr><td>🎯 Build All-in-One Pentesting Device</td><td class="in-progress">🔄 In Progress</td></tr>
        <tr><td>🎯 Master Hardware Exploitation</td><td class="in-progress">🔄 In Progress</td></tr>
        <tr><td>🎯 Contribute to Security Tools</td><td class="planning">📝 Planning</td></tr>
        <tr><td>🎯 Develop IoT Security Framework</td><td class="planning">📝 Planning</td></tr>
      </table>
    </div>
  </section>

  <section id="philosophy">
    <h2>💡 Philosophy</h2>
    <div class="philosophy">
      "Hacking is not about breaking rules—it's about understanding systems deeply and making them better, more secure, and more innovative."
      <br><br>
      <strong>🛡️ Ethical Hacking Principles:</strong> Knowledge • Responsibility • Innovation • Security
    </div>
  </section>

  <section class="connect">
    <h2>📫 Let's Connect</h2>
    <p>🤝 Open for Collaboration on Cybersecurity, Hardware Hacking, IoT Security & Open Source Tools</p>
    <a href="mailto:muhammadnihalmp955@gmail.com" class="btn">📧 Email Me</a>
    <a href="https://t.me/Muhammed_Nihal_MP" class="btn">💬 Telegram</a>
    <a href="https://www.linkedin.com/in/muhammed-nihal-mp-96a346283/" class="btn">💼 LinkedIn</a>
    <div class="views">🔥 Profile Views: <span id="views">Loading...</span></div>
  </section>

  <footer>
    ⭐ From <a href="https://github.com/Muhammednihalmp" style="color:var(--accent);">Muhammednihalmp</a> | Made with 💙 and ☕
  </footer>

</div>

<script>
  // Matrix Rain Effect
  const canvas = document.getElementById('matrix');
  const ctx = canvas.getContext('2d');
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;

  const matrix = "ABCDEFGHIJKLMNOPQRSTUVWXYZ123456789@#$%^&*()*&^%+-/~{[|`]}";
  const fontSize = 16;
  const columns = canvas.width / fontSize;
  const drops = Array(Math.floor(columns)).fill(1);

  function draw() {
    ctx.fillStyle = 'rgba(13, 17, 23, 0.05)';
    ctx.fillRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = '#00F7FF';
    ctx.font = fontSize + 'px monospace';

    for (let i = 0; i < drops.length; i++) {
      const text = matrix[Math.floor(Math.random() * matrix.length)];
      ctx.fillText(text, i * fontSize, drops[i] * fontSize);
      if (drops[i] * fontSize > canvas.height && Math.random() > 0.975) drops[i] = 0;
      drops[i]++;
    }
  }
  setInterval(draw, 35);

  // Mermaid.js (simple fallback)
  document.querySelectorAll('pre').forEach(pre => {
    if (pre.textContent.includes('graph LR')) {
      pre.innerHTML = '<div style="color:#00F7FF; text-align:center;">[Interactive Mermaid Diagram Placeholder]</div>';
    }
  });

  // Fake view counter
  document.getElementById('views').textContent = Math.floor(Math.random() * 50000) + 10000;
</script>

</body>
</html>
