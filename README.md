<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Commerce Classes by KV Sir</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #07111f;
      color: #fff;
      line-height: 1.6;
    }

    header {
      position: fixed;
      top: 0;
      width: 100%;
      z-index: 1000;
      background: rgba(7,17,31,0.95);
      border-bottom: 1px solid #1b314b;
    }

    nav {
      max-width: 1200px;
      margin: auto;
      padding: 18px 25px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      font-size: 22px;
      font-weight: 800;
      color: #20d9ff;
    }

    .logo span {
      color: #fff;
    }

    nav ul {
      display: flex;
      list-style: none;
      gap: 28px;
    }

    nav a {
      color: #fff;
      text-decoration: none;
      font-weight: 600;
    }

    nav a:hover {
      color: #20d9ff;
    }

    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      text-align: center;
      padding: 120px 20px 70px;
      background:
        radial-gradient(circle at center, #12375a 0%, #07111f 55%);
    }

    .hero-content {
      max-width: 900px;
    }

    .hero h1 {
      font-size: clamp(42px, 7vw, 82px);
      line-height: 1.05;
      margin-bottom: 20px;
    }

    .hero h1 span {
      color: #20d9ff;
    }

    .hero p {
      font-size: 20px;
      color: #c7d5e5;
      margin-bottom: 35px;
    }

    .btn {
      display: inline-block;
      padding: 14px 28px;
      margin: 6px;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 700;
      background: #20d9ff;
      color: #03101c;
      border: 2px solid #20d9ff;
      cursor: pointer;
    }

    .btn:hover {
      background: transparent;
      color: #20d9ff;
    }

    .btn-outline {
      background: transparent;
      color: #20d9ff;
    }

    section {
      padding: 90px 20px;
    }

    .container {
      max-width: 1150px;
      margin: auto;
    }

    .section-title {
      text-align: center;
      margin-bottom: 50px;
    }

    .section-title h2 {
      font-size: 42px;
      margin-bottom: 10px;
    }

    .section-title p {
      color: #9fb2c7;
    }

    .about {
      background: #0b1929;
    }

    .about-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 40px;
      align-items: center;
    }

    .about-box {
      padding: 35px;
      background: #102238;
      border: 1px solid #1c3a57;
      border-radius: 15px;
    }

    .about-box h3 {
      color: #20d9ff;
      font-size: 27px;
      margin-bottom: 15px;
    }

    .about-box p {
      color: #c3d1df;
    }

    .courses {
      background: #07111f;
    }

    .course-grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .course {
      background: #0e2035;
      border: 1px solid #1c3a57;
      border-radius: 15px;
      padding: 30px;
      transition: 0.3s;
    }

    .course:hover {
      transform: translateY(-8px);
      border-color: #20d9ff;
      box-shadow: 0 10px 30px rgba(32,217,255,0.12);
    }

    .course h3 {
      color: #20d9ff;
      margin-bottom: 12px;
      font-size: 24px;
    }

    .course p {
      color: #b8c8d8;
      margin-bottom: 20px;
    }

    .portal {
      background: #0b1929;
    }

    .portal-box {
      max-width: 600px;
      margin: auto;
      background: #102238;
      padding: 35px;
      border-radius: 15px;
      border: 1px solid #1c3a57;
    }

    input {
      width: 100%;
      padding: 14px;
      margin: 8px 0;
      background: #07111f;
      border: 1px solid #31506d;
      color: #fff;
      border-radius: 7px;
      outline: none;
    }

    input:focus {
      border-color: #20d9ff;
    }

    .contact {
      background: #07111f;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 30px;
    }

    .contact-box {
      background: #0e2035;
      padding: 30px;
      border-radius: 15px;
      border: 1px solid #1c3a57;
    }

    .contact-box h3 {
      color: #20d9ff;
      margin-bottom: 15px;
    }

    .contact-box p {
      color: #c5d3df;
      margin: 8px 0;
    }

    footer {
      text-align: center;
      padding: 25px;
      background: #030a12;
      color: #8da2b8;
      border-top: 1px solid #172b40;
    }

    .quote {
      text-align: center;
      font-size: 30px;
      font-weight: 700;
      color: #20d9ff;
      margin-top: 35px;
    }

    .mobile-menu {
      display: none;
      font-size: 28px;
      cursor: pointer;
      color: #20d9ff;
    }

    @media (max-width: 800px) {
      nav ul {
        display: none;
        position: absolute;
        top: 70px;
        left: 0;
        width: 100%;
        background: #07111f;
        flex-direction: column;
        text-align: center;
        padding: 20px;
      }

      nav ul.active {
        display: flex;
      }

      .mobile-menu {
        display: block;
      }

      .about-grid,
      .contact-grid {
        grid-template-columns: 1fr;
      }

      .course-grid {
        grid-template-columns: 1fr;
      }
    }
  </style>
</head>

<body>

<header>
  <nav>
    <div class="logo">COMMERCE <span>CLASSES</span></div>

    <div class="mobile-menu" onclick="toggleMenu()">☰</div>

    <ul id="navMenu">
      <li><a href="#home">Home</a></li>
      <li><a href="#about">About</a></li>
      <li><a href="#courses">Courses</a></li>
      <li><a href="#portal">Student Portal</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</header>

<section class="hero" id="home">
  <div class="hero-content">
    <h1>LEARN TODAY.<br><span>LEAD TOMORROW.</span></h1>

    <p>
      Welcome to <strong>Commerce Classes by KV Sir</strong> —
      build strong concepts, develop confidence and create your future.
    </p>

    <a href="#courses" class="btn">Explore Courses</a>
    <a href="#contact" class="btn btn-outline">Contact Us</a>

    <div class="quote">
      "Your Success Begins With The Right Knowledge."
    </div>
  </div>
</section>

<section class="about" id="about">
  <div class="container">

    <div class="section-title">
      <h2>About KV Sir</h2>
      <p>Learn with concepts. Grow with confidence.</p>
    </div>

    <div class="about-grid">

      <div class="about-box">
        <h3>Concept Based Learning</h3>
        <p>
          We focus on understanding concepts instead of simply memorizing
          answers. Our goal is to make Commerce simple, practical and
          interesting.
        </p>
      </div>

      <div class="about-box">
        <h3>Build Your Future</h3>
        <p>
          From school-level Commerce to professional education, students
          receive structured learning to prepare for their academic and
          professional journey.
        </p>
      </div>

    </div>
  </div>
</section>

<section class="courses" id="courses">
  <div class="container">

    <div class="section-title">
      <h2>Our Courses</h2>
      <p>Choose your path and start learning.</p>
    </div>

    <div class="course-grid">

      <div class="course">
        <h3>Class XI</h3>
        <p>
          Build a strong foundation in Accountancy, Business Studies,
          Economics and Commerce.
        </p>
        <button class="btn" onclick="showCourse('Class XI')">
          View Details
        </button>
      </div>

      <div class="course">
        <h3>Class XII</h3>
        <p>
          Strengthen concepts and prepare systematically for board
          examinations.
        </p>
        <button class="btn" onclick="showCourse('Class XII')">
          View Details
        </button>
      </div>

      <div class="course">
        <h3>B.Com</h3>
        <p>
          Develop a deeper understanding of commerce, accounting,
          business and economics.
        </p>
        <button class="btn" onclick="showCourse('B.Com')">
          View Details
        </button>
      </div>

      <div class="course">
        <h3>BBA</h3>
        <p>
          Learn business fundamentals, management concepts and practical
          decision-making skills.
        </p>
        <button class="btn" onclick="showCourse('BBA')">
          View Details
        </button>
      </div>

      <div class="course">
        <h3>MBA</h3>
        <p>
          Develop advanced management and business knowledge for higher
          education and career growth.
        </p>
        <button class="btn" onclick="showCourse('MBA')">
          View Details
        </button>
      </div>

      <div class="course">
        <h3>Personal Guidance</h3>
        <p>
          Get structured academic guidance and support according to your
          learning requirements.
        </p>
        <button class="btn" onclick="contactNow()">
          Enquire Now
        </button>
      </div>

    </div>
  </div>
</section>

<section class="portal" id="portal">
  <div class="container">

    <div class="section-title">
      <h2>Student Portal</h2>
      <p>Login or create your student account.</p>
    </div>

    <div class="portal-box">

      <input type="text" id="studentName" placeholder="Student Name">

      <input type="email" id="studentEmail" placeholder="Email Address">

      <input type="password" id="studentPassword" placeholder="Password">

      <button class="btn" onclick="signup()">Create Account</button>

      <button class="btn btn-outline" onclick="login()">Login</button>

      <p id="portalMessage" style="margin-top:15px;color:#20d9ff;"></p>

    </div>
  </div>
</section>

<section class="contact" id="contact">
  <div class="container">

    <div class="section-title">
      <h2>Contact Us</h2>
      <p>Start your learning journey today.</p>
    </div>

    <div class="contact-grid">

      <div class="contact-box">
        <h3>Commerce Classes by KV Sir</h3>

        <p>📍 Anand Nagar, Bahodapur, Gwalior</p>

        <p>
          📞
          <a
            href="tel:7987116714"
            style="color:#20d9ff;text-decoration:none;"
          >
            7987116714
          </a>
        </p>

        <p>📚 Class XI | Class XII | B.Com | BBA | MBA</p>

        <a
          class="btn"
          href="https://wa.me/917987116714?text=Hello%20KV%20Sir,%20I%20want%20information%20about%20your%20Commerce%20Classes."
          target="_blank"
        >
          WhatsApp Us
        </a>
      </div>

      <div class="contact-box">
        <h3>Send an Enquiry</h3>

        <input
          type="text"
          id="contactName"
          placeholder="Your Name"
        >

        <input
          type="text"
          id="contactCourse"
          placeholder="Course / Class"
        >

        <input
          type="text"
          id="contactMessage"
          placeholder="Your Message"
        >

        <button class="btn" onclick="sendWhatsApp()">
          Send Enquiry
        </button>
      </div>

    </div>
  </div>
</section>

<footer>
  © 2026 Commerce Classes by KV Sir | Anand Nagar, Bahodapur, Gwalior
</footer>

<script>

  function toggleMenu() {
    document.getElementById("navMenu").classList.toggle("active");
  }

  function showCourse(course) {
    alert(
      course +
      " course selected.\n\n" +
      "For admission, fees and batch details, please contact KV Sir on WhatsApp: 7987116714"
    );
  }

  function contactNow() {
    window.open(
      "https://wa.me/917987116714?text=Hello%20KV%20Sir,%20I%20want%20information%20about%20admission.",
      "_blank"
    );
  }

  function signup() {

    const name = document.getElementById("studentName").value;
    const email = document.getElementById("studentEmail").value;
    const password = document.getElementById("studentPassword").value;

    if (!name || !email || !password) {
      document.getElementById("portalMessage").innerText =
        "Please fill all fields.";
      return;
    }

    localStorage.setItem(
      "kvStudent",
      JSON.stringify({
        name: name,
        email: email,
        password: password
      })
    );

    document.getElementById("portalMessage").innerText =
      "Account created successfully!";
  }

  function login() {

    const email = document.getElementById("studentEmail").value;
    const password = document.getElementById("studentPassword").value;

    const student = JSON.parse(
      localStorage.getItem("kvStudent")
    );

    if (
      student &&
      student.email === email &&
      student.password === password
    ) {
      document.getElementById("portalMessage").innerText =
        "Welcome " + student.name + "! Login successful.";
    } else {
      document.getElementById("portalMessage").innerText =
        "Invalid email or password.";
    }
  }

  function sendWhatsApp() {

    const name =
      document.getElementById("contactName").value;

    const course =
      document.getElementById("contactCourse").value;

    const message =
      document.getElementById("contactMessage").value;

    if (!name || !course || !message) {
      alert("Please fill all enquiry fields.");
      return;
    }

    const text =
      "Hello KV Sir,%0A%0A" +
      "Name: " + encodeURIComponent(name) + "%0A" +
      "Course: " + encodeURIComponent(course) + "%0A" +
      "Message: " + encodeURIComponent(message);

    window.open(
      "https://wa.me/917987116714?text=" + text,
      "_blank"
    );
  }

</script>

</body>
</html>
