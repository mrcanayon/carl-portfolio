<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Carl's Portfolio</title>

  <!-- Google Font -->
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    html {
      scroll-behavior: smooth;
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Poppins', sans-serif;
      background-color: #ffffff;
      color: #333;
      line-height: 1.6;
      transition: background-color 0.3s ease, color 0.3s ease;
    }

    header {
      background: #1f1f1f;
      color: white;
      padding: 60px 20px;
      text-align: center;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }

    header h1 {
      font-size: 3rem;
      margin-bottom: 10px;
    }

    header p {
      font-size: 1.2rem;
      color: #bbb;
    }

    nav {
      background: #272727;
      display: flex;
      justify-content: center;
      padding: 15px 0;
      position: sticky;
      top: 0;
      z-index: 100;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      margin: 0 20px;
      font-weight: 500;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #00bcd4;
    }

    section {
      padding: 60px 20px;
      max-width: 1000px;
      margin: auto;
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.8s ease, transform 0.8s ease;
    }

    section.show {
      opacity: 1;
      transform: translateY(0);
    }

    section h2 {
      font-size: 2rem;
      color: #222;
      margin-bottom: 20px;
      position: relative;
    }

    section h2::after {
      content: "";
      display: block;
      width: 60px;
      height: 4px;
      background: #00bcd4;
      margin-top: 10px;
      border-radius: 2px;
    }

    ul {
      list-style: none;
    }

    ul li {
      background: #f9f9f9;
      margin: 10px 0;
      padding: 15px 20px;
      border-left: 4px solid #00bcd4;
      border-radius: 5px;
      transition: transform 0.2s ease;
    }

    ul li:hover {
      transform: scale(1.02);
    }

    a {
      color: #00bcd4;
    }

    .seowon {
      text-align: left;
    }

    .seowon img {
      max-width: 300px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
      margin-top: 20px;
    }

    .seowon p {
      margin-top: 15px;
      font-weight: 500;
      font-size: 1.1rem;
      color: #444;
    }

    .carousel {
      display: flex;
      justify-content: center;
      align-items: center;
      overflow: hidden;
      position: relative;
      height: 350px;
      margin-top: 30px;
    }

    .carousel img {
      position: absolute;
      max-width: 100%;
      max-height: 100%;
      opacity: 0;
      transition: opacity 0.5s ease;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
    }

    .carousel img.active {
      opacity: 1;
      position: relative;
    }

    .carousel-buttons {
      text-align: center;
      margin-top: 10px;
    }

    .carousel-buttons button {
      background-color: #00bcd4;
      color: white;
      border: none;
      padding: 10px 20px;
      margin: 0 10px;
      border-radius: 8px;
      cursor: pointer;
      font-size: 1.2rem;
      transition: background-color 0.3s;
    }

    .carousel-buttons button:hover {
      background-color: #0097a7;
    }

    footer {
      background: #1f1f1f;
      color: white;
      text-align: center;
      padding: 25px 20px;
      font-size: 0.9rem;
      margin-top: 40px;
    }

    @media (max-width: 600px) {
      header h1 {
        font-size: 2rem;
      }

      nav {
        flex-direction: column;
      }

      nav a {
        margin: 10px 0;
      }
    }
    
.seowon-form {
  background: #f0fbfd;
  padding: 30px;
  border-radius: 16px;
  box-shadow: 0 4px 15px rgba(0, 188, 212, 0.2);
  max-width: 600px;
  margin: 30px auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.seowon-form input,
.seowon-form textarea {
  padding: 12px 15px;
  border: 2px solid #b2ebf2;
  border-radius: 12px;
  font-family: 'Poppins', sans-serif;
  font-size: 1rem;
  background-color: #ffffff;
  color: #333;
  transition: border-color 0.3s, box-shadow 0.3s;
}

.seowon-form input:focus,
.seowon-form textarea:focus {
  border-color: #00bcd4;
  box-shadow: 0 0 8px rgba(0, 188, 212, 0.3);
  outline: none;
}

.seowon-form button {
  background-color: #00bcd4;
  color: white;
  padding: 12px 20px;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  border-radius: 12px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.seowon-form button:hover {
  background-color: #0097a7;
}

/* 🖼️ Floating Seowon image */
.seowon-sticker {
  width: 80px;
  border-radius: 50%;
  box-shadow: 0 4px 12px rgba(0, 188, 212, 0.3);
  position: absolute;
  right: 40px;
  transform: rotate(-6deg);
  margin-top: -20px;
  z-index: 10;
  transition: transform 0.3s ease;
}

.seowon-sticker:hover {
  transform: scale(1.1) rotate(0deg);
}

/* 💖 Sparkle Button */
.sparkle-button {
  position: relative;
  overflow: hidden;
}

.sparkle-button::after {
  content: "✨💖✨";
  position: absolute;
  right: 10px;
  top: 50%;
  transform: translateY(-50%);
  opacity: 0;
  transition: opacity 0.3s ease, right 0.3s ease;
}

.sparkle-button:hover::after {
  right: 15px;
  opacity: 1;
}

  </style>
</head>
<body>

  <header>
    <h1>Carl Justine Canayon</h1>
    <p>Web Developer | Gamer | Coffee Enthusiast ☕</p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#skills">Skills</a>
    <a href="#projects">Projects</a>
    <a href="#seowon">Seowon 💖</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Me</h2>
    <p>Hi! I'm Carl, a passionate web developer from the Philippines. I love building responsive and user-friendly websites.</p>
    <p>Also a proud fan of <strong>Seowon from UNIS 💖</strong> — her talent and energy inspire me every day to code better and vibe harder.</p>
  </section>
  
<section id="skills">
  <h2>Skills</h2>
  <ul>
    <li>HTML5, CSS3, JavaScript (ES6+)</li>
    <li>React.js, Vue.js</li>
    <li>Git & GitHub</li>
    <li>Responsive Web Design</li>
    <li>Basic UI/UX Design</li>
  </ul>
</section>


  <section id="projects">
    <h2>Projects</h2>
    <ul>
      <li><strong>Project A:</strong> A website for local businesses</li>
      <li><strong>Project B:</strong> A personal blog using HTML/CSS/JS</li>
      <li><strong>Project C:</strong> A to-do app built with React</li>
    </ul>
  </section>

  <section id="seowon" class="seowon">
    <h2>Seowon 💖</h2>
    <div class="carousel">
      <img src="https://kpopping.com/documents/f6/4/250531-UNIS-Twitter-Update-Seowon-documents-1.jpeg?v=95233" class="active" alt="Seowon 1">
      <img src="https://kpopping.com/documents/84/1/250608-UNIS-Twitter-Update-Seowon-documents-1.jpeg?v=95233" alt="Seowon 2">
      <img src="https://kpopping.com/documents/55/3/250504-UNIS-Twitter-Update-Seowon-documents-1(1).jpeg?v=95233" alt="Seowon 3">
    </div>

    <div class="carousel-buttons">
      <button id="prev">⟨</button>
      <button id="next">⟩</button>
    </div>

    <div style="max-width: 500px; margin: 20px auto; text-align: left; background: #fff; padding: 20px; border-radius: 12px; box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);">
      <h3 style="text-align:center; color: #00bcd4;">Seowon Profile</h3>
      <ul style="list-style: none; padding: 0; font-size: 1rem;">
        <li><strong>Full Name:</strong> Lim Seowon (김서원)</li>
        <li><strong>Birthday:</strong> January 27, 2011</li>
        <li><strong>Nationality:</strong> Korean 🇰🇷</li>
        <li><strong>Group:</strong> UNIS (유니스)</li>
        <li><strong>Position:</strong> Main Vocalist, Maknae</li>
        <li><strong>Debut:</strong> 2024, under F&F Entertainment</li>
      </ul>
      <p style="margin-top: 15px;">
        Seowon is known for her charismatic stage presence and graceful visuals. As one of the youngest in UNIS, she inspires many with her confidence, energy, and talent. Stan Seowon! 🌟
      </p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact Me</h2>
    <p>Email: canayoncarljustine@gmail.com</p>
    <p>GitHub: <a href="https://github.com/mrcanayon" target="_blank">mrcanayon</a></p>
    
<!-- Seowon Floating Image -->
  <img src="https://kpopping.com/documents/9c/1/250526-UNIS-Twitter-Update-Seowon-documents-1.jpeg?v=95233"
       alt="Seowon Sticker"
       class="seowon-sticker">
       
<form class="seowon-form" action="https://formspree.io/f/xovwegwr" method="POST" target="_blank
  <input type="text" name="name" placeholder="Your Name 💖" required />
  <input type="email" name="email" placeholder="Your Email ✉️" required />
  <textarea name="message" rows="5" placeholder="Your Message to Carl ✍️" required></textarea>
  <button type="submit" class="sparkle-button">Send Message 💌</button>
</form>



<footer>
  <p>© 2025 Carl Justine Canayon. All rights reserved.</p>
  <div>
    <a href="https://github.com/mrcanayon" target="_blank">GitHub</a> |
    <a href="https://linkedin.com/in/carl-justine-canayon-48666a276" target="_blank">LinkedIn</a>
  </div>
</footer>

  <script>
    const sections = document.querySelectorAll("section");

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add("show");
        }
      });
    }, {
      threshold: 0.1
    });

    sections.forEach(section => {
      observer.observe(section);
    });
  </script>

  <script>
    const images = document.querySelectorAll('.carousel img');
    let current = 0;
    let interval;

    function showImage(index) {
      images.forEach((img, i) => {
        img.classList.remove('active');
        if (i === index) img.classList.add('active');
      });
    }

    function nextImage() {
      current = (current + 1) % images.length;
      showImage(current);
    }

    function prevImage() {
      current = (current - 1 + images.length) % images.length;
      showImage(current);
    }

    function startAutoPlay() {
      interval = setInterval(nextImage, 3000);
    }

    function resetAutoPlay() {
      clearInterval(interval);
      startAutoPlay();
    }

    document.getElementById('next').addEventListener('click', () => {
      nextImage();
      resetAutoPlay();
    });

    document.getElementById('prev').addEventListener('click', () => {
      prevImage();
      resetAutoPlay();
    });

    showImage(current);
    startAutoPlay();
  </script>

</body>
</html>
