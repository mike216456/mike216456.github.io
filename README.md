<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Max Mercury International PMC</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #222;
      --secondary: #bdbdbd;
      --accent: #222;
      --text: #222;
      --muted: #222;
      --white: #bdbdbd;
      --divider: #bdbdbd;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Roboto', sans-serif;
    }
    body {
      background: #bdbdbd;
      color: #222;
      line-height: 1.7;
      margin: 0;
      padding: 0;
    }
    nav {
      width: 100%;
      background: var(--white);
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.04);
      padding: 1.2rem 0;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    .nav-container {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      padding: 0 2rem;
    }
    .nav-logo {
      font-size: 1.5rem;
      font-weight: bold;
      color: var(--primary);
      letter-spacing: 1px;
    }
    .nav-links {
      display: flex;
      gap: 2rem;
    }
    .nav-links a {
      color: var(--muted);
      text-decoration: none;
      font-weight: 500;
      transition: color 0.2s;
    }
    .nav-links a:hover {
      color: var(--accent);
    }
    header {
      background: linear-gradient(rgba(26,39,70,0.7), rgba(26,39,70,0.7)), url('https://images.unsplash.com/photo-1506744038136-46273834b3fb') no-repeat center center/cover;
      color: var(--white);
      padding: 6rem 2rem 5rem 2rem;
      text-align: center;
      position: relative;
    }
    header h1 {
      font-size: 2.8rem;
      font-weight: 700;
      letter-spacing: 1px;
      margin-bottom: 1rem;
    }
    header p {
      font-size: 1.3rem;
      color: #e3e7ed;
      margin-bottom: 0.5rem;
    }
    .section {
      padding: 3.5rem 2rem 3rem 2rem;
      max-width: 900px;
      margin: 0 auto;
      background: var(--white);
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.04);
      margin-top: 3rem;
      margin-bottom: 3rem;
      position: relative;
    }
    .section:not(:first-of-type) {
      border-top: 1px solid var(--divider);
    }
    .section h2 {
      font-size: 2rem;
      color: var(--primary);
      margin-bottom: 1.2rem;
      font-weight: 700;
    }
    .section p, .section ul {
      font-size: 1.08rem;
      margin-bottom: 1.2rem;
      color: var(--text);
    }
    .section ul {
      list-style-type: disc;
      padding-left: 1.5rem;
    }
    .section img {
      width: 100%;
      max-height: 320px;
      object-fit: cover;
      border-radius: 8px;
      margin: 2rem 0 1rem 0;
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.08);
      aspect-ratio: 16/9;
    }
    .contact {
      background: var(--primary);
      color: var(--white);
      padding: 2.5rem 2rem 2rem 2rem;
      border-radius: 10px;
      margin-top: 3rem;
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.08);
    }
    .contact h2 {
      color: var(--white);
      margin-bottom: 1.2rem;
    }
    .contact p {
      font-size: 1.05rem;
      margin-bottom: 1rem;
      color: #e3e7ed;
    }
    .contact strong {
      color: var(--accent);
    }
    .contact-form {
      margin-top: 1.5rem;
      display: flex;
      flex-direction: column;
      gap: 1rem;
      max-width: 400px;
    }
    .contact-form input, .contact-form textarea {
      padding: 0.7rem 1rem;
      border-radius: 5px;
      border: none;
      background: #f0f4fa;
      font-size: 1rem;
      resize: none;
    }
    .contact-form input:focus, .contact-form textarea:focus {
      outline: 2px solid var(--accent);
    }
    .contact-form button {
      background: var(--accent);
      color: var(--white);
      padding: 0.7rem 1.6rem;
      border-radius: 5px;
      font-weight: 600;
      border: none;
      cursor: pointer;
      transition: background 0.2s;
    }
    .contact-form button:hover {
      background: #176fd6;
    }
    .divider {
      width: 100%;
      height: 1px;
      background: var(--divider);
      margin: 3rem 0;
      border: none;
    }
    .btn {
      display: inline-block;
      background: var(--accent);
      color: var(--white);
      padding: 0.7rem 1.6rem;
      border-radius: 5px;
      font-weight: 600;
      text-decoration: none;
      transition: background 0.2s;
      margin-top: 1rem;
      border: none;
      cursor: pointer;
    }
    .btn:hover {
      background: #176fd6;
    }
    footer {
      background: var(--primary);
      color: var(--white);
      text-align: center;
      padding: 2rem 1rem;
      font-size: 1rem;
      letter-spacing: 0.5px;
      margin-top: 2rem;
    }
    .hero-images {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 0;
      background: var(--white);
      padding: 1.5rem 0 0.5rem 0;
      max-width: 1200px;
      margin: 0 auto;
    }
    .hero-images img {
      width: 100%;
      max-width: 1200px;
      aspect-ratio: 16/6;
      object-fit: cover;
      border-radius: 10px;
      box-shadow: 0 2px 12px rgba(26, 39, 70, 0.10);
    }
    .track-record-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 2rem;
      background: transparent;
    }
    .track-record-item {
      background: #e5e5e5;
      border-radius: 8px;
      padding: 1.2rem 1rem 2rem 1rem;
      text-align: center;
      display: flex;
      flex-direction: column;
      align-items: center;
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.04);
    }
    .track-record-num {
      font-size: 1.1rem;
      color: #222;
      font-weight: 400;
      margin-bottom: 0.5rem;
      letter-spacing: 2px;
    }
    .track-record-title {
      font-size: 1.1rem;
      font-weight: 600;
      margin-bottom: 1rem;
      color: #222;
      letter-spacing: 0.5px;
    }
    .track-record-item img {
      width: 100%;
      max-width: 180px;
      aspect-ratio: 1/1;
      object-fit: cover;
      border-radius: 6px;
      margin-bottom: 1rem;
      box-shadow: 0 2px 8px rgba(26, 39, 70, 0.08);
    }
    .track-record-desc {
      font-size: 0.98rem;
      color: #222;
      margin-top: 0.5rem;
    }
    @media (max-width: 1100px) {
      .track-record-grid {
        grid-template-columns: 1fr 1fr;
        gap: 1.5rem;
      }
    }
    @media (max-width: 700px) {
      .track-record-grid {
        grid-template-columns: 1fr;
        gap: 1rem;
      }
      .track-record-item img {
        max-width: 100%;
      }
    }
    @media (max-width: 900px) {
      .hero-images {
        flex-direction: column;
        gap: 1rem;
        padding: 1rem 0 0.5rem 0;
      }
      .hero-images img {
        width: 100%;
      }
    }
    @media (max-width: 700px) {
      .section, .contact {
        padding: 2rem 1rem;
        margin-top: 2rem;
        margin-bottom: 2rem;
      }
      .nav-container {
        flex-direction: column;
        gap: 1rem;
      }
      header {
        padding: 4rem 1rem 3rem 1rem;
      }
      header h1 {
        font-size: 2rem;
      }
    }
    .mission-vision-section {
      background: #bdbdbd;
      padding: 3.5rem 2rem 3rem 2rem;
      max-width: 100vw;
      margin: 0 auto 3rem auto;
      border-radius: 0;
      box-shadow: none;
    }
    .mission-vision-title {
      font-size: 3.2rem;
      font-family: 'Times New Roman', Times, serif;
      font-weight: 400;
      margin-bottom: 2.5rem;
      text-align: left;
      color: #222;
    }
    .mission-vision-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 2.5rem;
      justify-items: center;
      align-items: flex-start;
      background: transparent;
    }
    .mission-vision-item {
      background: none;
      border-radius: 0;
      padding: 0;
      text-align: center;
      box-shadow: none;
      display: flex;
      flex-direction: column;
      align-items: center;
    }
    .mission-vision-subtitle {
      font-size: 1.3rem;
      font-family: 'Times New Roman', Times, serif;
      font-weight: 400;
      margin-bottom: 1.2rem;
      color: #222;
    }
    .mission-vision-item img,
    .track-record-item img {
      width: 340px;
      height: 340px;
      object-fit: cover;
      border-radius: 0;
      margin-bottom: 1.5rem;
      box-shadow: none;
      display: block;
      margin-left: auto;
      margin-right: auto;
    }
    .mission-vision-grid,
    .track-record-grid {
      align-items: start;
      justify-items: center;
    }
    @media (max-width: 1100px) {
      .mission-vision-item img,
      .track-record-item img {
        width: 100%;
        height: auto;
        max-width: 340px;
      }
    }
    .mission-vision-desc {
      font-size: 1.25rem;
      color: #222;
      font-family: 'Times New Roman', Times, serif;
      font-weight: 400;
      margin-top: 0.5rem;
      line-height: 1.4;
    }
    @media (max-width: 1100px) {
      .mission-vision-grid {
        grid-template-columns: 1fr;
        gap: 2rem;
      }
      .mission-vision-item img {
        width: 100%;
        height: auto;
      }
    }
    .about-section {
      background: #bdbdbd;
      padding: 3.5rem 2rem 3rem 2rem;
      max-width: 100vw;
      margin: 0 auto 3rem auto;
      border-radius: 0;
      box-shadow: none;
    }
    .about-grid {
      display: grid;
      grid-template-columns: 1.2fr 1fr;
      gap: 3rem;
      align-items: center;
      background: transparent;
    }
    .about-title {
      font-size: 4rem;
      font-family: 'Times New Roman', Times, serif;
      font-weight: 400;
      margin-bottom: 2.5rem;
      text-align: left;
      color: #222;
    }
    .about-paragraph {
      font-size: 1.25rem;
      color: #222;
      font-family: 'Times New Roman', Times, serif;
      font-weight: 400;
      margin-bottom: 2rem;
      line-height: 1.4;
      text-align: left;
    }
    .about-image img {
      width: 100%;
      max-width: 600px;
      aspect-ratio: 1.5/1;
      object-fit: cover;
      border-radius: 0;
      box-shadow: none;
      display: block;
      margin: 0 auto;
    }
    @media (max-width: 1100px) {
      .about-grid {
        grid-template-columns: 1fr;
        gap: 2rem;
      }
      .about-image img {
        max-width: 100%;
        height: auto;
      }
    }
    nav, .section, .about-section, .mission-vision-section, .contact, .hero-images {
      background: #bdbdbd !important;
      box-shadow: none !important;
      border-radius: 0 !important;
    }
    .track-record-item, .mission-vision-item {
      background: #bdbdbd !important;
      box-shadow: none !important;
    }
    .minimal-nav {
      background: #bdbdbd;
      padding: 0;
      margin: 0;
      width: 100vw;
    }
    .nav-row {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      padding: 1.2rem 2rem 0.5rem 2rem;
    }
    .nav-logo-block {
      display: flex;
      flex-direction: row;
      align-items: flex-start;
      gap: 0.7rem;
    }
    .nav-logo-icon {
      font-size: 1.3rem;
      margin-top: 0.2rem;
    }
    .nav-logo-text {
      font-family: 'Times New Roman', Times, serif;
      font-size: 1.1rem;
      font-weight: 400;
      line-height: 1.1;
    }
    .nav-links-minimal {
      display: flex;
      align-items: center;
      gap: 2.5rem;
      font-size: 1.05rem;
    }
    .nav-links-minimal a {
      color: #222;
      text-decoration: none;
      font-weight: 400;
      font-family: 'Roboto', sans-serif;
      letter-spacing: 0.5px;
    }
    .nav-menu-icon {
      font-size: 1.7rem;
      cursor: pointer;
      margin-left: 1.5rem;
    }
    .nav-divider {
      border: none;
      border-top: 2px solid #222;
      margin: 0 0 0 0;
    }
    .hero-section {
      background: #bdbdbd;
      padding: 0 0 2rem 0;
      margin: 0;
    }
    .hero-content {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      padding: 2.5rem 2rem 1.5rem 2rem;
    }
    .hero-left {
      flex: 1;
    }
    .hero-title {
      font-family: 'Times New Roman', Times, serif;
      font-size: 3.5rem;
      font-weight: 400;
      margin: 0;
      letter-spacing: 1px;
      line-height: 1.1;
    }
    .hero-right {
      flex: 1;
      display: flex;
      flex-direction: column;
      align-items: flex-end;
      justify-content: flex-start;
      gap: 2.5rem;
      margin-top: 0.5rem;
    }
    .hero-subtext {
      font-size: 1rem;
      font-family: 'Roboto', sans-serif;
      color: #222;
      margin-bottom: 2.5rem;
      margin-right: 0.5rem;
    }
    .hero-btn {
      border: 1.5px solid #222;
      background: transparent;
      color: #222;
      font-size: 1rem;
      font-family: 'Roboto', sans-serif;
      padding: 0.6rem 2.2rem;
      border-radius: 0;
      text-decoration: none;
      font-weight: 400;
      transition: background 0.2s, color 0.2s;
      margin-right: 0.5rem;
      letter-spacing: 0.5px;
    }
    .hero-btn:hover {
      background: #222;
      color: #fff;
    }
    .hero-image-row {
      display: flex;
      flex-direction: row;
      gap: 0.5rem;
      width: 100vw;
      margin: 0;
      padding: 0 0 0 0;
      justify-content: center;
      align-items: stretch;
    }
    .hero-img {
      width: 50vw;
      height: 400px;
      object-fit: cover;
      border-radius: 1rem;
      margin: 0;
      display: block;
    }
    @media (max-width: 1100px) {
      .hero-content {
        flex-direction: column;
        gap: 2rem;
      }
      .hero-image-row {
        flex-direction: column;
        gap: 0.5rem;
      }
      .hero-img {
        width: 100vw;
        height: 250px;
      }
    }
  </style>
</head>
<body>
  <nav class="minimal-nav">
    <div class="nav-row">
      <div class="nav-logo-block">
        <span class="nav-logo-icon">&#9632;</span>
        <span class="nav-logo-text">Max Mercury<br>International PMC</span>
      </div>
      <div class="nav-links-minimal">
        <a href="#contact">Contact</a>
        <span class="nav-menu-icon">&#9776;</span>
      </div>
    </div>
    <hr class="nav-divider" />
  </nav>
  <section class="hero-section">
    <div class="hero-content">
      <div class="hero-left">
        <h1 class="hero-title">EXPERT<br>GUIDANCE</h1>
      </div>
      <div class="hero-right">
        <div class="hero-subtext">Dedicated to project success worldwide.</div>
        <a class="hero-btn" href="#about">Learn More</a>
      </div>
    </div>
    <div class="hero-image-row">
      <img src="hero1.jpg" alt="Modern building at sunset" class="hero-img" />
      <img src="hero2.jpg" alt="Upward view of skyscraper" class="hero-img" />
    </div>
  </section>
  <div class="section about-section" id="about">
    <div class="about-grid">
      <div class="about-text">
        <h2 class="about-title">About us</h2>
        <p class="about-paragraph">At Max Mercury International PMC, our vision is to shape the future of infrastructure by delivering end-to-end project solutions that elevate communities and industries alike.<br>
        We strive to be the partner of choice across the GCC, Europe, Asia, and Africa — known for our integrity, precision, and commitment to turning client ideas into impactful realities.</p>
        <p class="about-paragraph">From concept to completion, we specialize in crafting environments that inspire — including swimming pools, sports tracks, gyms, play areas, and more.<br>
        With decades of proven experience, we approach every project with innovation, excellence, and the determination to exceed expectations.</p>
      </div>
      <div class="about-image">
        <img src="about-blueprint.jpg" alt="Detailed blueprints and drawing tools" />
      </div>
    </div>
  </div>
  <div class="section mission-vision-section" id="mission-vision">
    <h2 class="mission-vision-title">Mission & Vision</h2>
    <div class="mission-vision-grid">
      <div class="mission-vision-item">
        <div class="mission-vision-subtitle">Our Mission</div>
        <img src="mission.jpg" alt="Consultant on construction site with plans" />
        <div class="mission-vision-desc">We deliver smart consultancy solutions that shape purposeful infrastructure from recreation areas to public sector projects.</div>
      </div>
      <div class="mission-vision-item">
        <div class="mission-vision-subtitle">Our Goal</div>
        <img src="goal.jpg" alt="Aerial view of sports complex and city" />
        <div class="mission-vision-desc">To be the most trusted project management consultancy in the GCC and beyond, known for innovation and results.</div>
      </div>
      <div class="mission-vision-item">
        <div class="mission-vision-subtitle">Why Choose us</div>
        <img src="why.jpg" alt="Team of consultants reviewing blueprints" />
        <div class="mission-vision-desc">Led by Charles Almeida and backed by 30+ years of experience, we bring bold visions to life with precision and care.</div>
      </div>
    </div>
  </div>
  <div class="section" id="track-record">
    <h2 style="text-align:center; font-size:2.2rem; font-weight:400; margin-bottom:2.5rem;">Our Proven Track Record</h2>
    <div class="track-record-grid">
      <div class="track-record-item">
        <div class="track-record-num">01</div>
        <div class="track-record-title">Precision Delivered</div>
        <img src="precision.jpg" alt="Luxury residential swimming pool under construction" />
        <div class="track-record-desc">Our expertly executed swimming pool installations reflect our commitment to precision, safety, and aesthetic excellence.</div>
      </div>
      <div class="track-record-item">
        <div class="track-record-num">02</div>
        <div class="track-record-title">Transformative Outcomes</div>
        <img src="transformative.jpg" alt="Modern public park with play area and palm trees" />
        <div class="track-record-desc">We've transformed community spaces and government facilities with custom outdoor gym and kids play area solutions that promote wellness and engagement.</div>
      </div>
      <div class="track-record-item">
        <div class="track-record-num">03</div>
        <div class="track-record-title">Innovative Solutions</div>
        <img src="innovative.jpg" alt="3D architectural model of hotel courtyard landscape" />
        <div class="track-record-desc">Our innovative landscape designs and outdoor fitness spaces have redefined user experience in both hospitality and residential environments.</div>
      </div>
      <div class="track-record-item">
        <div class="track-record-num">04</div>
        <div class="track-record-title">Proven Success</div>
        <img src="success.jpg" alt="Modern indoor gym with climbing wall and equipment" />
        <div class="track-record-desc">From indoor gym equipment to modern play zones, our work in educational institutions has delivered lasting value through smart, scalable project management.</div>
      </div>
    </div>
  </div>
  <div class="section contact" id="contact">
    <h2>Contact Us</h2>
    <p>We’d love to hear from you. Whether you're exploring a new project or need expert insights — our team is here to support your goals.</p>
    <form class="contact-form" action="mailto:charles@maxmercurypmc.com" method="POST" enctype="text/plain">
      <input type="text" name="name" placeholder="Your Name" required />
      <input type="email" name="email" placeholder="Your Email" required />
      <textarea name="message" rows="4" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
    <p style="margin-top:1.5rem;">Or reach us directly:<br>
      Email: <strong>charles@maxmercurypmc.com</strong><br>
      Phone: <strong>+971 55 996 8803</strong>
    </p>
  </div>
  <footer>
    <p>&copy; 2025 Max Mercury International PMC. All rights reserved.</p>
  </footer>
</body>
</html> 
