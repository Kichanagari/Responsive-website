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

#style.css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body, html {
  font-family: 'Segoe UI', sans-serif;
  scroll-behavior: smooth;
}

.container {
  width: 90%;
  max-width: 1000px;
  margin: auto;
}

.navbar {
  background-color: #111;
  color: #fff;
  padding: 1rem 0;
  position: sticky;
  top: 0;
  z-index: 100;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1.5rem;
  justify-content: flex-end;
}

.nav-links a {
  text-decoration: none;
  color: white;
  transition: color 0.3s;
}

.nav-links a:hover {
  color: #00bcd4;
}

.hero {
  background: #f5f5f5;
  text-align: center;
  padding: 5rem 1rem;
}

.hero h1 {
  font-size: 2.5rem;
  margin-bottom: 1rem;
}

.hero p {
  color: #555;
  font-size: 1.2rem;
  margin-bottom: 2rem;
}

.btn {
  padding: 0.8rem 2rem;
  background-color: #00bcd4;
  border: none;
  color: #fff;
  font-size: 1rem;
  cursor: pointer;
  text-decoration: none;
}

.btn:hover {
  background-color: #0097a7;
}

.section {
  padding: 4rem 0;
}

.bg-light {
  background-color: #f0f0f0;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.project-card {
  background: white;
  padding: 1.5rem;
  box-shadow: 0 0 10px rgba(0,0,0,0.1);
  border-radius: 10px;
}

#contactForm input,
#contactForm textarea {
  width: 100%;
  padding: 0.8rem;
  margin: 0.5rem 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

.footer {
  text-align: center;
  background: #111;
  color: #fff;
  padding: 1rem;
}
#script.js
document.getElementById("contactForm").addEventListener("submit", function (e) {
  e.preventDefault();
  alert("Thank you! Your message has been sent.");
  this.reset();
});
