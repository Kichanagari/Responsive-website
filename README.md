# index.html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Nikhil | Portfolio</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>

  <!-- Navigation -->
  <nav class="navbar">
    <div class="container">
      <div class="logo">Nikhil</div>
      <ul class="nav-links">
        <li><a href="#hero">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hero Section -->
  <section id="hero" class="hero">
    <h1>Hello, I'm Nikhil</h1>
    <p>Full Stack Developer passionate about building modern web experiences.</p>
    <a href="#projects" class="btn">View Projects</a>
  </section>

  <!-- About Section -->
  <section id="about" class="section">
    <div class="container">
      <h2>About Me</h2>
      <p>I’m a self-taught developer from a mechanical engineering background. I create responsive websites using HTML, CSS, JavaScript, and Bootstrap.</p>
    </div>
  </section>

  <!-- Projects Section -->
  <section id="projects" class="section bg-light">
    <div class="container">
      <h2>Projects</h2>
      <div class="project-grid">
        <div class="project-card">
          <h3>Portfolio Website</h3>
          <p>Responsive personal portfolio built with HTML/CSS/JS.</p>
        </div>
        <div class="project-card">
          <h3>To-Do App</h3>
          <p>A JavaScript-based app to manage your daily tasks.</p>
        </div>
        <div class="project-card">
          <h3>Weather App</h3>
          <p>Live weather data app using OpenWeatherMap API.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact" class="section">
    <div class="container">
      <h2>Contact Me</h2>
      <form id="contactForm">
        <input type="text" placeholder="Your Name" required />
        <input type="email" placeholder="Your Email" required />
        <textarea placeholder="Your Message" rows="5" required></textarea>
        <button type="submit" class="btn">Send</button>
      </form>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <p>© 2025 Nikhil. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>

