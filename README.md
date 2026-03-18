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
 
    /* ── Name ── */
    h1 {
      font-size: 1.6rem;
      font-weight: 500;
      margin-bottom: 4px;
    }
 
    .role {
      color: #888;
      font-style: italic;
      margin-bottom: 32px;
    }
 
    /* ── Bio ── */
    .bio {
      margin-bottom: 48px;
      color: #444;
    }
 
    /* ── Sections ── */
    section { margin-bottom: 40px; }
 
    h2 {
      font-size: 0.75rem;
      letter-spacing: 0.12em;
      text-transform: uppercase;
      color: #aaa;
      margin-bottom: 12px;
    }
 
    ul { list-style: none; }
    li { color: #1a1a1a; margin-bottom: 6px; }
 
    /* ── Links ── */
    .links { display: flex; flex-direction: column; gap: 8px; }
 
    .links a {
      color: #1a1a1a;
      text-decoration: none;
      width: fit-content;
    }
    .links a:hover { text-decoration: underline; }
  </style>
</head>
<body>

  <!-- Replace src with your actual photo path, e.g. src="photo.jpg" -->
  <img class="photo" src="IMG_2493 2.jpg" alt="Navin Kadel" onerror="this.style.background='#d8d3cc'; this.removeAttribute('src')" />

  <h1>Navin Kadel</h1>
  <p class="role">Neurobiology, UC San Diego &middot; D1 Athlete</p>

  <p class="bio">
    Undergrad studying neurobiology at UC San Diego. I compete as a D1 track athlete and am interested in the science of human performance.
  </p>
  <section>
    <h2>Academics</h2>
    <ul>
      <li>Relevant Courses: human physiology, linear algebra, probability & statistics</li>
      <li>cum. gpa: 4.0</li>
      
    </ul>
  </section>
  

  <section>
    <h2>Athletics</h2>
    <ul>
      <li>Big West Conference Qualifier</li>
      
    </ul>
  </section>

  <section>
    <h2>Links</h2>
    <div class="links">
      <a href="mailto:nkadel@ucsd.edu">nkadel@ucsd.edu</a>
      <a href="https://www.linkedin.com/in/navin-kadel-85a897292/" target="_blank">LinkedIn</a>
      <a href="https://www.instagram.com/navin.kadel" target="_blank">Instagram</a>
    </div>
  </section>

</body>
</html>
