<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Fitness Froth</title>
  <style>
    /* Reset and base styles */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }
    body {
      line-height: 1.6;
      background: #f5f9fc;
      color: #333;
    }
    header {
      background: #2f80ed;
      color: #fff;
      padding: 1em 2em;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 10;
    }
    header .logo {
      font-size: 1.5rem;
      font-weight: bold;
      letter-spacing: 2px;
    }
    nav a {
      color: #fff;
      text-decoration: none;
      margin-left: 1.5em;
      font-weight: 600;
      transition: color 0.3s ease;
    }
    nav a:hover {
      color: #fbc531;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1598970434795-0c54fe7c0642?auto=format&fit=crop&w=1400&q=80') no-repeat center center/cover;
      height: 80vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      color: white;
      text-align: center;
      padding: 0 1em;
    }
    .hero h1 {
      font-size: 3rem;
      margin-bottom: 0.5em;
      text-shadow: 2px 2px 8px #000;
    }
    .hero p {
      font-size: 1.25rem;
      margin-bottom: 1.5em;
      max-width: 600px;
      text-shadow: 1px 1px 6px #000;
    }
    .btn {
      background: #fbc531;
      color: #222;
      padding: 0.75em 2em;
      font-weight: bold;
      border: none;
      border-radius: 50px;
      cursor: pointer;
      transition: background 0.3s ease;
      text-decoration: none;
    }
    .btn:hover {
      background: #e1aa26;
    }
    main {
      max-width: 1200px;
      margin: 2em auto;
      padding: 0 1em;
    }
    section {
      margin-bottom: 4em;
    }
    section h2 {
      text-align: center;
      font-size: 2rem;
      margin-bottom: 1em;
      color: #2f80ed;
    }
    .about, .workouts, .nutrition, .testimonials, .contact {
      background: white;
      padding: 2em;
      border-radius: 10px;
      box-shadow: 0 8px 16px rgba(47, 128, 237, 0.1);
    }
    .about p, .nutrition p, .contact p {
      max-width: 700px;
      margin: 0 auto 1em;
      font-size: 1rem;
      color: #555;
      line-height: 1.6;
    }
    .workouts-list, .testimonials-list {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1.5em;
    }
    .workout, .testimonial {
      background: #f5f9fc;
      padding: 1em;
      border-radius: 8px;
      box-shadow: 0 4px 8px rgba(47, 128, 237, 0.1);
      width: 280px;
      text-align: center;
    }
    .workout h3, .testimonial h3 {
      margin-bottom: 0.5em;
      color: #2f80ed;
    }
    .testimonial p {
      font-style: italic;
      color: #666;
    }
    form {
      max-width: 700px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
    }
    label {
      margin-bottom: 0.5em;
      font-weight: 600;
      color: #2f80ed;
    }
    input, textarea {
      padding: 0.75em;
      margin-bottom: 1.5em;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 1rem;
      resize: vertical;
    }
    button[type="submit"] {
      background: #2f80ed;
      color: white;
      border: none;
      padding: 1em;
      border-radius: 50px;
      font-weight: bold;
      cursor: pointer;
      transition: background 0.3s ease;
    }
    button[type="submit"]:hover {
      background: #1c5ad6;
    }
    footer {
      text-align: center;
      padding: 1.5em;
      background: #2f80ed;
      color: white;
      font-size: 0.9rem;
    }
    @media (max-width: 768px) {
      nav a {
        margin-left: 1em;
      }
      .workouts-list, .testimonials-list {
        flex-direction: column;
        align-items: center;
      }
      .workout, .testimonial {
        width: 90%;
      }
      .hero h1 {
        font-size: 2.2rem;
      }
      .hero p {
        font-size: 1rem;
      }
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">Fitness Froth</div>
    <nav>
      <a href="#about">About</a>
      <a href="#workouts">Workouts</a>
      <a href="#nutrition">Nutrition</a>
      <a href="#testimonials">Testimonials</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>
  <section class="hero">
    <h1>Fuel Your Fitness Journey</h1>
    <p>Discover workouts, nutrition tips, and community support to help you thrive.</p>
    <a href="#workouts" class="btn">Get Started</a>
  </section>
  <main>
    <section id="about" class="about">
      <h2>About Fitness Froth</h2>
      <p>Fitness Froth is dedicated to empowering individuals to live healthier, stronger lives through expert workout plans, nutrition guidance, and supportive community resources.</p>
    </section>
    <section id="workouts" class="workouts">
      <h2>Workout Plans</h2>
      <div class="workouts-list">
        <article class="workout">
          <h3>Full Body Blast</h3>
          <p>A 30-minute high-intensity workout to strengthen and tone your entire body.</p>
        </article>
        <article class="workout">
          <h3>Yoga Flow</h3>
          <p>Relax and energize with this gentle and flexible yoga routine.</p>
        </article>
        <article class="workout">
          <h3>Cardio Burn</h3>
          <p>Get your heart rate up with this intense cardio circuit workout.</p>
        </article>
      </div>
    </section>
    <section id="nutrition" class="nutrition">
      <h2>Nutrition Tips</h2>
      <p>Proper nutrition is the foundation of fitness. Check out our guides to eating healthy, meal prepping, and staying hydrated.</p>
    </section>
    <section id="testimonials" class="testimonials">
      <h2>What Our Members Say</h2>
      <div class="testimonials-list">
        <article class="testimonial">
          <h3>Jane D.</h3>
          <p>"Fitness Froth transformed my life. The workouts are easy to follow and really effective."</p>
        </article>
        <article class="testimonial">
          <h3>Mark S.</h3>
          <p>"Love the nutrition advice here – easy to incorporate into my daily routine!"</p>
        </article>
      </div>
    </section>
    <section id="contact" class="contact">
      <h2>Contact Us</h2>
      <form>
        <label for="name">Name</label>
        <input id="name" type="text" placeholder="Your name" required />
        <label for="email">Email</label>
        <input id="email" type="email" placeholder="Your email" required />
        <label for="message">Message</label>
        <textarea id="message" rows="5" placeholder="Write your message here" required></textarea>
        <button type="submit">Send Message</button>
      </form>
    </section>
  </main>
  <footer>
    &copy; 2025 Fitness Froth. All rights reserved.
  </footer>
</body>
</html>
Fitness froth 
https://images.unsplash.com/photo-1598970434795-0c54fe7c0642?auto=format&fit=crop&w=1400&q=80
