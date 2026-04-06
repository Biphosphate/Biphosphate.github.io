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
      margin-bottom: 20px;
      background: #d8d3cc;
    }

    /* ── Header ── */
    .bio { color: #444; margin-bottom: 12px; }

    /* ── Header links ── */
    .header-links { display: flex; gap: 8px; align-items: center; margin-bottom: 40px; }
    .header-links a { color: #1a1a1a; text-decoration: none; font-size: 0.95rem; }
    .header-links a:hover { text-decoration: underline; }
    .header-links span { color: #aaa; }

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
    nav {
    display: flex;
    gap: 24px;
    margin-bottom: 40px;
    border-bottom: 1px solid #ddd;
    overflow-x: auto;
      -webkit-overflow-scrolling: touch;
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
    .links { display: flex; flex-direction: row; gap: 8px; margin-top: 8px; }
    .links a { color: #4a7fa5; text-decoration: underline; width: fit-content; }
    .links a:hover { text-decoration: underline; }
  </style>
</head>
<body>

  <img class="photo" src="IMG_2493 2.jpg" alt="Navin Kadel" onerror="this.style.background='#d8d3cc'; this.removeAttribute('src')" />

  <p class="bio">
    I am a first-year neurobiology undergraduate at UC San Diego interested in translational neuroscience.
  </p>

  <div class="header-links">
    <a href="mailto:nkadel@ucsd.edu">email</a>
    <span>/</span>
    <a href="https://www.linkedin.com/in/navin-kadel-85a897292/" target="_blank">linkedin</a>
    <span>/</span>
    <a href="cv.pdf" target="_blank" rel="noopener noreferrer">cv</a>
  </div>

  <nav>
    <button class="active" onclick="showTab(event, 'academics')">academics</button>
    <button onclick="showTab(event, 'athletics')">athletics</button>
    <button onclick="showTab(event, 'projects')">projects</button>
    <button onclick="showTab(event, 'misc')">misc</button>
  </nav>

  <div id="academics" class="tab active">
    <p class="content">relevant courses: human physiology, linear algebra, probability &amp; statistics, calculus, general chemistry</p>
    <p class="content">cumulative gpa: 4.0</p>
  </div>

  <div id="athletics" class="tab">
    <ul>
      <li>NCAA Division 1 Cross Country, Track &amp; Field Athlete</li>
      <li>Top 20 California Senior in the mile (4:11)</li>
      <li>CIF XC State Champion</li>
    </ul>
  </div>


  <div id="projects" class="tab">
    <p class="content">
      I competed in a brain computer interface hackathon and worked in a team of four doing data science/statistical tests. The dataset we chose was a linear prediction of simultaneous and independent movements of two finger groups using an intracortical brain-machine interface (Utah Array), which is basically predicting the way a rhesus macaque would move its fingers based only on neuron spiking. Our project specifically focused on reducing neural dimensionality by selectively removing low-correlation channels while maintaining decoder performance (measured by R², the proportion of variance in finger velocity explained by spiking activity in our regression model).</p>
    <img src="bciiiii.jpg" alt="BCI figures" style="width: 80%; margin-top: 24px; border-radius: 4px;" />
  </div>

  <div id="misc" class="tab">
    <p class="content">Inspired by 2D cross-sectioning that MRI machines do, I thought it would be interesting to create a 3D structure of basic neuroanatomy using a similar method. I cut out 12 uniquely shaped cardboard slices and painted both sides of each with their corresponding brain region, then connected the slices with three 1x1 lego studs hot-glued to each side.</p>
    <img src="IMG_0027_2.jpg" alt="Brain model" style="width: 80%; margin-top: 24px; border-radius: 4px;" />
    <img src="IMG_0028.jpg" alt="Brain model" style="width: 80%; margin-top: 24px; border-radius: 4px;" />
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
