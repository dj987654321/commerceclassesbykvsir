<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>COMMERCE CLASSES BY KV SIR</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
<header class="topbar">
  <div class="nav container">
    <a class="brand" href="index.html"><span class="brandMark">KV</span><span>COMMERCE CLASSES <b>BY KV SIR</b></span></a>
    <button class="menu" onclick="toggleMenu()">☰</button>
    <nav id="navLinks">
      <a class="active" href="index.html">HOME</a>
      <a href="courses.html">COURSES</a>
      <a href="#about">ABOUT</a>
      <a href="#gallery">GALLERY</a>
      <a href="#contact">CONTACT</a>
      <button class="navBtn" onclick="openAuth('login')">STUDENT LOGIN</button>
    </nav>
  </div>
</header>

<main>
<section class="hero">
  <div class="container heroGrid">
    <div class="heroCopy">
      <span class="eyebrow">SMART COMMERCE LEARNING</span>
      <h1>LEARN COMMERCE.<br><span>BUILD YOUR FUTURE.</span></h1>
      <p>Professional guidance for Class XI, Class XII, B.Com, BBA and MBA students with clear concepts, regular practice and doubt support.</p>
      <div class="actions">
        <a class="btn primary" href="courses.html">EXPLORE COURSES →</a>
        <button class="btn ghost" onclick="openAuth('signup')">CREATE STUDENT ACCOUNT</button>
      </div>
      <div class="heroStats">
        <div><strong>XI–XII</strong><small>CBSE / ICSE</small></div>
        <div><strong>B.COM</strong><small>COLLEGE</small></div>
        <div><strong>BBA / MBA</strong><small>MANAGEMENT</small></div>
      </div>
    </div>
    <div class="heroVisual">
      <img src="kv-sir-professional.jpg" alt="KV SIR">
      <div class="floatingCard"><b>KV SIR</b><span>COMMERCE EDUCATOR</span></div>
    </div>
  </div>
</section>

<section class="section" id="about">
  <div class="container twoCol">
    <div class="imageFrame"><img src="kv-sir-classroom.png" alt="KV SIR"></div>
    <div>
      <span class="eyebrow">ABOUT THE CLASSES</span>
      <h2>CONCEPTS FIRST. CONFIDENCE NEXT.</h2>
      <p class="lead">COMMERCE CLASSES BY KV SIR focuses on making commerce subjects easier to understand through structured lessons, examples, practice and student support.</p>
      <div class="featureList">
        <div><span>✓</span><b>INDIVIDUAL ATTENTION</b><small>Focused support for students.</small></div>
        <div><span>✓</span><b>SIMPLE TEACHING METHODS</b><small>Complex concepts explained clearly.</small></div>
        <div><span>✓</span><b>REGULAR TESTS & FEEDBACK</b><small>Practice, revision and progress checks.</small></div>
        <div><span>✓</span><b>DOUBT-CLEARING SESSIONS</b><small>Support when students need it.</small></div>
      </div>
    </div>
  </div>
</section>

<section class="section soft" id="courses">
  <div class="container">
    <div class="sectionHead">
      <span class="eyebrow">LEARNING PATHS</span>
      <h2>CHOOSE YOUR COURSE</h2>
      <p>CLICK ANY COURSE TO OPEN ITS DEDICATED COURSE PAGE.</p>
    </div>
    <div class="courseGrid">
      <a class="courseCard" href="course.html?course=class11"><span class="courseIcon">01</span><h3>CLASS XI</h3><p>ACCOUNTS • ECONOMICS • BUSINESS STUDIES</p><span class="learn">VIEW COURSE →</span></a>
      <a class="courseCard" href="course.html?course=class12"><span class="courseIcon">02</span><h3>CLASS XII</h3><p>ACCOUNTS • ECONOMICS • BUSINESS STUDIES</p><span class="learn">VIEW COURSE →</span></a>
      <a class="courseCard" href="course.html?course=bcom"><span class="courseIcon">03</span><h3>B.COM</h3><p>COMMERCE SUBJECTS • CONCEPT SUPPORT</p><span class="learn">VIEW COURSE →</span></a>
      <a class="courseCard" href="course.html?course=bba"><span class="courseIcon">04</span><h3>BBA</h3><p>BUSINESS • MANAGEMENT • COMMERCE</p><span class="learn">VIEW COURSE →</span></a>
      <a class="courseCard" href="course.html?course=mba"><span class="courseIcon">05</span><h3>MBA</h3><p>MANAGEMENT • BUSINESS • ACADEMIC SUPPORT</p><span class="learn">VIEW COURSE →</span></a>
    </div>
  </div>
</section>

<section class="section">
  <div class="container portal">
    <div>
      <span class="eyebrow">STUDENT PORTAL</span>
      <h2>ONE ACCOUNT FOR YOUR LEARNING</h2>
      <p class="lead">Create a student account to keep your profile, selected course and learning dashboard in one place.</p>
      <button class="btn primary" onclick="openAuth('signup')">CREATE ACCOUNT</button>
      <button class="btn light" onclick="openAuth('login')">SIGN IN</button>
    </div>
    <div class="portalMock">
      <div class="mockTop"><span>STUDENT DASHBOARD</span><i>●</i></div>
      <div class="mockBody"><div class="avatar">S</div><div><b>MY LEARNING</b><small>COURSES • PROFILE • SUPPORT</small></div></div>
      <div class="mockRows"><span>MY COURSES</span><span>›</span><span>MY PROFILE</span><span>›</span><span>SUPPORT</span><span>›</span></div>
    </div>
  </div>
</section>

<section class="section soft" id="gallery">
  <div class="container">
    <div class="sectionHead"><span class="eyebrow">GALLERY</span><h2>COMMERCE CLASSES BY KV SIR</h2></div>
    <div class="galleryGrid">
      <div class="galleryItem wide"><img src="commerce-classes-poster.png" alt="COMMERCE CLASSES BY KV SIR POSTER"><div class="galleryCaption">COURSE INFORMATION & CLASS DETAILS</div></div>
      <div class="galleryItem"><img src="kv-sir-professional.jpg" alt="KV SIR"><div class="galleryCaption">KV SIR</div></div>
      <div class="galleryItem"><img src="kv-sir-classroom.png" alt="KV SIR"><div class="galleryCaption">LEARNING & GUIDANCE</div></div>
    </div>
  </div>
</section>

<section class="section" id="contact">
  <div class="container contact">
    <div>
      <span class="eyebrow">CONTACT</span>
      <h2>START YOUR COMMERCE JOURNEY</h2>
      <p class="lead">ANAND NAGAR, BAHODAPUR, GWALIOR</p>
      <div class="contactCards">
        <a href="tel:7987116714"><b>PHONE</b><span>7987116714</span></a>
        <a href="https://wa.me/917987116714" target="_blank"><b>WHATSAPP</b><span>SEND AN ENQUIRY</span></a>
      </div>
    </div>
    <form class="contactForm" onsubmit="sendWhatsApp(event)">
      <h3>QUICK ENQUIRY</h3>
      <input id="qName" placeholder="STUDENT NAME" required>
      <input id="qPhone" placeholder="PHONE NUMBER" required>
      <select id="qCourse" required><option value="">SELECT COURSE</option><option>CLASS XI</option><option>CLASS XII</option><option>B.COM</option><option>BBA</option><option>MBA</option></select>
      <textarea id="qMessage" placeholder="YOUR MESSAGE" required></textarea>
      <button class="btn primary">SEND ON WHATSAPP</button>
    </form>
  </div>
</section>
</main>

<footer><div class="container footerFlex"><div><b>COMMERCE CLASSES BY KV SIR</b><small>ANAND NAGAR, BAHODAPUR, GWALIOR</small></div><div>© 2026 COMMERCE CLASSES BY KV SIR</div></div></footer>

<div class="modal" id="authModal">
  <div class="authBox">
    <button class="close" onclick="closeAuth()">×</button>
    <div class="authBrand">KV</div>
    <h2 id="authTitle">STUDENT SIGN IN</h2>
    <p id="authSub">ACCESS YOUR STUDENT PORTAL</p>
    <div class="tabs"><button id="tabLogin" class="active" onclick="setAuth('login')">SIGN IN</button><button id="tabSignup" onclick="setAuth('signup')">CREATE ACCOUNT</button></div>
    <form onsubmit="authSubmit(event)">
      <input id="authName" placeholder="FULL NAME" style="display:none">
      <input id="authEmail" type="email" placeholder="EMAIL ADDRESS" required>
      <input id="authPassword" type="password" placeholder="PASSWORD" minlength="6" required>
      <button class="btn primary full" id="authButton">SIGN IN</button>
    </form>
    <small class="demoNote">DEMO ACCOUNT SYSTEM FOR GITHUB PAGES. FOR PRODUCTION USE, CONNECT FIREBASE/SUPABASE AUTHENTICATION.</small>
  </div>
</div>

<script src="app.js"></script>
</body>
</html>
