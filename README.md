<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050b16">
<title>Commerce Classes by KV Sir</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    width:100%;
    min-width:100%;
    scroll-behavior:smooth;
}

body{
    width:100%;
    min-width:100%;
    overflow-x:hidden;
    font-family:Arial,Helvetica,sans-serif;
    background:#050b16;
    color:#fff;
}

/* ================= HEADER ================= */

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:9999;
    background:rgba(3,9,18,.82);
    backdrop-filter:blur(16px);
    border-bottom:1px solid rgba(32,217,255,.12);
}

.navbar{
    width:100%;
    height:78px;
    padding:0 5%;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
    color:#fff;
    font-size:17px;
    font-weight:800;
    white-space:nowrap;
}

.logo-box{
    width:44px;
    height:44px;
    border-radius:12px;
    display:flex;
    align-items:center;
    justify-content:center;
    background:#20d9ff;
    color:#06111d;
    font-weight:900;
    box-shadow:0 0 25px rgba(32,217,255,.4);
}

.logo span{
    color:#20d9ff;
}

.nav-links{
    list-style:none;
    display:flex;
    align-items:center;
    gap:30px;
}

.nav-links a{
    text-decoration:none;
    color:#fff;
    font-size:14px;
    font-weight:700;
    transition:.3s;
}

.nav-links a:hover{
    color:#20d9ff;
    text-shadow:0 0 12px #20d9ff;
}

.login-btn{
    background:#20d9ff;
    color:#03101a!important;
    padding:13px 21px;
    border-radius:9px;
    box-shadow:0 0 20px rgba(32,217,255,.25);
}

.login-btn:hover{
    background:#fff;
    color:#03101a!important;
}

/* ================= MOBILE MENU ================= */

.menu-btn{
    display:none;
    font-size:30px;
    color:#20d9ff;
    cursor:pointer;
}

/* ================= HERO ================= */

.hero{
    position:relative;
    width:100%;
    min-height:100vh;
    min-height:100svh;

    display:flex;
    align-items:center;
    justify-content:center;

    padding:120px 20px 70px;

    overflow:hidden;

    background:
        radial-gradient(
            circle at 50% 50%,
            rgba(0,109,255,.28) 0%,
            rgba(0,46,100,.15) 30%,
            #07111f 65%,
            #020711 100%
        );
}

/* Animated light */

.hero::before{
    content:"";
    position:absolute;
    width:650px;
    height:650px;
    border-radius:50%;

    background:radial-gradient(
        circle,
        rgba(32,217,255,.16),
        transparent 68%
    );

    left:50%;
    top:50%;

    transform:translate(-50%,-50%);

    animation:pulseGlow 5s ease-in-out infinite;

    pointer-events:none;
}

.hero::after{
    content:"";
    position:absolute;
    inset:0;

    background:
        linear-gradient(
            120deg,
            transparent 35%,
            rgba(32,217,255,.05),
            transparent 65%
        );

    animation:shine 7s linear infinite;
    pointer-events:none;
}

@keyframes pulseGlow{
    0%,100%{
        transform:translate(-50%,-50%) scale(1);
        opacity:.65;
    }

    50%{
        transform:translate(-50%,-50%) scale(1.25);
        opacity:1;
    }
}

@keyframes shine{
    0%{
        transform:translateX(-100%);
    }

    100%{
        transform:translateX(100%);
    }
}

/* ================= PARTICLES ================= */

.particle{
    position:absolute;
    width:4px;
    height:4px;
    border-radius:50%;
    background:#20d9ff;
    box-shadow:0 0 12px #20d9ff;
    opacity:.5;
    animation:float 7s linear infinite;
}

.p1{left:10%;top:75%;animation-delay:0s;}
.p2{left:20%;top:25%;animation-delay:2s;}
.p3{left:80%;top:30%;animation-delay:1s;}
.p4{left:90%;top:70%;animation-delay:3s;}
.p5{left:35%;top:85%;animation-delay:4s;}
.p6{left:70%;top:15%;animation-delay:2.5s;}
.p7{left:55%;top:80%;animation-delay:1.5s;}

@keyframes float{
    0%{
        transform:translateY(40px);
        opacity:0;
    }

    30%{
        opacity:.7;
    }

    70%{
        opacity:.4;
    }

    100%{
        transform:translateY(-100px);
        opacity:0;
    }
}

/* ================= HERO CONTENT ================= */

.hero-content{
    position:relative;
    z-index:5;

    width:100%;
    max-width:1150px;

    margin-left:auto!important;
    margin-right:auto!important;

    text-align:center;

    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;

    animation:heroIn 1.2s ease forwards;
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
    color:#20d9ff;
    font-size:14px;
    font-weight:800;
    letter-spacing:3px;
    margin-bottom:28px;

    text-shadow:
        0 0 10px rgba(32,217,255,.7);

    animation:fadeDown 1s ease .2s both;
}

@keyframes fadeDown{
    from{
        opacity:0;
        transform:translateY(-20px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }
}

.hero h1{
    width:100%;
    text-align:center;

    font-size:clamp(48px,8vw,105px);
    line-height:.98;

    font-weight:900;
    letter-spacing:-4px;

    margin-bottom:30px;

    text-shadow:
        0 5px 25px rgba(0,0,0,.4);

    animation:titleIn 1.2s ease .25s both;
}

@keyframes titleIn{
    from{
        opacity:0;
        transform:scale(.92);
    }

    to{
        opacity:1;
        transform:scale(1);
    }
}

.hero h1 span{
    display:block;

    color:#20d9ff;

    text-shadow:
        0 0 10px rgba(32,217,255,.55),
        0 0 35px rgba(32,217,255,.25);
}

.hero-line{
    width:80%;
    max-width:850px;
    height:1px;

    background:linear-gradient(
        90deg,
        transparent,
        rgba(255,255,255,.7),
        transparent
    );

    margin:0 auto 28px;

    position:relative;
}

.hero-line::after{
    content:"";
    position:absolute;
    left:50%;
    top:0;

    width:120px;
    height:2px;

    transform:translateX(-50%);

    background:#20d9ff;

    box-shadow:
        0 0 15px #20d9ff,
        0 0 30px #20d9ff;
}

.hero p{
    width:100%;
    max-width:800px;

    margin:0 auto;

    color:#c9d6e3;

    font-size:18px;
    line-height:1.8;

    text-align:center;

    animation:fadeUp 1s ease .7s both;
}

@keyframes fadeUp{
    from{
        opacity:0;
        transform:translateY(25px);
    }

    to{
        opacity:1;
        transform:translateY(0);
    }
}

/* ================= BUTTONS ================= */

.hero-buttons{
    width:100%;
    display:flex;
    justify-content:center;
    align-items:center;
    gap:10px;

    margin-top:35px;

    animation:fadeUp 1s ease .9s both;
}

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;

    min-width:190px;

    padding:15px 25px;

    border-radius:10px;

    text-decoration:none;

    font-weight:800;
    font-size:14px;

    color:#03101a;
    background:#20d9ff;

    border:2px solid #20d9ff;

    cursor:pointer;

    transition:.3s;

    box-shadow:
        0 0 20px rgba(32,217,255,.15);
}

.btn:hover{
    transform:translateY(-4px);

    background:transparent;
    color:#20d9ff;

    box-shadow:
        0 0 25px rgba(32,217,255,.3);
}

.btn-outline{
    background:transparent;
    color:#20d9ff;
}

/* ================= SECTIONS ================= */

section{
    width:100%;
    padding:110px 5%;
}

.container{
    width:100%;
    max-width:1250px;
    margin:0 auto;
}

.section-title{
    text-align:center;
    margin-bottom:55px;
}

.section-title h2{
    font-size:clamp(35px,5vw,55px);
    margin-bottom:12px;
}

.section-title p{
    color:#9fb2c5;
}

/* ================= ABOUT ================= */

.about{
    background:#091827;
}

.about-grid{
    width:100%;
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:30px;
}

.about-box{
    padding:40px;

    background:#0d2035;

    border:1px solid #1b3b59;
    border-radius:18px;

    transition:.3s;
}

.about-box:hover{
    transform:translateY(-7px);
    border-color:#20d9ff;
    box-shadow:0 15px 40px rgba(32,217,255,.08);
}

.about-box h3{
    color:#20d9ff;
    margin-bottom:15px;
}

.about-box p{
    color:#c5d3df;
    font-size:17px;
}

/* ================= COURSES ================= */

.courses{
    background:#07111f;
}

.course-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.course{
    padding:32px;

    background:#0d2035;

    border:1px solid #1b3b59;
    border-radius:18px;

    transition:.35s;
}

.course:hover{
    transform:translateY(-9px);
    border-color:#20d9ff;

    box-shadow:
        0 15px 40px rgba(32,217,255,.1);
}

.course h3{
    color:#20d9ff;
    font-size:24px;
    margin-bottom:14px;
}

.course p{
    color:#b9c9d9;
    margin-bottom:22px;
}

/* ================= PORTAL ================= */

.portal{
    background:#091827;
}

.portal-box{
    width:100%;
    max-width:650px;
    margin:auto;

    padding:40px;

    background:#0d2035;

    border:1px solid #1b3b59;
    border-radius:18px;
}

.input{
    width:100%;

    padding:15px;
    margin-bottom:14px;

    background:#07111f;
    color:white;

    border:1px solid #31506d;
    border-radius:8px;

    outline:none;
}

.input:focus{
    border-color:#20d9ff;
    box-shadow:0 0 12px rgba(32,217,255,.12);
}

/* ================= CONTACT ================= */

.contact{
    background:#07111f;
}

.contact-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:30px;
}

.contact-box{
    padding:40px;

    background:#0d2035;

    border:1px solid #1b3b59;
    border-radius:18px;
}

.contact-box h3{
    color:#20d9ff;
    margin-bottom:20px;
}

.contact-box p{
    color:#c6d4e0;
    margin:12px 0;
}

/* ================= FOOTER ================= */

footer{
    width:100%;
    padding:30px 20px;

    text-align:center;

    color:#879db2;
    background:#020812;

    border-top:1px solid #172d44;
}

/* ================= TABLET ================= */

@media(max-width:900px){

    .navbar{
        height:70px;
        padding:0 20px;
    }

    .menu-btn{
        display:block;
    }

    .nav-links{
        position:absolute;
        top:70px;
        left:0;

        width:100%;

        background:#07111f;

        display:none;
        flex-direction:column;

        padding:25px;

        border-bottom:1px solid #1b3b59;
    }

    .nav-links.active{
        display:flex;
    }

    .about-grid,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .course-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .hero h1{
        font-size:clamp(45px,9vw,75px);
    }
}

/* ================= MOBILE ================= */

@media(max-width:600px){

    section{
        padding:85px 18px;
    }

    .logo{
        font-size:13px;
    }

    .logo-box{
        width:40px;
        height:40px;
    }

    .hero{
        padding:110px 18px 60px;
    }

    .hero-small{
        font-size:11px;
        letter-spacing:2px;
    }

    .hero h1{
        font-size:47px;
        letter-spacing:-2px;
    }

    .hero p{
        font-size:16px;
    }

    .hero-buttons{
        flex-direction:column;
        width:100%;
    }

    .btn{
        width:100%;
    }

    .course-grid{
        grid-template-columns:1fr;
    }

    .about-box,
    .course,
    .contact-box,
    .portal-box{
        padding:28px 22px;
    }
}
</style>
</head>

<body>

<header>

<nav class="navbar">

<div class="logo">
    <div class="logo-box">KV</div>
    <span>COMMERCE CLASSES BY KV SIR</span>
</div>

<div class="menu-btn" onclick="toggleMenu()">☰</div>

<ul class="nav-links" id="navLinks">
    <li><a href="#home">HOME</a></li>
    <li><a href="#courses">COURSES</a></li>
    <li><a href="#about">ABOUT</a></li>
    <li><a href="#contact">CONTACT</a></li>
    <li><a href="#portal" class="login-btn">STUDENT LOGIN</a></li>
</ul>

</nav>

</header>


<main>

<!-- HERO -->

<section class="hero" id="home">

<div class="particle p1"></div>
<div class="particle p2"></div>
<div class="particle p3"></div>
<div class="particle p4"></div>
<div class="particle p5"></div>
<div class="particle p6"></div>
<div class="particle p7"></div>

<div class="hero-content">

<div class="hero-small">
SMART COMMERCE LEARNING • BUILD YOUR FUTURE
</div>

<h1>
LEARN TODAY.
<span>LEAD TOMORROW.</span>
</h1>

<div class="hero-line"></div>

<p>
COMMERCE CLASSES BY KV SIR helps students turn difficult
concepts into clear understanding, confidence and consistent progress.
</p>

<div class="hero-buttons">

<a href="#courses" class="btn">
EXPLORE COURSES →
</a>

<a href="#contact" class="btn btn-outline">
START YOUR JOURNEY
</a>

</div>

</div>

</section>


<!-- ABOUT -->

<section class="about" id="about">

<div class="container">

<div class="section-title">
<h2>ABOUT KV SIR</h2>
<p>Strong concepts. Better confidence. Brighter future.</p>
</div>

<div class="about-grid">

<div class="about-box">
<h3>CONCEPT BASED LEARNING</h3>
<p>
We focus on understanding Commerce concepts clearly rather than
just memorising answers. Our approach makes learning simple,
practical and effective.
</p>
</div>

<div class="about-box">
<h3>BUILD YOUR FUTURE</h3>
<p>
Students receive structured guidance to develop academic
knowledge, confidence and skills for their future studies and career.
</p>
</div>

</div>

</div>

</section>


<!-- COURSES -->

<section class="courses" id="courses">

<div class="container">

<div class="section-title">
<h2>OUR COURSES</h2>
<p>Choose your course and start your journey.</p>
</div>

<div class="course-grid">

<div class="course">
<h3>CLASS XI</h3>
<p>
Build your foundation in Accountancy, Business Studies,
Economics and Commerce.
</p>
<button class="btn" onclick="courseInfo('Class XI')">
VIEW DETAILS
</button>
</div>

<div class="course">
<h3>CLASS XII</h3>
<p>
Strengthen your concepts and prepare confidently for
your board examinations.
</p>
<button class="btn" onclick="courseInfo('Class XII')">
VIEW DETAILS
</button>
</div>

<div class="course">
<h3>B.COM</h3>
<p>
Develop deeper knowledge of accounting, business,
economics and commerce.
</p>
<button class="btn" onclick="courseInfo('B.Com')">
VIEW DETAILS
</button>
</div>

<div class="course">
<h3>BBA</h3>
<p>
Learn business fundamentals, management concepts and
practical decision-making skills.
</p>
<button class="btn" onclick="courseInfo('BBA')">
VIEW DETAILS
</button>
</div>

<div class="course">
<h3>MBA</h3>
<p>
Build advanced knowledge of management and business
for higher education and career development.
</p>
<button class="btn" onclick="courseInfo('MBA')">
VIEW DETAILS
</button>
</div>

<div class="course">
<h3>PERSONAL GUIDANCE</h3>
<p>
Get academic guidance and support according to your
learning requirements.
</p>
<button class="btn" onclick="whatsapp()">
ENQUIRE NOW
</button>
</div>

</div>

</div>

</section>


<!-- STUDENT PORTAL -->

<section class="portal" id="portal">

<div class="container">

<div class="section-title">
<h2>STUDENT PORTAL</h2>
<p>Login or create your student account.</p>
</div>

<div class="portal-box">

<input
class="input"
type="text"
id="studentName"
placeholder="Student Name">

<input
class="input"
type="email"
id="studentEmail"
placeholder="Email Address">

<input
class="input"
type="password"
id="studentPassword"
placeholder="Password">

<button class="btn" onclick="signup()">
CREATE ACCOUNT
</button>

<button class="btn btn-outline" onclick="login()">
LOGIN
</button>

<p id="portalMessage"
style="margin-top:15px;color:#20d9ff;text-align:center;">
</p>

</div>

</div>

</section>


<!-- CONTACT -->

<section class="contact" id="contact">

<div class="container">

<div class="section-title">
<h2>CONTACT US</h2>
<p>Start your learning journey today.</p>
</div>

<div class="contact-grid">

<div class="contact-box">

<h3>CONTACT DETAILS</h3>

<p>📍 Anand Nagar, Bahodapur, Gwalior</p>

<p>📞 7987116714</p>

<p>📚 Class XI | Class XII | B.Com | BBA | MBA</p>

<a
class="btn"
href="https://wa.me/917987116714?text=Hello%20KV%20Sir,%20I%20want%20information%20about%20your%20Commerce%20Classes."
target="_blank">
WHATSAPP US
</a>

</div>


<div class="contact-box">

<h3>SEND AN ENQUIRY</h3>

<input
class="input"
id="contactName"
placeholder="Your Name">

<input
class="input"
id="contactCourse"
placeholder="Course / Class">

<input
class="input"
id="contactMessage"
placeholder="Your Message">

<button class="btn" onclick="sendWhatsApp()">
SEND ENQUIRY
</button>

</div>

</div>

</div>

</section>

</main>


<footer>

© 2026 Commerce Classes by KV Sir
<br>
Anand Nagar, Bahodapur, Gwalior

</footer>


<script>

function toggleMenu(){
    document.getElementById("navLinks").classList.toggle("active");
}

document.querySelectorAll(".nav-links a").forEach(function(link){
    link.addEventListener("click",function(){
        document.getElementById("navLinks").classList.remove("active");
    });
});

function courseInfo(course){
    alert(
        course +
        "\n\nFor admission, fees and batch details, contact KV Sir on WhatsApp: 7987116714"
    );
}

function whatsapp(){
    window.open(
        "https://wa.me/917987116714?text=Hello%20KV%20Sir,%20I%20want%20information%20about%20admission.",
        "_blank"
    );
}

function signup(){

    const name=document.getElementById("studentName").value.trim();
    const email=document.getElementById("studentEmail").value.trim();
    const password=document.getElementById("studentPassword").value;
    const message=document.getElementById("portalMessage");

    if(!name || !email || !password){
        message.innerText="Please fill all fields.";
        return;
    }

    localStorage.setItem(
        "kvStudent",
        JSON.stringify({
            name:name,
            email:email,
            password:password
        })
    );

    message.innerText="Account created successfully!";
}

function login(){

    const email=document.getElementById("studentEmail").value.trim();
    const password=document.getElementById("studentPassword").value;
    const message=document.getElementById("portalMessage");

    const student=JSON.parse(localStorage.getItem("kvStudent"));

    if(student && student.email===email && student.password===password){
        message.innerText="Welcome "+student.name+"! Login successful.";
    }else{
        message.innerText="Invalid email or password.";
    }
}

function sendWhatsApp(){

    const name=document.getElementById("contactName").value.trim();
    const course=document.getElementById("contactCourse").value.trim();
    const msg=document.getElementById("contactMessage").value.trim();

    if(!name || !course || !msg){
        alert("Please fill all enquiry fields.");
        return;
    }

    const text=
        "Hello KV Sir,%0A%0A"+
        "Name: "+encodeURIComponent(name)+"%0A"+
        "Course: "+encodeURIComponent(course)+"%0A"+
        "Message: "+encodeURIComponent(msg);

    window.open(
        "https://wa.me/917987116714?text="+text,
        "_blank"
    );
}

</script>

</body>
</html>
