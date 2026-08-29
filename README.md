<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>C2 Creations Photography | Luxury Wedding Photography</title>

<meta name="description"
content="C2 Creations Photography — Luxury Wedding Photography, Candid Photography, Pre-Wedding and Cinematic Wedding Films.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>

:root{
  --ivory:#fbf6ef;
  --cream:#f4e8da;
  --burgundy:#641d2d;
  --wine:#7b293c;
  --plum:#452536;
  --gold:#c7a56a;
  --gold-light:#e5c995;
  --peach:#e8b39e;
  --brown:#392725;
  --white:#fffdf9;
}

*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

html{
  scroll-behavior:smooth;
}

body{
  background:var(--ivory);
  color:var(--brown);
  font-family:"DM Sans",sans-serif;
  overflow-x:hidden;
}

a{
  text-decoration:none;
  color:inherit;
}

img{
  width:100%;
  display:block;
}

/* =========================
   NAVBAR
========================= */

.navbar{
  position:fixed;
  top:0;
  left:0;
  width:100%;
  z-index:1000;
  padding:22px 5%;
  display:flex;
  align-items:center;
  justify-content:space-between;
  transition:.4s;
}

.navbar.scrolled{
  background:rgba(69,37,54,.96);
  backdrop-filter:blur(12px);
  padding:15px 5%;
  box-shadow:0 10px 30px rgba(0,0,0,.08);
}

.logo{
  font-family:"Cormorant Garamond",serif;
  color:white;
  font-size:27px;
  letter-spacing:3px;
  font-weight:600;
}

.logo span{
  display:block;
  font-family:"DM Sans",sans-serif;
  font-size:8px;
  letter-spacing:4px;
  text-align:center;
  margin-top:-4px;
  color:var(--gold-light);
}

.nav-links{
  display:flex;
  gap:30px;
  list-style:none;
  color:white;
  font-size:12px;
  letter-spacing:1.5px;
  text-transform:uppercase;
}

.nav-links a{
  position:relative;
}

.nav-links a:after{
  content:"";
  position:absolute;
  bottom:-7px;
  left:0;
  width:0;
  height:1px;
  background:var(--gold-light);
  transition:.3s;
}

.nav-links a:hover:after{
  width:100%;
}

.menu-btn{
  display:none;
  color:white;
  font-size:27px;
  cursor:pointer;
}

/* =========================
   HERO
========================= */

.hero{
  min-height:100vh;
  position:relative;
  display:flex;
  align-items:center;
  justify-content:center;
  overflow:hidden;

  background:
  linear-gradient(
    90deg,
    rgba(44,19,27,.58),
    rgba(74,25,39,.18),
    rgba(44,19,27,.35)
  ),
  url("YOUR-HERO-PHOTO-URL") center/cover no-repeat;
}

.hero:before{
  content:"";
  position:absolute;
  inset:0;
  background:
  radial-gradient(
    circle at 50% 45%,
    transparent 10%,
    rgba(40,15,22,.25) 100%
  );
}

.hero-content{
  position:relative;
  z-index:2;
  text-align:center;
  color:white;
  max-width:900px;
  padding:30px;
  animation:heroIn 1.5s ease;
}

@keyframes heroIn{
  from{
    opacity:0;
    transform:translateY(35px);
  }
  to{
    opacity:1;
    transform:translateY(0);
  }
}

.hero-small{
  letter-spacing:6px;
  text-transform:uppercase;
  font-size:11px;
  color:var(--gold-light);
  margin-bottom:20px;
}

.hero h1{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(55px,8vw,110px);
  line-height:.82;
  font-weight:500;
  letter-spacing:-2px;
}

.hero h1 span{
  color:var(--gold-light);
  font-style:italic;
}

.hero p{
  margin:30px auto;
  max-width:600px;
  font-family:"Cormorant Garamond",serif;
  font-size:22px;
  line-height:1.5;
}

.hero-btn{
  display:inline-block;
  border:1px solid var(--gold-light);
  padding:15px 32px;
  color:white;
  font-size:11px;
  letter-spacing:2px;
  text-transform:uppercase;
  transition:.35s;
}

.hero-btn:hover{
  background:var(--gold-light);
  color:var(--plum);
}

.scroll{
  position:absolute;
  bottom:25px;
  left:50%;
  transform:translateX(-50%);
  color:white;
  font-size:10px;
  letter-spacing:3px;
  text-transform:uppercase;
}

/* =========================
   GENERAL
========================= */

.section{
  padding:110px 7%;
}

.section-heading{
  text-align:center;
  max-width:800px;
  margin:0 auto 60px;
}

.eyebrow{
  color:var(--wine);
  text-transform:uppercase;
  letter-spacing:4px;
  font-size:10px;
  margin-bottom:15px;
}

.section-heading h2{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(45px,6vw,72px);
  line-height:.95;
  font-weight:500;
  color:var(--plum);
}

.section-heading p{
  margin-top:20px;
  font-size:14px;
  line-height:1.8;
  color:#715e59;
}

/* =========================
   INTRO
========================= */

.intro{
  background:var(--ivory);
}

.intro-grid{
  max-width:1100px;
  margin:auto;
  display:grid;
  grid-template-columns:1fr 1.2fr;
  gap:70px;
  align-items:center;
}

.intro-image{
  position:relative;
}

.intro-image img{
  height:600px;
  object-fit:cover;
}

.intro-image:after{
  content:"";
  position:absolute;
  width:80%;
  height:80%;
  border:1px solid var(--gold);
  top:-20px;
  left:-20px;
  z-index:-1;
}

.intro-text h3{
  font-family:"Cormorant Garamond",serif;
  font-size:48px;
  font-weight:500;
  color:var(--plum);
  line-height:1;
}

.intro-text p{
  margin:25px 0;
  line-height:1.9;
  color:#6f5c57;
  font-size:14px;
}

.signature{
  font-family:"Cormorant Garamond",serif;
  color:var(--wine);
  font-size:30px;
  font-style:italic;
}

/* =========================
   SERVICES
========================= */

.services{
  background:linear-gradient(135deg,#f1e1d4,#fbf6ef);
}

.services-grid{
  max-width:1100px;
  margin:auto;
  display:grid;
  grid-template-columns:repeat(4,1fr);
  gap:20px;
}

.service{
  background:rgba(255,255,255,.65);
  border:1px solid rgba(199,165,106,.35);
  padding:45px 25px;
  text-align:center;
  transition:.4s;
}

.service:hover{
  transform:translateY(-10px);
  background:white;
  box-shadow:0 20px 50px rgba(77,38,47,.1);
}

.service-number{
  color:var(--gold);
  font-family:"Cormorant Garamond",serif;
  font-size:25px;
}

.service h3{
  margin:18px 0 12px;
  font-family:"Cormorant Garamond",serif;
  font-size:29px;
  color:var(--plum);
}

.service p{
  font-size:12px;
  line-height:1.7;
  color:#78635d;
}

/* =========================
   PORTFOLIO
========================= */

.portfolio{
  background:var(--plum);
  color:white;
}

.portfolio .section-heading h2{
  color:white;
}

.portfolio .section-heading p{
  color:#d7c8c2;
}

.gallery{
  max-width:1200px;
  margin:auto;
  columns:3 250px;
  column-gap:15px;
}

.gallery-item{
  position:relative;
  margin-bottom:15px;
  overflow:hidden;
  break-inside:avoid;
}

.gallery-item img{
  transition:.7s;
}

.gallery-item:hover img{
  transform:scale(1.06);
}

.gallery-overlay{
  position:absolute;
  inset:0;
  display:flex;
  align-items:flex-end;
  padding:25px;
  background:linear-gradient(transparent,rgba(35,14,23,.75));
  opacity:0;
  transition:.4s;
}

.gallery-item:hover .gallery-overlay{
  opacity:1;
}

.gallery-overlay span{
  font-family:"Cormorant Garamond",serif;
  font-size:25px;
}

/* =========================
   FEATURE
========================= */

.feature{
  min-height:620px;
  display:flex;
  align-items:center;
  justify-content:center;
  text-align:center;
  color:white;

  background:
  linear-gradient(rgba(79,23,39,.55),rgba(79,23,39,.55)),
  url("YOUR-COUPLE-PHOTO-URL") center/cover fixed;
}

.feature-content{
  max-width:850px;
  padding:30px;
}

.feature h2{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(50px,7vw,85px);
  line-height:.9;
  font-weight:500;
}

.feature p{
  margin:25px auto;
  font-family:"Cormorant Garamond",serif;
  font-size:22px;
  max-width:650px;
}

/* =========================
   TESTIMONIAL
========================= */

.testimonials{
  background:var(--cream);
}

.testimonial-box{
  max-width:850px;
  margin:auto;
  text-align:center;
}

.quote{
  color:var(--gold);
  font-family:"Cormorant Garamond",serif;
  font-size:65px;
  line-height:.5;
}

.testimonial-text{
  font-family:"Cormorant Garamond",serif;
  font-size:30px;
  line-height:1.4;
  color:var(--plum);
  margin:30px 0;
}

.client{
  color:var(--wine);
  font-size:11px;
  text-transform:uppercase;
  letter-spacing:3px;
}

/* =========================
   CTA
========================= */

.cta{
  padding:110px 7%;
  text-align:center;
  background:
  radial-gradient(circle at 20% 30%,rgba(232,179,158,.3),transparent 30%),
  radial-gradient(circle at 80% 70%,rgba(199,165,106,.25),transparent 30%),
  var(--ivory);
}

.cta h2{
  font-family:"Cormorant Garamond",serif;
  font-size:clamp(50px,7vw,90px);
  color:var(--plum);
  line-height:.9;
}

.cta p{
  margin:25px auto;
  max-width:600px;
  line-height:1.7;
  color:#715e59;
}

.cta-buttons{
  display:flex;
  justify-content:center;
  gap:15px;
  flex-wrap:wrap;
}

.btn{
  display:inline-block;
  padding:16px 30px;
  background:var(--burgundy);
  color:white;
  font-size:11px;
  letter-spacing:2px;
  text-transform:uppercase;
  transition:.3s;
}

.btn:hover{
  background:var(--plum);
  transform:translateY(-3px);
}

.btn-outline{
  background:transparent;
  color:var(--burgundy);
  border:1px solid var(--burgundy);
}

/* =========================
   FOOTER
========================= */

footer{
  background:var(--plum);
  color:white;
  padding:70px 7% 25px;
}

.footer-grid{
  max-width:1100px;
  margin:auto;
  display:grid;
  grid-template-columns:2fr 1fr 1fr;
  gap:50px;
}

.footer-brand h2{
  font-family:"Cormorant Garamond",serif;
  font-size:38px;
  font-weight:500;
}

.footer-brand p{
  margin-top:15px;
  max-width:400px;
  line-height:1.7;
  color:#cbbcb8;
  font-size:13px;
}

.footer-title{
  color:var(--gold-light);
  font-size:11px;
  letter-spacing:2px;
  text-transform:uppercase;
  margin-bottom:20px;
}

.footer-links{
  list-style:none;
}

.footer-links li{
  margin-bottom:12px;
  font-size:13px;
  color:#ddd0ca;
}

.footer-bottom{
  border-top:1px solid rgba(255,255,255,.12);
  margin-top:50px;
  padding-top:20px;
  text-align:center;
  font-size:10px;
  color:#bcaeaa;
}

/* =========================
   WHATSAPP
========================= */

.whatsapp{
  position:fixed;
  right:22px;
  bottom:22px;
  width:58px;
  height:58px;
  border-radius:50%;
  background:#25d366;
  color:white;
  display:flex;
  align-items:center;
  justify-content:center;
  font-size:27px;
  z-index:999;
  box-shadow:0 10px 30px rgba(0,0,0,.2);
  transition:.3s;
}

.whatsapp:hover{
  transform:scale(1.1);
}

/* =========================
   RESPONSIVE
========================= */

@media(max-width:850px){

  .nav-links{
    position:absolute;
    top:70px;
    right:5%;
    background:var(--plum);
    width:230px;
    padding:25px;
    display:none;
    flex-direction:column;
    gap:20px;
    box-shadow:0 15px 40px rgba(0,0,0,.2);
  }

  .nav-links.active{
    display:flex;
  }

  .menu-btn{
    display:block;
  }

  .intro-grid{
    grid-template-columns:1fr;
    gap:50px;
  }

  .intro-image img{
    height:500px;
  }

  .services-grid{
    grid-template-columns:1fr 1fr;
  }

  .footer-grid{
    grid-template-columns:1fr;
  }

}

@media(max-width:550px){

  .navbar{
    padding:18px 5%;
  }

  .logo{
    font-size:22px;
  }

  .hero{
    min-height:90vh;
  }

  .hero h1{
    font-size:58px;
  }

  .hero p{
    font-size:18px;
  }

  .section{
    padding:80px 6%;
  }

  .services-grid{
    grid-template-columns:1fr;
  }

  .intro-image img{
    height:430px;
  }

  .testimonial-text{
    font-size:25px;
  }

}

/* =========================
   REVEAL ANIMATION
========================= */

.reveal{
  opacity:0;
  transform:translateY(35px);
  transition:1s ease;
}

.reveal.show{
  opacity:1;
  transform:translateY(0);
}

</style>
</head>


<body>

<!-- =========================
     NAVIGATION
========================= -->

<header class="navbar" id="navbar">

  <a href="#home" class="logo">
    C2 CREATIONS
    <span>PHOTOGRAPHY</span>
  </a>

  <nav>
    <ul class="nav-links" id="navLinks">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#services">Services</a></li>
      <li><a href="#portfolio">Portfolio</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <div class="menu-btn" onclick="toggleMenu()">☰</div>

</header>


<!-- =========================
     HERO
========================= -->

<section class="hero" id="home">

  <div class="hero-content">

    <div class="hero-small">
      Luxury Wedding Photography
    </div>

    <h1>
      Stories<br>
      <span>Worth Remembering</span>
    </h1>

    <p>
      We capture the emotions, elegance and little moments
      that make your wedding uniquely yours.
    </p>

    <a href="#portfolio" class="hero-btn">
      Explore Our Work
    </a>

  </div>

  <div class="scroll">
    Scroll to discover
  </div>

</section>


<!-- =========================
     ABOUT
========================= -->

<section class="section intro" id="about">

  <div class="intro-grid">

    <div class="intro-image reveal">
      <img
      src="YOUR-ABOUT-PHOTO-URL"
      alt="C2 Creations Photography Wedding">
    </div>

    <div class="intro-text reveal">

      <div class="eyebrow">
        The Art of Storytelling
      </div>

      <h3>
        Your love story,<br>
        beautifully preserved.
      </h3>

      <p>
        At C2 Creations Photography, we believe wedding photography
        is more than simply taking pictures.
      </p>

      <p>
        It is about preserving the laughter, emotions, glances,
        celebrations and beautiful details that you will want
        to relive for years to come.
      </p>

      <p>
        Our approach combines cinematic storytelling,
        candid emotions and timeless portraits to create
        photographs that feel as beautiful as the memories themselves.
      </p>

      <div class="signature">
        C2 Creations
      </div>

    </div>

  </div>

</section>


<!-- =========================
     SERVICES
========================= -->

<section class="section services" id="services">

  <div class="section-heading reveal">

    <div class="eyebrow">
      What We Capture
    </div>

    <h2>
      Crafted for your<br>
      once-in-a-lifetime moments.
    </h2>

    <p>
      From intimate ceremonies to grand celebrations,
      every frame is thoughtfully created.
    </p>

  </div>


  <div class="services-grid">

    <div class="service reveal">
      <div class="service-number">01</div>
      <h3>Wedding</h3>
      <p>
        Complete wedding photography with timeless
        portraits and authentic moments.
      </p>
    </div>

    <div class="service reveal">
      <div class="service-number">02</div>
      <h3>Candid</h3>
      <p>
        Natural emotions and spontaneous moments
        captured beautifully.
      </p>
    </div>

    <div class="service reveal">
      <div class="service-number">03</div>
      <h3>Pre-Wedding</h3>
      <p>
        Romantic and cinematic storytelling
        created around your connection.
      </p>
    </div>

    <div class="service reveal">
      <div class="service-number">04</div>
      <h3>Cinematic Films</h3>
      <p>
        Emotional wedding films crafted
        like a beautiful cinematic story.
      </p>
    </div>

  </div>

</section>


<!-- =========================
     PORTFOLIO
========================= -->

<section class="section portfolio" id="portfolio">

  <div class="section-heading reveal">

    <div class="eyebrow">
      Selected Stories
    </div>

    <h2>
      Moments that<br>
      speak for themselves.
    </h2>

    <p>
      A glimpse into our visual storytelling.
    </p>

  </div>


  <div class="gallery">

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-1-URL" alt="Wedding Photography">
      <div class="gallery-overlay">
        <span>Wedding Story</span>
      </div>
    </div>

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-2-URL" alt="Indian Bride">
      <div class="gallery-overlay">
        <span>Bridal Portrait</span>
      </div>
    </div>

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-3-URL" alt="Wedding Couple">
      <div class="gallery-overlay">
        <span>The Couple</span>
      </div>
    </div>

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-4-URL" alt="Wedding Ceremony">
      <div class="gallery-overlay">
        <span>The Ceremony</span>
      </div>
    </div>

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-5-URL" alt="Indian Wedding">
      <div class="gallery-overlay">
        <span>Celebration</span>
      </div>
    </div>

    <div class="gallery-item reveal">
      <img src="YOUR-PHOTO-6-URL" alt="Wedding Couple Portrait">
      <div class="gallery-overlay">
        <span>Forever</span>
      </div>
    </div>

  </div>

</section>


<!-- =========================
     FEATURE
========================= -->

<section class="feature">

  <div class="feature-content reveal">

    <div class="eyebrow" style="color:#e5c995;">
      Because Every Love Story Is Different
    </div>

    <h2>
      We don't just<br>
      take photographs.
    </h2>

    <p>
      We preserve how it felt.
    </p>

    <a href="#contact" class="hero-btn">
      Let's Create Something Beautiful
    </a>

  </div>

</section>


<!-- =========================
     TESTIMONIAL
========================= -->

<section class="section testimonials">

  <div class="section-heading reveal">

    <div class="eyebrow">
      Kind Words
    </div>

    <h2>
      From our couples
    </h2>

  </div>

  <div class="testimonial-box reveal">

    <div class="quote">“</div>

    <div class="testimonial-text">
      Every photograph brought us back to the emotions
      of our wedding day. The moments were captured
      beautifully and naturally.
    </div>

    <div class="client">
      A Beautiful Wedding Story
    </div>

  </div>

</section>


<!-- =========================
     CONTACT CTA
========================= -->

<section class="cta" id="contact">

  <div class="reveal">

    <div class="eyebrow">
      Your Story Begins Here
    </div>

    <h2>
      Let's capture<br>
      your forever.
    </h2>

    <p>
      Tell us about your wedding, your vision and your story.
      We'd love to create something timeless for you.
    </p>

    <div class="cta-buttons">

      <!-- CHANGE NUMBER BELOW -->

      <a
      href="https://wa.me/91XXXXXXXXXX"
      target="_blank"
      class="btn">
        WhatsApp Us
      </a>

      <!-- CHANGE PHONE NUMBER BELOW -->

      <a
      href="tel:+91XXXXXXXXXX"
      class="btn btn-outline">
        Call Now
      </a>

    </div>

  </div>

</section>


<!-- =========================
     FOOTER
========================= -->

<footer>

  <div class="footer-grid">

    <div class="footer-brand">

      <h2>
        C2 CREATIONS
      </h2>

      <p>
        Luxury Wedding Photography & Cinematic Films.
        Creating timeless visual stories filled with
        emotion, elegance and love.
      </p>

    </div>


    <div>

      <div class="footer-title">
        Explore
      </div>

      <ul class="footer-links">

        <li><a href="#home">Home</a></li>

        <li><a href="#about">About</a></li>

        <li><a href="#services">Services</a></li>

        <li><a href="#portfolio">Portfolio</a></li>

        <li><a href="#contact">Contact</a></li>

      </ul>

    </div>


    <div>

      <div class="footer-title">
        Connect
      </div>

      <ul class="footer-links">

        <li>
          Varanasi & Beyond
        </li>

        <li>
          Wedding Photography
        </li>

        <li>
          Cinematic Films
        </li>

        <!-- CHANGE INSTAGRAM LINK -->

        <li>
          <a href="https://instagram.com/"
          target="_blank">
            Instagram
          </a>
        </li>

      </ul>

    </div>

  </div>


  <div class="footer-bottom">

    © 2026 C2 Creations Photography.
    All Rights Reserved.

  </div>

</footer>


<!-- =========================
     WHATSAPP FLOATING BUTTON
========================= -->

<a
href="https://wa.me/91XXXXXXXXXX"
target="_blank"
class="whatsapp"
aria-label="WhatsApp">
  ✆
</a>


<script>

/* =========================
   NAVBAR SCROLL
========================= */

window.addEventListener("scroll",function(){

  const navbar=document.getElementById("navbar");

  if(window.scrollY>50){
    navbar.classList.add("scrolled");
  }else{
    navbar.classList.remove("scrolled");
  }

});


/* =========================
   MOBILE MENU
========================= */

function toggleMenu(){

  document
  .getElementById("navLinks")
  .classList
  .toggle("active");

}


/* Close mobile menu after click */

document.querySelectorAll(".nav-links a").forEach(link=>{

  link.addEventListener("click",()=>{

    document
    .getElementById("navLinks")
    .classList
    .remove("active");

  });

});


/* =========================
   SCROLL REVEAL
========================= */

const reveals=document.querySelectorAll(".reveal");

const observer=new IntersectionObserver(

  entries=>{

    entries.forEach(entry=>{

      if(entry.isIntersecting){

        entry.target.classList.add("show");

      }

    });

  },

  {
    threshold:.12
  }

);


reveals.forEach(element=>{
  observer.observe(element);
});


/* =========================
   IMAGE ERROR FALLBACK
========================= */

document.querySelectorAll("img").forEach(img=>{

  img.addEventListener("error",function(){

    this.style.background=
      "linear-gradient(135deg,#641d2d,#c7a56a)";

    this.style.minHeight="250px";

  });

});

</script>

</body>
</html>
