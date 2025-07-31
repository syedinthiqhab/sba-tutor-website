<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>SBA Tutoring</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <!-- Header -->
  <header>
    <div class="logo-title">
      <img src="c:\Users\syed inthiqhab alam\Pictures\sba logo.jpg" alt="SBA Logo" class="logo" />
      <h1>SBA Tutoring</h1>
    </div>
    <nav>
      <a href="#home">Home</a>
      <a href="#subjects">Subjects</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="home">
    <div class="hero-content">
      <h2>Welcome to SBA Tutoring</h2>
      <p>Empowering young minds through personalized learning experiences.</p>
      <div class="highlight-section">
        <div class="highlight-box">
          <h3>📘 Classes Offered</h3>
          <ul>
            <li>English</li>
            <li>Maths</li>
            <li>Science</li>
            <li>Social</li>
            <li>Hindi</li>
          </ul>
        </div>
        <div class="highlight-box coding">
          <h3>💻 Coding Skills</h3>
          <p>Learn basics of programming, logic building, and creative coding for school students.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Subjects Section -->
  <section class="subjects" id="subjects">
    <h2>Our Subjects</h2>
    <div class="category">
      <h3>Academic Subjects</h3>
      <ul>
        <li>English</li>
        <li>Mathematics</li>
        <li>Science</li>
        <li>Social Studies</li>
        <li>Hindi</li>
      </ul>
    </div>
    <div class="category">
      <h3>Computer Skills</h3>
      <ul>
        <li>Basic Programming</li>
        <li>Scratch Coding</li>
        <li>Problem Solving</li>
      </ul>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="contact" id="contact">
    <h2>Contact Us</h2>
    <div class="google-form">
       <iframe src="https://docs.google.com/forms/d/e/1FAIpQLSeZJxRRQNXK2C-RLAcfcfdSOypemghLSV-9zlR0XZow_g2RMg/viewform?embedded=true" width="640" height="687" frameborder="0" marginheight="0" marginwidth="0">Loading…</iframe>
    </div>
    <p class="call-us">📞 Call Us: 8870532269</p>
    <p class="email-us">📧 Email: sbatutoring@gmail.com</p>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2025 SBA Tutoring. All rights reserved.</p>
  </footer>
</body>
</html>
css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  line-height: 1.6;
  background-color: #f0f4f8;
  color: #333;
}

/* Header */
header {
  background: linear-gradient(to right, #20002c, #cbb4d4);
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 15px 30px;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo-title {
  display: flex;
  align-items: center;
}

.logo {
  width: 40px;
  height: 40px;
  margin-right: 12px;
  border-radius: 50%;
  object-fit: cover;
}

nav a {
  color: white;
  text-decoration: none;
  margin-left: 20px;
  font-weight: bold;
  transition: color 0.3s ease;
}

nav a:hover {
  color: #ffe600;
}

/* Hero Section */
.hero {
  background: url('https://media.istockphoto.com/id/1639821542/photo/teenage-girl-studding-at-home.jpg?s=612x612&w=0&k=20&c=FC_221TlkE5JhEHuraBGKuNGoEO52ikDcLynV5WqqAY=') no-repeat center center/cover;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
  padding: 40px;
  animation: zoomIn 5s ease-in-out forwards;
}

.hero-content {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 60px;
  border-radius: 16px;
  max-width: 1000px;
  opacity: 0;
  transform: translateY(40px);
  animation: fadeInUp 2s ease-out forwards, slideIn 2.5s ease-out forwards;
  animation-delay: 0.5s;
}

.hero-content h2 {
  font-size: 4rem;
  margin-bottom: 30px;
  animation: fadeInText 2s ease-in-out;
}

.hero-content p {
  font-size: 1.75rem;
  margin-bottom: 20px;
  animation: fadeInText 2.5s ease-in-out;
}

/* Highlight Section for Classes and Coding */
.highlight-section {
  display: flex;
  flex-wrap: wrap;
  gap: 40px;
  justify-content: center;
  margin-top: 30px;
}

.highlight-box {
  background: rgba(255, 255, 255, 0.1);
  border: 2px solid #ffe600;
  padding: 25px 30px;
  border-radius: 14px;
  max-width: 400px;
  text-align: left;
  animation: boxFadeIn 1.5s ease forwards;
  transition: transform 0.3s ease;
}

.highlight-box:hover {
  transform: scale(1.05);
  background: rgba(255, 255, 255, 0.2);
}

.highlight-box h3 {
  font-size: 1.8rem;
  margin-bottom: 15px;
  color: #ffe600;
}

.highlight-box ul {
  list-style: none;
  padding-left: 0;
}

.highlight-box ul li {
  font-size: 1.2rem;
  margin: 5px 0;
  color: #fff;
}

.highlight-box.coding {
  border-color: #00e0ff;
}

.highlight-box.coding h3 {
  color: #00e0ff;
}

.highlight-box.coding p {
  font-size: 1.1rem;
  color: #fff;
}

/* Animations */
@keyframes fadeInUp {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes zoomIn {
  0% {
    background-size: 100%;
  }
  100% {
    background-size: 110%;
  }
}

@keyframes slideIn {
  from {
    transform: translateX(-30px);
    opacity: 0;
  }
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

@keyframes fadeInText {
  0% {
    opacity: 0;
    transform: scale(0.95);
  }
  100% {
    opacity: 1;
    transform: scale(1);
  }
}

@keyframes boxFadeIn {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }
  100% {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Subjects Section */
.subjects {
  padding: 60px 30px;
  background: linear-gradient(to right, #f9f9f9, #e0ecff);
  text-align: center;
}

.subjects h2 {
  font-size: 2.5rem;
  color: #2c3e50;
  margin-bottom: 30px;
}

.category {
  margin-bottom: 40px;
  padding: 20px;
  background: white;
  border-radius: 16px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.category h3 {
  color: #1a237e;
  margin-bottom: 15px;
}

.category ul {
  list-style: none;
}

.category li {
  font-size: 1.1rem;
  margin: 8px 0;
}

/* Contact Section */
.contact {
  padding: 60px 30px;
  background: linear-gradient(to right, #dfefff, #e6f2ff);
  text-align: center;
}

.contact h2 {
  font-size: 2.5rem;
  margin-bottom: 20px;
  color: #0d47a1;
}

.google-form {
  max-width: 800px;
  margin: 0 auto 30px;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.1);
  border-radius: 12px;
  overflow: hidden;
}

.call-us,
.email-us {
  font-size: 1.2rem;
  margin: 10px 0;
  color: #0d47a1;
  font-weight: bold;
}

/* Footer */
footer {
  background-color: #2c3e50;
  color: white;
  padding: 20px;
  text-align: center;
}
