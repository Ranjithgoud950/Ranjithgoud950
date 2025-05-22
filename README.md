<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>myRANJITHGOUD - Portfolio</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      margin: 0;
      background: linear-gradient(#f9f9f9, #e4e4e4);
      color: #333;
      scroll-behavior: smooth;
      overflow-x: hidden;
    }

    #loader {
      position: fixed;
      top: 0;
      left: 0;
      width: 100vw;
      height: 100vh;
      background: white;
      z-index: 9999;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    #loader span {
      font-size: 2rem;
      color: #5f2c82;
      animation: pulse 1.5s infinite;
    }

    @keyframes pulse {
      0%, 100% { opacity: 0.3; }
      50% { opacity: 1; }
    }

    .fade-in {
      opacity: 0;
      transform: translateY(30px);
      transition: opacity 0.8s ease-out, transform 0.8s ease-out;
    }

    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    header.hero {
      background: linear-gradient(135deg, #5f2c82, #49a09d);
      color: white;
      padding: 60px 20px;
      text-align: center;
      position: relative;
    }

    header.hero::after {
      content: "";
      position: absolute;
      bottom: -10px;
      left: 50%;
      transform: translateX(-50%);
      width: 80%;
      height: 10px;
      background: rgba(255,255,255,0.2);
      border-radius: 50%;
      filter: blur(8px);
    }

    header.hero h1 {
      font-size: 3em;
      margin: 0;
    }

    header.hero p {
      font-size: 1.3em;
      margin-top: 10px;
      opacity: 0.9;
    }

    section {
      padding: 40px 20px;
      max-width: 1000px;
      margin: auto;
    }

    h2 {
      font-size: 2em;
      margin-bottom: 10px;
      color: #5f2c82;
      position: relative;
    }

    h2::after {
      content: "";
      position: absolute;
      left: 0;
      bottom: -5px;
      width: 60px;
      height: 3px;
      background: #49a09d;
    }

    .gallery {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .gallery img {
      width: 300px;
      border-radius: 12px;
      transition: transform 0.4s ease, box-shadow 0.4s ease;
      cursor: pointer;
      animation: float 3s ease-in-out infinite;
    }

    .gallery img:hover {
      transform: scale(1.07);
      box-shadow: 0 12px 24px rgba(0, 0, 0, 0.2);
    }

    video {
      display: block;
      width: 100%;
      max-width: 600px;
      margin: 20px auto;
      border-radius: 12px;
      box-shadow: 0 5px 15px rgba(0, 0, 0, 0.15);
    }

    .contact p {
      font-size: 1.1em;
    }

    .contact a {
      display: inline-block;
      margin-top: 15px;
      padding: 12px 24px;
      background-color: #5f2c82;
      color: white;
      border-radius: 8px;
      text-decoration: none;
      font-weight: bold;
      transition: background-color 0.3s ease, transform 0.3s ease;
      animation: bounce 2s infinite;
    }

    .contact a:hover {
      background-color: #49a09d;
      transform: translateY(-3px);
    }

    @keyframes bounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }

    @keyframes float {
      0% { transform: translateY(0px); }
      50% { transform: translateY(-6px); }
      100% { transform: translateY(0px); }
    }
  </style>
</head>
<body>
  <div id="loader"><span>Loading Portfolio...</span></div>
  <audio autoplay loop hidden>
    <source src="background-music.mp3" type="audio/mpeg">
  </audio>
  <header class="hero fade-in">
    <h1>myRANJITHGOUD</h1>
    <p>Creative Graphic Designer & Video Editor</p>
  </header>

  <section class="about fade-in">
    <h2>About Me</h2>
    <p>I’m a passionate Graphic Designer and Video Editor with 1.5 years of hands-on experience in creating visually compelling designs and impactful video content. Let's make something amazing together!</p>
  </section>

  <section class="portfolio fade-in">
    <h2>My Work</h2>
    <div class="gallery">
      <img src="akshaya_tritiya.jpg" alt="Akshaya Tritiya Design">
      <img src="International2.jpg" alt="Labour Day Design">
      <img src="hanuman.jpg" alt="Hanuman Jayanti Design">
    </div>
    <video controls src="video1.mp4"></video>
    <video controls src="video2.mp4"></video>
    <video controls src="video3.mp4"></video>
  </section>

  <section class="contact fade-in">
    <h2>Contact</h2>
    <p>Email: ranjithgoud8370@gmail.com</p>
    <p>Phone: 8374940317</p>
    <a href="Resume_ranjithgoud.pdf" download>Download My Resume</a>
  </section>

  <script>
    window.addEventListener('load', () => {
      document.getElementById('loader').style.display = 'none';
      document.querySelectorAll('.fade-in').forEach(el => el.classList.add('visible'));
    });

    const observer = new IntersectionObserver(entries => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('.fade-in').forEach(el => {
      observer.observe(el);
    });
  </script>
</body>
</html>

Ranjithgoud950/Ranjithgoud950 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
