<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Animated Business Website</title>
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      line-height: 1.6;
      background: #fff;
      color: #333;
      overflow-x: hidden;
    }

    header {
      background: linear-gradient(to right, #141e30, #243b55);
      color: #fff;
      padding: 1.5rem;
      text-align: center;
      animation: slideDown 1s ease-in-out;
    }

    nav a {
      color: #fff;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
      transition: color 0.3s;
    }

    nav a:hover {
      color: #00ffcc;
    }

    #hero {
      padding: 3rem;
      text-align: center;
      background: #f0f0f0;
      animation: fadeIn 2s ease-in-out;
    }

    #hero .btn {
      background: #333;
      color: #fff;
      padding: 0.7rem 1.2rem;
      text-decoration: none;
      display: inline-block;
      margin-top: 1rem;
      border-radius: 10px;
      transition: transform 0.3s;
    }

    #hero .btn:hover {
      transform: scale(1.1);
      background-color: #222;
    }

    section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
      animation: fadeInUp 1s ease forwards;
    }

    h2 {
      text-align: center;
      margin-bottom: 1rem;
    }

    .service {
      background: #fff;
      padding: 1rem;
      margin: 1rem 0;
      border-left: 5px solid #00bcd4;
      display: flex;
      align-items: center;
      gap: 1rem;
      box-shadow: 0 4px 6px rgba(0,0,0,0.1);
      transition: transform 0.3s;
    }

    .service:hover {
      transform: translateY(-5px);
    }

    .service i {
      font-size: 2rem;
      color: #00bcd4;
      transform: rotateY(0deg);
      transition: transform 0.6s;
    }

    .service:hover i {
      transform: rotateY(180deg);
    }

    form {
      display: flex;
      flex-direction: column;
    }

    input, textarea {
      padding: 0.5rem;
      margin: 0.5rem 0;
      width: 100%;
      border-radius: 5px;
      border: 1px solid #ccc;
    }

    button {
      background: #333;
      color: #fff;
      padding: 0.7rem;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      transition: background 0.3s;
    }

    button:hover {
      background: #555;
    }

    footer {
      background: #222;
      color: #fff;
      text-align: center;
      padding: 1rem;
      animation: slideUp 1s ease-in-out;
    }

    /* Animations */
    @keyframes fadeIn {
      0% {opacity: 0;}
      100% {opacity: 1;}
    }

    @keyframes fadeInUp {
      0% {opacity: 0; transform: translateY(20px);}
      100% {opacity: 1; transform: translateY(0);}
    }

    @keyframes slideDown {
      from { transform: translateY(-100%); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    @keyframes slideUp {
      from { transform: translateY(100%); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Your Company</h1>
    <nav>
      <a href="#services">Services</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <section id="hero">
    <h2>We Build Beautiful Websites</h2>
    <p>Modern, responsive, and SEO-friendly</p>
    <a href="#contact" class="btn">Get Started</a>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <div class="service">
      <i class="fas fa-laptop-code"></i>
      <div>
        <h3>Web Design</h3>
        <p>Custom design to fit your brand.</p>
      </div>
    </div>
    <div class="service">
      <i class="fas fa-chart-line"></i>
      <div>
        <h3>SEO Optimization</h3>
        <p>Rank higher and attract traffic organically.</p>
      </div>
    </div>
    <div class="service">
      <i class="fas fa-tools"></i>
      <div>
        <h3>Website Maintenance</h3>
        <p>Keep your site updated, secure, and fast.</p>
      </div>
    </div>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>We are a team of creative professionals helping businesses succeed online with modern design, smart marketing, and reliable service. Let’s build your digital future.</p>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" rows="4"></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>© 2025 Your Company. All rights reserved.</p>
  </footer>
</body>
</html>
