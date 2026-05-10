<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Our Wedding</title>

<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: "Georgia", serif;
}

body {
  background: #fff;
  color: #222;
}

/* NAV */
nav {
  position: fixed;
  top: 0;
  width: 100%;
  background: rgba(255,255,255,0.9);
  padding: 15px;
  text-align: center;
  z-index: 10;
  border-bottom: 1px solid #eee;
}

nav a {
  margin: 0 15px;
  text-decoration: none;
  color: #333;
  font-size: 14px;
}

/* HERO */
.hero {
  height: 100vh;
  background: url('images/wedding/hero.jpg') center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
  position: relative;
}

.hero::after {
  content: "";
  position: absolute;
  top:0; left:0;
  width:100%;
  height:100%;
  background: rgba(0,0,0,0.4);
}

.hero-content {
  position: relative;
  z-index: 1;
}

.hero h1 {
  font-size: 48px;
  letter-spacing: 2px;
}

.hero p {
  margin-top: 10px;
  font-size: 18px;
}

/* SECTIONS */
section {
  padding: 80px 20px;
  max-width: 1100px;
  margin: auto;
}

/* GALLERY */
.gallery {
  column-count: 3;
  column-gap: 15px;
}

.gallery img {
  width: 100%;
  margin-bottom: 15px;
  border-radius: 8px;
  break-inside: avoid;
}
<h2>Our Memories</h2>


<div style="display:grid;grid-template-columns:repeat(auto-fit,minmax(200px,1fr));gap:10px;">

  <img src="photos/0G9A5789.jpg" style="width:100%;border-radius:10px;">
  <img src="photos/0G9A6195.29.jpg" style="width:100%;border-radius:10px;">
  <img src="photos/0G9A7999.JPG" style="width:100%;border-radius:10px;">


</div>
/* RSVP */
.rsvp {
  text-align: center;
}

input, textarea {
  width: 100%;
  max-width: 400px;
  padding: 10px;
  margin: 10px 0;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  padding: 10px 20px;
  border: none;
  background: #222;
  color: white;
  cursor: pointer;
  border-radius: 5px;
}

footer {
  text-align: center;
  padding: 30px;
  font-size: 12px;
  color: #777;
}

/* MOBILE */
@media(max-width: 768px){
  .gallery { column-count: 2; }
  .hero h1 { font-size: 32px; }
}
</style>

</head>

<body>

<nav>
  <a href="#home">Home</a>
  <a href="#gallery">Gallery</a>
  <a href="#rsvp">RSVP</a>
</nav>

<!-- HERO -->
<section class="hero" id="home">
  <div class="hero-content">
    <h1>Our Wedding</h1>
    <p>Two hearts, one journey</p>
  </div>
</section>

<!-- GALLERY -->
<section id="gallery">
  <h2 style="text-align:center; margin-bottom:40px;">Gallery</h2>

  <div class="gallery">

    <!-- Wedding photos -->
    <img src="images/wedding/1.jpg">
    <img src="images/wedding/2.jpg">
    <img src="images/wedding/3.jpg">

    <!-- Non-wedding photos -->
    <img src="images/nonwedding/1.jpg">
    <img src="images/nonwedding/2.jpg">
    <img src="images/nonwedding/3.jpg">

  </div>
</section>

<!-- RSVP -->
<section id="rsvp" class="rsvp">
  <h2>RSVP</h2>
  <p style="margin:10px 0 20px;">We’d love to hear from you</p>

  <input type="text" placeholder="Your Name" />
  <input type="email" placeholder="Your Email" />
  <textarea rows="4" placeholder="Message"></textarea><br/>
  <button>Send</button>
</section>

<footer>
  Made with love ❤️
</footer>

</body>
</html>
