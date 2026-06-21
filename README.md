<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Tomiwa Akinlolu — Student Profile</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;700&family=Source+Serif+4:ital,opsz,wght@0,8..60,400;1,8..60,500&display=swap');

  :root{
    --chalk: #F3EFE3;
    --slate: #1F2B26;
    --ochre: #D98E3B;
    --moss: #6E8C73;
    --paper-line: rgba(243,239,227,0.08);
  }

  *{ box-sizing:border-box; margin:0; padding:0; }

  html,body{
    background: var(--slate);
    color: var(--chalk);
    font-family: 'Source Serif 4', serif;
    min-height:100vh;
  }

  .bg{
    position:fixed; inset:0; z-index:-1;
    background:
      repeating-linear-gradient(0deg, var(--paper-line) 0 1px, transparent 1px 38px),
      radial-gradient(circle at 18% 20%, rgba(217,142,59,0.10), transparent 40%),
      radial-gradient(circle at 85% 75%, rgba(110,140,115,0.14), transparent 45%),
      linear-gradient(160deg, #1F2B26 0%, #233129 55%, #1A2420 100%);
  }

  header{
    padding: 4rem 1.5rem 2rem;
    text-align:center;
  }

  h1{
    font-family:'Space Grotesk', sans-serif;
    font-weight:700;
    font-size: clamp(2.2rem, 5.5vw, 3.6rem);
    color: var(--ochre);
    text-transform: uppercase;
    letter-spacing: 0.04em;
    display:inline-block;
    border-bottom: 3px solid var(--moss);
    padding-bottom: 0.6rem;
  }

  .eyebrow{
    font-family:'Space Grotesk', sans-serif;
    letter-spacing:0.25em; text-transform:uppercase;
    font-size:0.72rem; color: var(--moss);
    margin-bottom:1.2rem;
  }

  main{
    max-width: 760px;
    margin: 0 auto;
    padding: 1rem 1.5rem 5rem;
  }

  section{
    background: rgba(243,239,227,0.04);
    border: 1px solid rgba(243,239,227,0.1);
    border-radius: 4px;
    padding: 2rem;
    margin-bottom: 2rem;
  }

  section h2{
    font-family:'Space Grotesk', sans-serif;
    font-size: 1.3rem;
    color: var(--chalk);
    margin-bottom: 1rem;
    border-left: 4px solid var(--ochre);
    padding-left: 0.7rem;
  }

  p{
    line-height: 1.7;
    color: rgba(243,239,227,0.85);
    margin-bottom: 0.8rem;
  }

  ul{
    list-style: none;
    margin-bottom: 0.8rem;
  }

  ul li{
    line-height: 1.7;
    color: rgba(243,239,227,0.85);
  }

  ul li strong{
    color: var(--chalk);
    font-family:'Space Grotesk', sans-serif;
    font-weight:500;
  }

  #send-btn{
    margin-top: 0.5rem;
    display:inline-flex;
    align-items:center;
    gap:0.7rem;
    padding: 0.95rem 2.1rem;
    background: var(--ochre);
    color: #fff;
    font-family:'Space Grotesk', sans-serif;
    font-weight:700;
    font-size:1rem;
    letter-spacing:0.02em;
    text-decoration:none;
    border-radius: 4px;
    border: 1px solid transparent;
    transition: transform 0.18s ease;
  }

  #send-btn:hover{ transform: translateY(-2px); }

  #send-btn:focus-visible{
    outline: 2px solid var(--chalk);
    outline-offset: 3px;
  }

  #send-btn svg{ width:18px; height:18px; flex-shrink:0; }

  footer{
    text-align:center;
    padding: 1.6rem;
    font-family:'Space Grotesk', sans-serif;
    font-size:0.72rem;
    letter-spacing:0.08em;
    color: rgba(243,239,227,0.45);
  }
</style>
</head>
<body>

<div class="bg" aria-hidden="true"></div>

<header>
  <div class="eyebrow">University of Jos &middot; Plateau State</div>
  <h1>Tomiwa Akinlolu</h1>
</header>

<main>

  <section id="about">
    <h2>About Me</h2>
    <ul>
      <li><strong>Full Name:</strong> Tomiwa Akinlolu</li>
      <li><strong>Department:</strong> Computer Science</li>
      <li><strong>Matriculation Number:</strong> UJ/2024/NS/0905</li>
      <li><strong>Level:</strong> 200 Level</li>
    </ul>
    <p>Beyond coursework, I build full-stack web applications, run a content brand called Comic Guru, and have a strong interest in trading, forex markets, and theology. I spend most of my development time in VS Code, working across React, Express, and MongoDB.</p>
  </section>

  <section id="page-info">
    <h2>About This Page</h2>
    <p>This page was created as part of an assessment for a Computer Science course at the University of Jos, focused on Human-Computer Interaction and front-end web fundamentals. It demonstrates a valid HTML5 structure, semantic sectioning, basic styling, and a working contact mechanism using a <code>mailto:</code> link.</p>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p>Have a question about this page or want to reach me directly? Send an email below.</p>
    <a id="send-btn" href="mailto:2024ns0905@unijos.edu.ng?subject=Hello%20Tomiwa">
      <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="5" width="18" height="14" rx="2"/><path d="M3 7l9 6 9-6"/></svg>
      Send Email
    </a>
  </section>

</main>

<footer>2024NS0905@UNIJOS.EDU.NG</footer>

<script>
        /* -------------------------------------------------------
           Matric-number → button colour
           Replace the matric value below with your own number.
           ------------------------------------------------------- */
        const matric = "UJ/2024/NS/0905"; // <-- CHANGE THIS TO YOUR MAT. NO.

	/* CHANGE NOTHING BEYOND THIS POINT - CHANGE NOTHING BEYOND THIS POINT */ 

        function hashString(str) {
            let hash = 0;
            for (let i = 0; i < str.length; i++) {
                hash = (hash * 31 + str.charCodeAt(i)) >>> 0;
            }
            return hash;
        }

        // Normalise input
        const normalised = matric.trim().toUpperCase();

        // Map the hash to a hue value between 0 and 359 degrees
        const hue = hashString(normalised) % 360;

        // Build an HSL colour: fixed saturation & lightness, varying hue
        const buttonColour = `hsl(${hue}, 65%, 45%)`;

        // Apply the colour to the Send Email button
        document.getElementById("send-btn").style.background = buttonColour;
    </script>

</body>
</html>
