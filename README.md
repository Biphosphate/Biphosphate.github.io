
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Navin Kadel</title>
  <link href="https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;1,400&display=swap" rel="stylesheet" />
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      background: #f5f2ee;
      color: #1a1a1a;
      font-family: "EB Garamond", Georgia, serif;
      font-size: 1.1rem;
      line-height: 1.7;
      padding: 80px 24px 120px;
      max-width: 600px;
      margin: auto;
    }

    /* ── Photo ── */
    .photo {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      display: block;
      margin-bottom: 32px;
      background: #d8d3cc;
    }

    /* ── Header ── */
    .role {
      color: #888;
      font-style: italic;
      margin-bottom: 16px;
    }

    .bio { color: #444; margin-bottom: 40px; }

    /* ── Header links ── */
    .header-links { display: flex; gap: 20px; margin-bottom: 48px; }
    .header-links a { color: #1a1a1a; text-decoration: none; font-size: 0.95rem; }
    .header-links a:hover { text-decoration: underline; }

    /* ── Tabs ── */
    nav {
      display: flex;
      gap: 24px;
      margin-bottom: 40px;
      border-bottom: 1px solid #ddd;
    }

    nav button {
      background: none;
      border: none;
      font-family: inherit;
      font-size: 0.75rem;
      letter-spacing: 0.1em;
      text-transform: uppercase;
      color: #aaa;
      cursor: pointer;
      padding-bottom: 10px;
      border-bottom: 2px solid transparent;
      margin-bottom: -1px;
      transition: color 0.15s;
    }

    nav button:hover { color: #555; }
    nav button.active { color: #1a1a1a; border-bottom: 2px solid #1a1a1a; }

    /* ── Tab panels ── */
    .tab { display: none; }
    .tab.active { display: block; }

    ul { list-style: none; }
    li { color: #1a1a1a; margin-bottom: 8px; }

    p.content { color: #444; margin-bottom: 12px; }

    /* ── Links inside tabs ── */
    .links { display: flex; flex-direction: column; gap: 8px; margin-top: 8px; }
    .links a { color: #1a1a1a; text-decoration: none; width: fit-content; }
    .links a:hover { text-decoration: underline; }
  </style>
</head>
<body>

  <img class="photo" src="IMG_4638.JPG" alt="Navin Kadel" onerror="this.style.background='#d8d3cc'; this.removeAttribute('src')" />

  <p class="role">Neurobiology, UC San Diego &middot; D1 Athlete</p>

  <p class="bio">
    I am a first-year undergraduate studying neurobiology at UC San Diego.<br>
    Interested in translational neuroscience and running fast.
  </p>

  <div class="header-links">
    <a href="mailto:nkadel@ucsd.edu">email</a>
  </div>

  <nav>
    <button class="active" onclick="showTab(event, 'academics')">academics</button>
    <button onclick="showTab(event, 'athletics')">athletics</button>
    <button onclick="showTab(event, 'research')">research</button>
    <button onclick="showTab(event, 'misc')">misc</button>
    <button onclick="showTab(event, 'connect')">connect</button>
  </nav>

  <div id="academics" class="tab active">
    <p class="content">Relevant courses: human physiology, linear algebra, probability &amp; statistics, calculus, general chemistry</p>
    <p class="content">Cum. GPA: 4.0</p>
  </div>

  <div id="athletics" class="tab">
    <ul>
      <li>2024 CIF XC State Champion</li>
      <li>Top 20 California Senior in the mile</li>
      <li>NCAA Division 1 Cross Country, Track &amp; Field Athlete</li>
      <li>Big West Conference Qualifier</li>
    </ul>
  </div>

  <div id="research" class="tab">
    <p class="content">to be added soon...</p>
  </div>

  <div id="misc" class="tab">
    <p class="content">brain slice</p>
  </div>

  <div id="connect" class="tab">
    <p class="content">I am open to connect if you find anything here interesting.</p>
    <div class="links">
      <a href="mailto:nkadel@ucsd.edu">nkadel@ucsd.edu</a>
      <a href="https://www.linkedin.com/in/navin-kadel-85a897292/" target="_blank">LinkedIn</a>
      <a href="https://www.instagram.com/navin.kadel" target="_blank">Instagram</a>
    </div>
  </div>

  <script>
    function showTab(event, id) {
      document.querySelectorAll('.tab').forEach(t => t.classList.remove('active'));
      document.querySelectorAll('nav button').forEach(b => b.classList.remove('active'));
      document.getElementById(id).classList.add('active');
      event.target.classList.add('active');
    }
  </script>

</body>
</html>
