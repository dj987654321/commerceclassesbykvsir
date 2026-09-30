```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>COMMERCE CLASSES BY KV SIR</title>

<link rel="stylesheet" href="style.css">

<style>
/* ================================
   HOMEPAGE IMPROVEMENTS
================================ */

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: Arial, Helvetica, sans-serif;
  background: #f7f9fc;
  color: #111827;
}

/* NAVIGATION */

.topbar {
  position: sticky;
  top: 0;
  z-index: 1000;
  background: rgba(255,255,255,0.96);
  border-bottom: 1px solid #e5e7eb;
  backdrop-filter: blur(12px);
}

.container {
  width: min(1180px, 92%);
  margin: auto;
}

.nav {
  min-height: 78px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.brand {
  display: flex;
  align-items: center;
  gap: 12px;
  text-decoration: none;
  color: #111827;
  font-weight: 800;
  letter-spacing: .5px;
}

.brand b {
  color: #2563eb;
}

.brandMark {
  width: 45px;
  height: 45px;
  display: grid;
  place-items: center;
  border-radius: 14px;
  background: linear-gradient(135deg,#2563eb,#7c3aed);
  color: white;
  font-weight: 900;
  box-shadow: 0 10px 25px rgba(37,99,235,.25);
}

#navLinks {
  display: flex;
  align-items: center;
  gap: 25px;
}

#navLinks a {
  text-decoration: none;
  color: #374151;
  font-weight: 700;
  font-size: 14px;
}

#navLinks a:hover,
#navLinks a.active {
  color: #2563eb;
}

.navBtn {
  border: none;
  padding: 12px 18px;
  border-radius: 10px;
  background: #111827;
  color: white;
  font-weight: 800;
  cursor: pointer;
}

.menu {
  display: none;
  border: none;
  background: transparent;
  font-size: 28px;
}

/* HERO */

.hero {
  position: relative;
  overflow: hidden;
  padding: 90px 0 100px;
  background:
    radial-gradient(circle at 80% 20%, rgba(37,99,235,.16), transparent 30%),
    radial-gradient(circle at 15% 80%, rgba(124,58,237,.12), transparent 28%),
    linear-gradient(135deg,#f8fbff,#eef4ff);
}

.heroGrid {
  display: grid;
  grid-template-columns: 1.1fr .9fr;
  gap: 60px;
  align-items: center;
}

.eyebrow {
  display: inline-block;
  color: #2563eb;
  font-weight: 900;
  font-size: 13px;
  letter-spacing: 2px;
  margin-bottom: 15px;
}

.hero h1 {
  font-size: clamp(42px,6vw,78px);
  line-height: .98;
  margin: 0 0 25px;
  font-weight: 950;
  letter-spacing: -3px;
}

.hero h1 span {
  color: #2563eb;
}

.hero p {
  max-width: 650px;
  font-size: 19px;
  line-height: 1.7;
  color: #4b5563;
}

.actions {
  display: flex;
  flex-wrap: wrap;
  gap: 14px;
  margin-top: 30px;
}

.btn {
  border: none;
  border-radius: 12px;
  padding: 15px 22px;
  font-weight: 900;
  cursor: pointer;
  text-decoration: none;
  display: inline-block;
}

.primary {
  background: #2563eb;
  color: white;
  box-shadow: 0 12px 25px rgba(37,99,235,.25);
}

.primary:hover {
  transform: translateY(-2px);
}

.ghost {
  background: white;
  color: #111827;
  border: 1px solid #dbe3ef;
}

.heroStats {
  display: flex;
  flex-wrap: wrap;
  gap: 35px;
  margin-top: 45px;
}

.heroStats div {
  display: flex;
  flex-direction: column;
  gap: 5px;
}

.heroStats strong {
  font-size: 20px;
}

.heroStats small {
  color: #6b7280;
}

/* HERO IMAGE */

.heroVisual {
  position: relative;
  text-align: center;
}

.heroVisual img {
  width: min(420px,100%);
  height: 500px;
  object-fit: cover;
  border-radius: 35px;
  box-shadow: 0 30px 70px rgba(15,23,42,.20);
  border: 8px solid white;
}

.floatingCard {
  position: absolute;
  left: 20px;
  bottom: 35px;
  background: white;
  padding: 18px 24px;
  border-radius: 16px;
  box-shadow: 0 15px 40px rgba(15,23,42,.15);
  text-align: left;
}

.floatingCard b {
  display: block;
  font-size: 18px;
}

.floatingCard span {
  color: #6b7280;
  font-size: 12px;
}

/* INSPIRATION */

.inspiration {
  padding: 90px 0;
  background: #111827;
  color: white;
  text-align: center;
}

.inspiration h2 {
  max-width: 850px;
  margin: auto;
  font-size: clamp(30px,5vw,55px);
  line-height: 1.15;
}

.inspiration p {
  max-width: 700px;
  margin: 22px auto 0;
  color: #cbd5e1;
  font-size: 18px;
  line-height: 1.7;
}

.quoteMark {
  font-size: 70px;
  color: #60a5fa;
  line-height: .5;
  margin-bottom: 25px;
}

/* ABOUT */

.section {
  padding: 90px 0;
}

.soft {
  background: #f1f5f9;
}

.twoCol {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
  align-items: center;
}

.imageFrame img {
  width: 100%;
  max-height: 550px;
  object-fit: cover;
  border-radius: 28px;
  box-shadow: 0 25px 60px rgba(15,23,42,.12);
}

.section h2 {
  font-size: clamp(30px,4vw,48px);
  margin: 0 0 20px;
  line-height: 1.1;
}

.lead {
  font-size: 17px;
  line-height: 1.8;
  color: #5b6472;
}

.featureList {
  display: grid;
  gap: 16px;
  margin-top: 30px;
}

.featureList div {
  display: grid;
  grid-template-columns: 35px 1fr;
  column-gap: 10px;
}

.featureList span {
  grid-row: span 2;
  width: 30px;
  height: 30px;
  display: grid;
  place-items: center;
  background: #dbeafe;
  color: #2563eb;
  border-radius: 50%;
  font-weight: 900;
}

.featureList b {
  font-size: 14px;
}

.featureList small {
  color: #6b7280;
  margin-top: 3px;
}

/* STUDENT PROFILE */

.profileSection {
  padding: 100px 0;
  background:
    radial-gradient(circle at center, rgba(37,99,235,.10), transparent 40%),
    #f8fafc;
}

.profileCenter {
  max-width: 850px;
  margin: auto;
  text-align: center;
}

.profileCenter h2 {
  margin-bottom: 15px;
}

.profileCard {
  margin: 35px auto 0;
  max-width: 650px;
  background: white;
  border-radius: 28px;
  padding: 40px;
  box-shadow: 0 25px 70px rgba(15,23,42,.12);
  border: 1px solid #e5e7eb;
}

.profileAvatar {
  width: 90px;
  height: 90px;
  margin: auto;
  display: grid;
  place-items: center;
  border-radius: 50%;
  background: linear-gradient(135deg,#2563eb,#7c3aed);
  color: white;
  font-size: 32px;
  font-weight: 900;
}

.profileCard h3 {
  margin: 20px 0 8px;
  font-size: 25px;
}

.profileCard p {
  color: #6b7280;
  margin-bottom: 25px;
}

.profileButtons {
  display: flex;
  justify-content: center;
  gap: 12px;
  flex-wrap: wrap;
}

/* CONTACT */

.contact {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 60px;
  align-items: start;
}

.contactCards {
  display: flex;
  gap: 15px;
  flex-wrap: wrap;
  margin-top: 25px;
}

.contactCards a {
  min-width: 190px;
  padding: 18px;
  border-radius: 15px;
  background: #f1f5f9;
  text-decoration: none;
  color: #111827;
}

.contactCards b,
.contactCards span {
  display: block;
}

.contactCards span {
  margin-top: 6px;
  color: #2563eb;
}

.contactForm {
  background: white;
  padding: 30px;
  border-radius: 25px;
  box-shadow: 0 20px 50px rgba(15,23,42,.10);
}

.contactForm h3 {
  margin-top: 0;
}

.contactForm input,
.contactForm select,
.contactForm textarea {
  width: 100%;
  padding: 14px;
  margin: 7px 0;
  border: 1px solid #dbe3ef;
  border-radius: 10px;
  font: inherit;
}

.contactForm textarea {
  min-height: 120px;
  resize: vertical;
}

/* FOOTER */

footer {
  background: #0f172a;
  color: white;
  padding: 30px 0;
}

.footerFlex {
  display: flex;
  justify-content: space-between;
  gap: 20px;
  align-items: center;
}

.footerFlex small {
  display: block;
  color: #94a3b8;
  margin-top: 6px;
}

/* MOBILE */

@media(max-width:800px) {

  #navLinks {
    display: none;
    position: absolute;
    top: 78px;
    left: 0;
    right: 0;
    background: white;
    padding: 20px;
    flex-direction: column;
    box-shadow: 0 15px 30px rgba(0,0,0,.1);
  }

  #navLinks.show {
    display: flex;
  }

  .menu {
    display: block;
  }

  .heroGrid,
  .twoCol,
  .contact {
    grid-template-columns: 1fr;
  }

  .hero {
    padding-top: 55px;
  }

  .heroVisual {
    order: -1;
  }

  .heroVisual img {
    height: 420px;
  }

  .heroStats {
    gap: 20px;
  }

  .footerFlex {
    flex-direction: column;
    text-align: center;
  }
}
</style>
</head>

<body>

<!-- ================================
     NAVIGATION
================================ -->

<header class="topbar">

  <div class="nav container">

    <a class="brand" href="index.html">
      <span class="brandMark">KV</span>

      <span>
        COMMERCE CLASSES
        <b>BY KV SIR</b>
      </span>
    </a>

    <button class="menu" onclick="toggleMenu()">☰</button>

    <nav id="navLinks">

      <a class="active" href="index.html">HOME</a>

      <a href="#about">ABOUT</a>

      <a href="#profile">PROFILE</a>

      <a href="#contact">CONTACT</a>

      <button
        class="navBtn"
        onclick="openAuth('login')">
        STUDENT LOGIN
      </button>

    </nav>

  </div>

</header>


<main>

<!-- ================================
     INSPIRATIONAL HERO
================================ -->

<section class="hero">

  <div class="container heroGrid">

    <div class="heroCopy">

      <span class="eyebrow">
        SMART COMMERCE LEARNING
      </span>

      <h1>
        LEARN TODAY.
        <br>
        <span>LEAD TOMORROW.</span>
      </h1>

      <p>
        Welcome to COMMERCE CLASSES BY KV SIR —
        a place where concepts become clear,
        confidence grows and students prepare
        themselves for a brighter future.
      </p>

      <div class="actions">

        <a
          class="btn primary"
          href="#about">
          START YOUR JOURNEY →
        </a>

        <button
          class="btn ghost"
          onclick="openAuth('signup')">
          CREATE STUDENT ACCOUNT
        </button>

      </div>

      <div class="heroStats">

        <div>
          <strong>XI–XII</strong>
          <small>CBSE / ICSE</small>
        </div>

        <div>
          <strong>B.COM</strong>
          <small>COLLEGE</small>
        </div>

        <div>
          <strong>BBA / MBA</strong>
          <small>MANAGEMENT</small>
        </div>

      </div>

    </div>


    <div class="heroVisual">

      <img
        src="kv-sir-professional.jpg"
        alt="KV SIR">

      <div class="floatingCard">

        <b>KV SIR</b>

        <span>
          COMMERCE EDUCATOR
        </span>

      </div>

    </div>

  </div>

</section>


<!-- ================================
     INSPIRATIONAL MESSAGE
================================ -->

<section class="inspiration">

  <div class="container">

    <div class="quoteMark">
      “
    </div>

    <h2>
      YOUR DREAMS DESERVE
      <br>
      YOUR BEST EFFORT.
    </h2>

    <p>
      Success is not built in one day.
      It is built through consistent learning,
      discipline, practice and the courage
      to keep improving every day.
    </p>

  </div>

</section>


<!-- ================================
     ABOUT
================================ -->

<section
  class="section"
  id="about">

  <div class="container twoCol">

    <div class="imageFrame">

      <img
        src="kv-sir-classroom.png"
        alt="KV SIR teaching">

    </div>


    <div>

      <span class="eyebrow">
        ABOUT THE CLASSES
      </span>

      <h2>
        CONCEPTS FIRST.
        <br>
        CONFIDENCE NEXT.
      </h2>

      <p class="lead">

        COMMERCE CLASSES BY KV SIR focuses
        on making commerce subjects easier
        to understand through structured lessons,
        examples, practice and student support.

      </p>


      <div class="featureList">

        <div>
          <span>✓</span>
          <b>INDIVIDUAL ATTENTION</b>
          <small>
            Focused support for students.
          </small>
        </div>

        <div>
          <span>✓</span>
          <b>SIMPLE TEACHING METHODS</b>
          <small>
            Complex concepts explained clearly.
          </small>
        </div>

        <div>
          <span>✓</span>
          <b>REGULAR TESTS & FEEDBACK</b>
          <small>
            Practice, revision and progress checks.
          </small>
        </div>

        <div>
          <span>✓</span>
          <b>DOUBT-CLEARING SESSIONS</b>
          <small>
            Support when students need it.
          </small>
        </div>

      </div>

    </div>

  </div>

</section>


<!-- ================================
     CENTERED STUDENT PROFILE
================================ -->

<section
  class="profileSection"
  id="profile">

  <div class="container profileCenter">

    <span class="eyebrow">
      STUDENT PROFILE
    </span>

    <h2>
      YOUR LEARNING.
      <br>
      YOUR PROFILE.
    </h2>

    <p class="lead">
      Create your personal student account
      and keep your learning journey organized
      in one place.
    </p>


    <div class="profileCard">

      <div class="profileAvatar">
        KV
      </div>

      <h3>
        STUDENT PORTAL
      </h3>

      <p>
        Manage your account, learning information
        and student support.
      </p>


      <div class="profileButtons">

        <button
          class="btn primary"
          onclick="openAuth('login')">
          SIGN IN
        </button>

        <button
          class="btn ghost"
          onclick="openAuth('signup')">
          CREATE ACCOUNT
        </button>

      </div>

    </div>

  </div>

</section>


<!-- ================================
     CONTACT
================================ -->

<section
  class="section soft"
  id="contact">

  <div class="container contact">

    <div>

      <span class="eyebrow">
        CONTACT
      </span>

      <h2>
        START YOUR
        <br>
        COMMERCE JOURNEY
      </h2>

      <p class="lead">
        ANAND NAGAR, BAHODAPUR, GWALIOR
      </p>


      <div class="contactCards">

        <a href="tel:7987116714">

          <b>PHONE</b>

          <span>
            7987116714
          </span>

        </a>


        <a
          href="https://wa.me/917987116714"
          target="_blank">

          <b>WHATSAPP</b>

          <span>
            SEND AN ENQUIRY
          </span>

        </a>

      </div>

    </div>


    <form
      class="contactForm"
      onsubmit="sendWhatsApp(event)">

      <h3>
        QUICK ENQUIRY
      </h3>

      <input
        id="qName"
        placeholder="STUDENT NAME"
        required>

      <input
        id="qPhone"
        placeholder="PHONE NUMBER"
        required>

      <select
        id="qCourse"
        required>

        <option value="">
          SELECT COURSE
        </option>

        <option>
          CLASS XI
        </option>

        <option>
          CLASS XII
        </option>

        <option>
          B.COM
        </option>

        <option>
          BBA
        </option>

        <option>
          MBA
        </option>

      </select>

      <textarea
        id="qMessage"
        placeholder="YOUR MESSAGE"
        required></textarea>

      <button class="btn primary">
        SEND ON WHATSAPP
      </button>

    </form>

  </div>

</section>

</main>


<!-- ================================
     FOOTER
================================ -->

<footer>

  <div class="container footerFlex">

    <div>

      <b>
        COMMERCE CLASSES BY KV SIR
      </b>

      <small>
        ANAND NAGAR, BAHODAPUR, GWALIOR
      </small>

    </div>

    <div>
      © 2026 COMMERCE CLASSES BY KV SIR
    </div>

  </div>

</footer>


<!-- ================================
     LOGIN / SIGNUP MODAL
================================ -->

<div
  class="modal"
  id="authModal">

  <div class="authBox">

    <button
      class="close"
      onclick="closeAuth()">
      ×
    </button>

    <div class="authBrand">
      KV
    </div>

    <h2 id="authTitle">
      STUDENT SIGN IN
    </h2>

    <p id="authSub">
      ACCESS YOUR STUDENT PORTAL
    </p>


    <div class="tabs">

      <button
        id="tabLogin"
        class="active"
        onclick="setAuth('login')">
        SIGN IN
      </button>

      <button
        id="tabSignup"
        onclick="setAuth('signup')">
        CREATE ACCOUNT
      </button>

    </div>


    <form onsubmit="authSubmit(event)">

      <input
        id="authName"
        placeholder="FULL NAME"
        style="display:none">

      <input
        id="authEmail"
        type="email"
        placeholder="EMAIL ADDRESS"
        required>

      <input
        id="authPassword"
        type="password"
        placeholder="PASSWORD"
        minlength="6"
        required>

      <button
        class="btn primary full"
        id="authButton">
        SIGN IN
      </button>

    </form>

    <small class="demoNote">

      DEMO ACCOUNT SYSTEM FOR GITHUB PAGES.
      FOR PRODUCTION USE, CONNECT FIREBASE
      OR SUPABASE AUTHENTICATION.

    </small>

  </div>

</div>


<script src="app.js"></script>

</body>
</html>
```
