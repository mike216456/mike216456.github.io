<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Max Mercury International PMC</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary: #1a2746;
      --secondary: #f5f7fa;
      --accent: #1e90ff;
      --text: #222;
      --muted: #6c7a89;
      --white: #fff;
      --divider: #e3e7ed;
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Roboto', sans-serif;
    }
    body {
      background: var(--secondary);
      color: var(--text);
      line-height: 1.7;
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
  </style>
</head>
<body>
  <nav>
    <div class="nav-container">
      <div class="nav-logo">Max Mercury PMC</div>
      <div class="nav-links">
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#why">Why Us</a>
        <a href="#mission">Mission</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </nav>
  <header>
    <h1>Max Mercury International PMC</h1>
    <p>Precision. Integrity. Results — Your Partner in Project Excellence.</p>
  </header>
  <div class="section" id="about">
    <h2>About Us</h2>
    <p>Max Mercury International PMC is a UAE-based project management and consultancy firm with international reach — operating throughout the GCC, Europe, Asia, and Africa. Led by Charles Almeida, a highly regarded industry expert with over 25 years of hands-on experience, we specialize in transforming visions into realities.</p>
    <p>Our team brings over 30 years of collective field experience and goes above and beyond to exceed client expectations. Whether it's civil infrastructure, recreational design, or urban development — we manage every detail with professionalism and precision.</p>
    <img src="https://images.unsplash.com/photo-1503387762-592deb58ef4e" alt="Project planning image">
  </div>
  <div class="section" id="services">
    <h2>Our Services</h2>
    <p>We deliver expert consultancy and turnkey project management services across a wide range of sectors:</p>
    <ul>
      <li>Custom Swimming Pool Design & Build</li>
      <li>Professional Sports Track Planning</li>
      <li>Full-Scale Landscaping Projects</li>
      <li>Indoor Gym Layouts & Equipment Supply</li>
      <li>Safe & Durable Kids’ Play Areas</li>
      <li>Outdoor Fitness & Wellness Installations</li>
    </ul>
    <img src="https://images.unsplash.com/photo-1581092914980-bd2eeda59d20" alt="Landscaping project">
  </div>
  <div class="section" id="why">
    <h2>Why Choose Us</h2>
    <p>With a passion for delivering excellence, Max Mercury International PMC stands out as the go-to partner for public and private sector projects. We prioritize clear communication, innovative design, sustainable practices, and cost-effective execution.</p>
    <p>Our consultants understand the local and international landscape, making us uniquely positioned to guide complex projects from concept to completion.</p>
    <img src="https://images.unsplash.com/photo-1600294037681-c80b4cb5d0c2" alt="Construction management">
  </div>
  <div class="section" id="mission">
    <h2>Our Mission</h2>
    <p>To deliver exceptional consulting and project management services rooted in integrity, innovation, and client satisfaction. We aim to set the standard for excellence in every environment we build and every relationship we maintain.</p>
    <div class="divider"></div>
    <h2>Vision Statement</h2>
    <p>To be a globally respected leader in project consulting and management — shaping spaces that enhance communities and inspire progress.</p>
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
