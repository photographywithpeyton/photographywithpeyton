<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>[Your Name] Photography</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Montserrat', sans-serif;
      line-height: 1.6;
      color: #333;
    }

    /* Navigation */
    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 20px 40px;
      background: #f9f9f9;
      position: sticky;
      top: 0;
      z-index: 100;
      box-shadow: 0 2px 5px rgba(0,0,0,0.05);
    }
    nav a {
      text-decoration: none;
      color: #333;
      margin-left: 20px;
      font-weight: 600;
    }

    /* Hero */
    .hero {
      height: 80vh;
      background: url('hero-photo.jpg') center/cover no-repeat;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 10px;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.5);
    }
    .hero button {
      padding: 15px 30px;
      font-size: 1rem;
      border: none;
      background: #00a99d;
      color: white;
      cursor: pointer;
      font-weight: 700;
      border-radius: 5px;
      transition: background 0.3s;
    }
    .hero button:hover {
      background: #00887a;
    }

    /* Sections */
    section {
      padding: 60px 40px;
    }
    h2 {
      text-align: center;
      margin-bottom: 40px;
      font-size: 2.2rem;
      color: #00a99d;
    }

    /* About */
    .about {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      gap: 40px;
    }
    .about img {
      width: 300px;
      border-radius: 10px;
    }
    .about p {
      flex: 1;
      font-size: 1.1rem;
    }

    /* Portfolio */
    .portfolio {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 20px;
    }
    .portfolio img {
      width: 100%;
      border-radius: 10px;
    }

    /* Pricing */
    .pricing {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 30px;
    }
    .price-card {
      border: 1px solid #ddd;
      padding: 20px;
      border-radius: 10px;
      text-align: center;
      width: 250px;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .price-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 10px 20px rgba(0,0,0,0.1);
    }
    .price-card h3 {
      margin-bottom: 15px;
      color: #00a99d;
    }
    .price-card p {
      margin-bottom: 10px;
    }

    /* Contact */
    .contact form {
      max-width: 500px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }
    .contact input, .contact textarea {
      padding: 10px;
      font-size: 1rem;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
    .contact button {
      padding: 12px;
      border: none;
      background: #00a99d;
      color: white;
      font-weight: 700;
      cursor: pointer;
      border-radius: 5px;
      transition: background 0.3s;
    }
    .contact button:hover {
      background: #00887a;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 30px;
      background: #f9f9f9;
      color: #555;
    }

    @media(max-width: 768px){
      .about {
        flex-direction: column;
      }
      .hero h1 {
        font-size: 2.2rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <nav>
    <div><strong>[Your Name]</strong> Photography</div>
    <div>
      <a href="#about">About</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#pricing">Pricing</a>
      <a href="#contact">Contact</a>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Capturing Moments You’ll Treasure Forever</h1>
    <button onclick="location.href='#contact'">Book Your Session</button>
  </section>

  <!-- About Section -->
  <section id="about">
    <h2>About Me</h2>
    <div class="about">
      <img src="about-photo.jpg" alt="Photographer">
      <p>Hi! I’m [Your Name], a beginner photographer passionate about capturing authentic moments and beautiful memories. My style is natural, creative, and fun. I’d love to work with you and make your special moments last forever.</p>
    </div>
  </section>

  <!-- Portfolio Section -->
  <section id="portfolio">
    <h2>Portfolio</h2>
    <div class="portfolio">
      <img src="photo1.jpg" alt="">
      <img src="photo2.jpg" alt="">
      <img src="photo3.jpg" alt="">
      <img src="photo4.jpg" alt="">
      <img src="photo5.jpg" alt="">
      <img src="photo6.jpg" alt="">
    </div>
  </section>

  <!-- Pricing Section -->
  <section id="pricing">
    <h2>Pricing</h2>
    <div class="pricing">
      <div class="price-card">
        <h3>Mini Session</h3>
        <p>20–30 minutes</p>
        <p>5–10 edited images</p>
        <p><strong>$100</strong></p>
      </div>
      <div class="price-card">
        <h3>Standard Session</h3>
        <p>1–2 hours</p>
        <p>20–30 edited images</p>
        <p><strong>$200</strong></p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Contact Me</h2>
    <div class="contact">
      <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <input type="text" placeholder="Preferred Date">
        <input type="text" placeholder="Location">
        <textarea rows="5" placeholder="Message / Outfit Ideas"></textarea>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    © [Year] [Your Name] Photography | Instagram | Facebook
  </footer>

</body>
</html>
<!--
**photographywithpeyton/photographywithpeyton** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

