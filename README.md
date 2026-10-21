
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#080808">
<meta name="description" content="Prime Era Digital Marketing Agency. Professional websites, branding, social media marketing and creative design.">
<title>Prime Era | Digital Marketing Agency</title>

<style>
:root {
  --gold: #d8b568;
  --black: #080808;
  --card: #141414;
  --muted: #b8b8b8;
}
* { box-sizing: border-box; margin: 0; padding: 0; }
html { scroll-behavior: smooth; scroll-padding-top: 85px; }
body {
  font-family: Arial, sans-serif;
  background: var(--black);
  color: #fff;
  line-height: 1.7;
}
a { text-decoration: none; color: inherit; }
.container { width: min(1100px, 90%); margin: auto; }
header {
  position: sticky; top: 0; z-index: 100;
  background: rgba(8,8,8,.96);
  border-bottom: 1px solid #292929;
  backdrop-filter: blur(12px);
}
.nav {
  min-height: 75px; display: flex;
  justify-content: space-between; align-items: center;
  gap: 20px;
}
.logo { color: var(--gold); font-size: 25px; font-weight: 900; letter-spacing: 2px; }
nav { display: flex; align-items: center; gap: 24px; }
nav a { font-size: 14px; transition: color .2s; }
nav a:hover { color: var(--gold); }
.menu-btn {
  display: none; background: none; color: white;
  border: 1px solid #444; border-radius: 6px;
  padding: 7px 12px; font-size: 22px;
}
.hero {
  text-align: center; padding: 105px 0 95px;
  background: radial-gradient(ellipse at top, #332716 0%, #080808 65%);
}
.tag {
  color: var(--gold); font-size: 13px;
  letter-spacing: 4px; font-weight: bold;
}
h1 {
  font-size: clamp(38px, 7vw, 70px);
  line-height: 1.12; margin: 24px auto;
  max-width: 900px;
}
.gold { color: var(--gold); }
.hero p {
  color: var(--muted); font-size: 18px;
  max-width: 650px; margin: 0 auto 30px;
}
.actions {
  display: flex; justify-content: center;
  flex-wrap: wrap; gap: 14px; margin-top: 28px;
}
.btn {
  display: inline-block; padding: 13px 22px;
  border-radius: 7px; font-weight: bold;
  background: var(--gold); color: #111;
  border: 1px solid var(--gold); cursor: pointer;
  transition: .2s;
}
.btn:hover { transform: translateY(-2px); }
.btn-outline { background: transparent; color: var(--gold); }
section { padding: 75px 0; }
.section-head { text-align: center; margin-bottom: 35px; }
h2 { font-size: clamp(29px, 5vw, 42px); line-height: 1.25; margin-top: 8px; }
.section-head p { color: var(--muted); margin-top: 12px; }
.grid {
  display: grid; grid-template-columns: repeat(3, minmax(0, 1fr));
  gap: 18px;
}
.card {
  background: var(--card); border: 1px solid #303030;
  border-radius: 12px; padding: 25px;
  transition: transform .2s, border-color .2s;
}
.card:hover { transform: translateY(-5px); border-color: var(--gold); }
.icon { font-size: 32px; margin-bottom: 12px; }
.card h3 { font-size: 20px; margin-bottom: 10px; }
.card p, .muted { color: var(--muted); font-size: 15px; }
.portfolio-box {
  min-height: 155px; display: flex;
  align-items: center; justify-content: center;
  text-align: center; border-radius: 9px;
  background: linear-gradient(135deg, #57401d, #171717 75%);
  border: 1px solid #3b3020; padding: 20px;
}
.portfolio-box h3 { color: var(--gold); }
.about {
  max-width: 760px; margin: auto; text-align: center;
}
.about p { color: var(--muted); margin-top: 16px; }
.stats {
  display: grid; grid-template-columns: repeat(3, 1fr);
  gap: 15px; margin-top: 30px;
}
.stat {
  background: #111; border: 1px solid #303030;
  border-radius: 10px; padding: 20px;
}
.stat strong { color: var(--gold); display: block; font-size: 23px; }
.contact-wrap {
  display: grid; grid-template-columns: 1fr 1fr;
  gap: 30px; align-items: start;
}
.contact-info p { color: var(--muted); margin: 15px 0; }
form { display: grid; gap: 13px; }
input, textarea, select {
  width: 100%; padding: 13px;
  background: #141414; color: white;
  border: 1px solid #383838; border-radius: 7px;
  font: inherit;
}
textarea { min-height: 120px; resize: vertical; }
input:focus, textarea:focus, select:focus {
  outline: 1px solid var(--gold);
}
form .btn { width: 100%; font-size: 16px; }
footer {
  padding: 28px 0; text-align: center;
  border-top: 1px solid #292929;
  color: var(--muted); font-size: 13px;
}
.whatsapp {
  position: fixed; right: 16px; bottom: 18px;
  z-index: 99; background: #20c76a; color: #062b15;
  padding: 12px 18px; border-radius: 30px;
  font-weight: bold; box-shadow: 0 4px 18px #0008;
}
@media(max-width: 760px) {
  .nav { min-height: 68px; }
  .logo { font-size: 21px; }
  .menu-btn { display: block; }
  nav {
    display: none; position: absolute; top: 68px;
    left: 0; right: 0; padding: 18px 5%;
    background: #101010; border-bottom: 1px solid #333;
    flex-direction: column; align-items: stretch; gap: 0;
  }
  nav.open { display: flex; }
  nav a { padding: 12px 0; border-bottom: 1px solid #252525; }
  .hero { padding: 75px 0 65px; }
  .tag { letter-spacing: 2px; }
  .hero p { font-size: 16px; }
  section { padding: 58px 0; }
  .grid { grid-template-columns: 1fr; }
  .contact-wrap { grid-template-columns: 1fr; }
  .stats { gap: 8px; }
  .stat { padding: 12px 6px; }
  .stat strong { font-size: 19px; }
  .stat span { font-size: 12px; }
  .whatsapp { right: 12px; bottom: 12px; }
}
</style>
</head>

<body>
<header>
  <div class="container nav">
    <a class="logo" href="#home">PRIME ERA.</a>
    <button class="menu-btn" id="menuBtn" aria-label="Open menu"
      aria-expanded="false" aria-controls="navLinks">☰</button>
    <nav id="navLinks">
      <a href="#home">Home</a>
      <a href="#services">Services</a>
      <a href="#portfolio">Portfolio</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</header>

<main>
<section class="hero" id="home">
  <div class="container">
    <div class="tag">STRATEGY · DESIGN · GROWTH</div>
    <h1>Build Your Brand.<br><span class="gold">Grow Your Business.</span></h1>
    <p>We help businesses build a powerful online presence through professional websites, digital advertising and creative design.</p>
    <div class="actions">
      <a class="btn" href="#services">Explore Services ↗</a>
      <a class="btn btn-outline" href="#contact">Contact Us</a>
    </div>
  </div>
</section>

<section id="services">
  <div class="container">
    <div class="section-head">
      <div class="tag">WHAT WE DO</div>
      <h2>Our <span class="gold">Services</span></h2>
      <p>Creative solutions to help your business stand out.</p>
    </div>
    <div class="grid">
      <article class="card">
        <div class="icon">💻</div>
        <h3>Website Development</h3>
        <p>Modern, responsive websites designed to showcase your brand and convert visitors into customers.</p>
      </article>
      <article class="card">
        <div class="icon">📱</div>
        <h3>Social Media Marketing</h3>
        <p>Build your online presence with engaging content and a consistent social media strategy.</p>
      </article>
      <article class="card">
        <div class="icon">🎯</div>
        <h3>Digital Advertising</h3>
        <p>Reach the right audience with targeted advertising campaigns for your business goals.</p>
      </article>
      <article class="card">
        <div class="icon">🎨</div>
        <h3>Logo & Brand Identity</h3>
        <p>Create a memorable brand with thoughtful logos, colors and professional visual design.</p>
      </article>
      <article class="card">
        <div class="icon">🎬</div>
        <h3>Creative Content</h3>
        <p>Promotional graphics, reels and creative concepts to communicate your brand's message.</p>
      </article>
      <article class="card">
        <div class="icon">📈</div>
        <h3>Growth Strategy</h3>
        <p>Practical digital strategies to strengthen your brand visibility and customer engagement.</p>
      </article>
    </div>
  </div>
</section>

<section id="portfolio">
  <div class="container">
    <div class="section-head">
      <div class="tag">OUR WORK</div>
      <h2>Creative <span class="gold">Portfolio</span></h2>
      <p>A glimpse of the projects and ideas we can create for your brand.</p>
    </div>
    <div class="grid">
      <div class="portfolio-box"><h3>01<br>Website Design</h3></div>
      <div class="portfolio-box"><h3>02<br>Brand Identity</h3></div>
      <div class="portfolio-box"><h3>03<br>Social Media Creatives</h3></div>
    </div>
    <p class="muted" style="text-align:center;margin-top:18px">
      These are service examples. Add your actual completed projects here.
    </p>
  </div>
</section>

<section id="about">
  <div class="container">
    <div class="about">
      <div class="tag">WHO WE ARE</div>
      <h2>Ideas Into <span class="gold">Impact.</span></h2>
      <p>Prime Era is a digital marketing and creative agency focused on helping businesses present themselves professionally online. From websites and branding to social media content, our goal is to make your brand memorable.</p>
      <div class="stats">
        <div class="stat"><strong>Design</strong><span>Creative Ideas</span></div>
        <div class="stat"><strong>Digital</strong><span>Modern Solutions</span></div>
        <div class="stat"><strong>Growth</strong><span>Business Focus</span></div>
      </div>
    </div>
  </div>
</section>

<section id="contact">
  <div class="container">
    <div class="section-head">
      <div class="tag">LET'S CONNECT</div>
      <h2>Start Your <span class="gold">Project</span></h2>
      <p>Tell us about your business and what you want to create.</p>
    </div>
    <div class="contact-wrap">
      <div class="contact-info">
        <h3>Let's build something great.</h3>
        <p>Have a website, branding or marketing project in mind? Send us your details and let's discuss your ideas.</p>
        <p>📍 Location: Add your business location</p>
        <p>💬 WhatsApp: Use the button to contact us</p>
      </div>
      <form id="contactForm">
        <input id="name" type="text" placeholder="Your name" required>
        <input id="phone" type="tel" placeholder="Your phone number" required>
        <select id="service" required>
          <option value="">Choose a service</option>
          <option>Website Development</option>
          <option>Social Media Marketing</option>
          <option>Digital Advertising</option>
          <option>Logo & Brand Identity</option>
          <option>Creative Content</option>
          <option>Other</option>
        </select>
        <textarea id="message" placeholder="Tell us about your project" required></textarea>
        <button class="btn" type="submit">Send Enquiry on WhatsApp ↗</button>
      </form>
    </div>
  </div>
</section>
</main>

<footer>
  <div class="container">
    <p class="logo">PRIME ERA.</p>
    <p>Strategy · Design · Growth</p>
    <p style="margin-top:12px">© <span id="year"></span> Prime Era. All rights reserved.</p>
  </div>
</footer>

<a class="whatsapp" id="whatsappBtn" href="#" target="_blank"
   rel="noopener noreferrer" aria-label="Contact Prime Era on WhatsApp">
  WhatsApp ↗
</a>

<script>
/* IMPORTANT: Replace this with your WhatsApp number.
   Use country code + number, digits only. Example: 919876543210 */
const WHATSAPP_NUMBER = "91XXXXXXXXXX";

const menuBtn = document.getElementById("menuBtn");
const navLinks = document.getElementById("navLinks");

menuBtn.addEventListener("click", () => {
  const isOpen = navLinks.classList.toggle("open");
  menuBtn.setAttribute("aria-expanded", String(isOpen));
  menuBtn.textContent = isOpen ? "✕" : "☰";
});

navLinks.querySelectorAll("a").forEach(link => {
  link.addEventListener("click", () => {
    navLinks.classList.remove("open");
    menuBtn.setAttribute("aria-expanded", "false");
    menuBtn.textContent = "☰";
  });
});

document.getElementById("year").textContent = new Date().getFullYear();

function openWhatsApp(message) {
  if (!/^91\d{10}$/.test(WHATSAPP_NUMBER)) {
    alert("Please add your WhatsApp number in the website code first.");
    return;
  }
  const url = "https://wa.me/" + WHATSAPP_NUMBER +
    "?text=" + encodeURIComponent(message);
  window.open(url, "_blank", "noopener");
}

document.getElementById("whatsappBtn").addEventListener("click", event => {
  event.preventDefault();
  openWhatsApp("Hello Prime Era! I would like to know about your services.");
});

document.getElementById("contactForm").addEventListener("submit", event => {
  event.preventDefault();
  const name = document.getElementById("name").value.trim();
  const phone = document.getElementById("phone").value.trim();
  const service = document.getElementById("service").value;
  const message = document.getElementById("message").value.trim();

  if (!name || !phone || !service || !message) {
    alert("Please complete all fields.");
    return;
  }

  openWhatsApp(
    "Hello Prime Era!\n" +
    "Name: " + name + "\n" +
    "Phone: " + phone + "\n" +
    "Service: " + service + "\n" +
    "Project details: " + message
  );
});
</script>
</body>
</html>

<!-- Floating WhatsApp Button -->
<a
  href="https://wa.me/918055905561?text=Hello%20Prime%20Era%2C%20I%20want%20to%20know%20about%20your%20digital%20marketing%20services."
  class="whatsapp-float"
  target="_blank"
  rel="noopener noreferrer"
  aria-label="Chat with Prime Era on WhatsApp"
>
  WhatsApp Us
</a>

<style>
.whatsapp-float {
  position: fixed;
  right: 18px;
  bottom: 20px;
  z-index: 9999;
  background: #25D366;
  color: #fff;
  padding: 14px 20px;
  border-radius: 50px;
  font-size: 16px;
  font-weight: bold;
  text-decoration: none;
  box-shadow: 0 4px 12px rgba(0,0,0,.25);
}
.whatsapp-float:hover {
  background: #128C7E;
}
</style>
