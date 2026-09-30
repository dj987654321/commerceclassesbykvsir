<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Commerce Classes by KV Sir</title>

<style>
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    width:100%;
    overflow-x:hidden;
    font-family:Arial,Helvetica,sans-serif;
    background:#050b16;
    color:white;
}

/* ================= HEADER ================= */

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    height:78px;
    z-index:9999;
    background:rgba(3,9,18,.90);
    backdrop-filter:blur(15px);
    border-bottom:1px solid rgba(32,217,255,.15);
}

.navbar{
    width:100%;
    height:100%;
    padding:0 5%;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
    font-size:17px;
    font-weight:800;
    white-space:nowrap;
}

.logo-box{
    width:44px;
    height:44px;
    border-radius:12px;
    background:#20d9ff;
    color:#06111d;
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:900;
    box-shadow:0 0 25px rgba(32,217,255,.35);
}

.logo span{
    color:#20d9ff;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:28px;
    list-style:none;
}

.nav-links li{
    position:relative;
}

.nav-links a{
    color:white;
    text-decoration:none;
    font-size:14px;
    font-weight:700;
    transition:.3s;
}

.nav-links a:hover{
    color:#20d9ff;
}

.login-btn{
    background:#20d9ff;
    color:#03101a!important;
    padding:13px 21px;
    border-radius:9px;
}

/* ================= COURSES DROPDOWN ================= */

.course-menu{
    position:relative;
}

.course-menu > a{
    cursor:pointer;
}

.course-menu > a::after{
    content:" ▾";
    color:#20d9ff;
}

.course-dropdown{
    position:absolute;
    top:52px;
    left:50%;
    transform:translateX(-50%) translateY(14px) scale(.96);
    transform-origin:top center;

    width:290px;

    background:linear-gradient(145deg,rgba(10,27,47,.98),rgba(3,12,25,.98));
    border:1px solid rgba(32,217,255,.35);
    border-radius:18px;

    padding:12px;

    opacity:0;
    visibility:hidden;
    pointer-events:none;

    transition:.35s cubic-bezier(.2,.8,.2,1);

    box-shadow:
        0 25px 70px rgba(0,0,0,.65),
        0 0 35px rgba(32,217,255,.14),
        inset 0 1px 0 rgba(255,255,255,.06);
}

.course-menu.open .course-dropdown{
    opacity:1;
    visibility:visible;
    pointer-events:auto;
    transform:translateX(-50%) translateY(0) scale(1);
}

.course-menu > a::after{
    transition:.3s;
}

.course-menu.open > a::after{
    display:inline-block;
    transform:rotate(180deg);
}

.course-dropdown::before{
    content:"";
    position:absolute;
    top:-7px;
    left:50%;
    width:13px;
    height:13px;
    transform:translateX(-50%) rotate(45deg);
    background:#0a1b2f;
    border-left:1px solid rgba(32,217,255,.35);
    border-top:1px solid rgba(32,217,255,.35);
}

.course-dropdown a{
    position:relative;
    display:flex;
    align-items:center;
    gap:8px;
    margin:4px 0;
    overflow:hidden;
}

.course-dropdown a::after{
    content:"→";
    margin-left:auto;
    opacity:0;
    transform:translateX(-8px);
    transition:.25s;
}

.course-dropdown a:hover::after{
    opacity:1;
    transform:translateX(0);
}

.course-dropdown a{
    display:block;
    padding:13px 15px;
    border-radius:9px;
    color:#dbe8f3;
}

.course-dropdown a:hover{
    background:rgba(32,217,255,.10);
    color:#20d9ff;
    padding-left:22px;
}

/* ================= EXTRA VISUAL EFFECTS ================= */

body::before{
    content:"";
    position:fixed;
    inset:0;
    pointer-events:none;
    z-index:9998;
    background:
        radial-gradient(circle at 15% 20%,rgba(32,217,255,.035),transparent 28%),
        radial-gradient(circle at 85% 75%,rgba(95,75,255,.035),transparent 30%);
}

header::after{
    content:"";
    position:absolute;
    left:0;
    bottom:-1px;
    width:100%;
    height:1px;
    background:linear-gradient(90deg,transparent,#20d9ff,transparent);
    box-shadow:0 0 18px rgba(32,217,255,.55);
    opacity:.75;
}

.course{
    position:relative;
    overflow:hidden;
}

.course::before,
.about-box::before,
.contact-box::before,
.portal-box::before{
    content:"";
    position:absolute;
    width:180px;
    height:180px;
    top:-90px;
    right:-90px;
    border-radius:50%;
    background:radial-gradient(circle,rgba(32,217,255,.13),transparent 68%);
    transition:.4s;
    pointer-events:none;
}

.course:hover::before,
.about-box:hover::before,
.contact-box:hover::before,
.portal-box:hover::before{
    transform:scale(1.35);
}

.course::after{
    content:"";
    position:absolute;
    top:0;
    left:-120%;
    width:70%;
    height:100%;
    background:linear-gradient(100deg,transparent,rgba(255,255,255,.07),transparent);
    transform:skewX(-20deg);
    transition:.7s;
}

.course:hover::after{
    left:140%;
}

.btn{
    position:relative;
    overflow:hidden;
}

.btn::after{
    content:"";
    position:absolute;
    top:0;
    left:-120%;
    width:65%;
    height:100%;
    background:linear-gradient(100deg,transparent,rgba(255,255,255,.32),transparent);
    transform:skewX(-20deg);
    transition:.6s;
}

.btn:hover::after{
    left:140%;
}

.section-title h2{
    text-shadow:0 0 25px rgba(32,217,255,.10);
}

.course-grid .course:nth-child(1){animation:cardIn .7s ease both;}
.course-grid .course:nth-child(2){animation:cardIn .7s .08s ease both;}
.course-grid .course:nth-child(3){animation:cardIn .7s .16s ease both;}
.course-grid .course:nth-child(4){animation:cardIn .7s .24s ease both;}
.course-grid .course:nth-child(5){animation:cardIn .7s .32s ease both;}
.course-grid .course:nth-child(6){animation:cardIn .7s .40s ease both;}

@keyframes cardIn{
    from{opacity:0;transform:translateY(25px);}
    to{opacity:1;transform:translateY(0);}
}

@media(max-width:900px){
    .course-dropdown{
        position:static;
        width:100%;
        transform:none;
        transform-origin:initial;
    }

    .course-menu.open .course-dropdown{
        transform:none;
    }

    .course-dropdown::before{
        display:none;
    }
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
    width:100%;
    min-height:100vh;
    min-height:100svh;

    display:flex;
    align-items:center;
    justify-content:center;

    text-align:center;

    padding:110px 20px 60px;

    position:relative;
    overflow:hidden;

    background:
        radial-gradient(
            circle at center,
            rgba(0,120,255,.28) 0%,
            rgba(0,60,120,.15) 30%,
            #07111f 65%,
            #020711 100%
        );
}

/* glowing center */

.hero::before{
    content:"";
    position:absolute;

    width:700px;
    height:700px;

    left:50%;
    top:50%;

    transform:translate(-50%,-50%);

    border-radius:50%;

    background:radial-gradient(
        circle,
        rgba(32,217,255,.18),
        transparent 68%
    );

    animation:glow 5s ease-in-out infinite;
}

@keyframes glow{
    0%,100%{
        transform:translate(-50%,-50%) scale(1);
        opacity:.65;
    }

    50%{
        transform:translate(-50%,-50%) scale(1.25);
        opacity:1;
    }
}

/* moving light */

.hero::after{
    content:"";
    position:absolute;
    top:0;
    left:-100%;
    width:60%;
    height:100%;

    background:linear-gradient(
        90deg,
        transparent,
        rgba(32,217,255,.05),
        transparent
    );

    transform:skewX(-20deg);
    animation:lightMove 7s infinite;
}

@keyframes lightMove{
    0%{
        left:-100%;
    }
    100%{
        left:150%;
    }
}

.hero-content{
    position:relative;
    z-index:5;

    width:100%;
    max-width:1100px;

    margin:auto;

    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;

    text-align:center;

    animation:heroIn 1s ease;
}

@keyframes heroIn{
    from{
        opacity:0;
        transform:translateY(30px);
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
    text-shadow:0 0 15px rgba(32,217,255,.6);
}

.hero h1{
    width:100%;
    font-size:clamp(48px,8vw,100px);
    line-height:1;
    font-weight:900;
    letter-spacing:-4px;
    text-align:center;
    margin-bottom:30px;
}

.hero h1 span{
    display:block;
    color:#20d9ff;

    text-shadow:
        0 0 10px rgba(32,217,255,.7),
        0 0 35px rgba(32,217,255,.25);
}

.hero-line{
    width:75%;
    max-width:850px;
    height:1px;

    background:linear-gradient(
        90deg,
        transparent,
        white,
        transparent
    );

    margin:0 auto 28px;

    position:relative;
}

.hero-line::after{
    content:"";
    position:absolute;

    width:130px;
    height:2px;

    left:50%;
    top:0;

    transform:translateX(-50%);

    background:#20d9ff;

    box-shadow:0 0 20px #20d9ff;
}

.hero p{
    width:100%;
    max-width:800px;

    margin:auto;

    color:#c8d6e4;
    font-size:18px;
    line-height:1.8;

    text-align:center;
}

.hero-buttons{
    margin-top:35px;

    display:flex;
    justify-content:center;
    align-items:center;
    gap:10px;
}

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;

    min-width:190px;

    padding:15px 25px;

    border-radius:10px;

    background:#20d9ff;
    color:#03101a;

    border:2px solid #20d9ff;

    text-decoration:none;

    font-size:14px;
    font-weight:800;

    cursor:pointer;

    transition:.3s;
}

.btn:hover{
    transform:translateY(-4px);
    background:transparent;
    color:#20d9ff;
    box-shadow:0 0 25px rgba(32,217,255,.3);
}

.btn-outline{
    background:transparent;
    color:#20d9ff;
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

.p1{left:10%;top:75%;}
.p2{left:20%;top:25%;animation-delay:2s;}
.p3{left:80%;top:30%;animation-delay:1s;}
.p4{left:90%;top:70%;animation-delay:3s;}
.p5{left:35%;top:85%;animation-delay:4s;}
.p6{left:70%;top:15%;animation-delay:2.5s;}

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

/* ================= SECTIONS ================= */

section{
    width:100%;
    padding:110px 5%;
}

.container{
    width:100%;
    max-width:1250px;
    margin:auto;
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
    transition:.3s;
}

.course:hover{
    transform:translateY(-8px);
    border-color:#20d9ff;
    box-shadow:0 15px 40px rgba(32,217,255,.1);
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
    font-size:16px;
}

.input:focus{
    border-color:#20d9ff;
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

/* ================= MOBILE ================= */

@media(max-width:900px){

    .navbar{
        padding:0 20px;
    }

    .menu-btn{
        display:block;
    }

    .nav-links{
        position:absolute;
        top:78px;
        left:0;
        width:100%;

        display:none;
        flex-direction:column;

        padding:25px;

        background:#07111f;
        border-bottom:1px solid #1b3b59;
    }

    .nav-links.active{
        display:flex;
    }

    .course-menu{
        width:100%;
        text-align:center;
    }

    .course-dropdown{
        position:static;

        width:100%;

        transform:none;

        display:none;

        opacity:1;
        visibility:visible;

        margin-top:10px;

        box-shadow:none;
    }

    .course-menu.open .course-dropdown{
        display:block;
    }

    .course-menu:hover .course-dropdown{
        transform:none;
    }

    .about-grid,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .course-grid{
        grid-template-columns:repeat(2,1fr);
    }
}

@media(max-width:600px){

    section{
        padding:85px 18px;
    }

    .logo{
        font-size:12px;
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

<li>
<a href="#home">HOME</a>
</li>

<li class="course-menu" id="courseMenu">

<a href="#courses" onclick="toggleCourses(event)">
COURSES
</a>

<div class="course-dropdown">

<a href="#class11" onclick="showCourse('Class XI')">
📘 Class XI
</a>

<a href="#class12" onclick="showCourse('Class XII')">
📕 Class XII
</a>

<a href="#bcom" onclick="showCourse('B.Com')">
📊 B.Com
</a>

<a href="#bba" onclick="showCourse('BBA')">
💼 BBA
</a>

<a href="#mba" onclick="showCourse('MBA')">
🎓 MBA
</a>

<a href="#guidance" onclick="showCourse('Personal Guidance')">
⭐ Personal Guidance
</a>

</div>

</li>

<li>
<a href="#about">ABOUT</a>
</li>

<li>
<a href="#contact">CONTACT</a>
</li>

<li>
<a href="#portal" class="login-btn">STUDENT LOGIN</a>
</li>

</ul>

</nav>

</header>


<main>

<!-- ================= HOME ================= -->

<section class="hero" id="home">

<div class="particle p1"></div>
<div class="particle p2"></div>
<div class="particle p3"></div>
<div class="particle p4"></div>
<div class="particle p5"></div>
<div class="particle p6"></div>

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


<!-- ================= ABOUT ================= -->

<section class="about" id="about">

<div class="container">

<div class="section-title">

<h2>ABOUT KV SIR</h2>

<p>
Strong concepts. Better confidence. Brighter future.
</p>

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


<!-- ================= COURSES ================= -->

<section class="courses" id="courses">

<div class="container">

<div class="section-title">

<h2>OUR COURSES</h2>

<p>
Choose your course and explore the subjects, learning options and guidance available.
</p>

</div>

<div class="course-grid">

<div class="course" id="class11">

<h3>CLASS XI</h3>

<p>
Build your foundation in Accountancy, Business Studies,
Economics and Commerce.
</p>

<button class="btn" onclick="showCourse('Class XI')">
VIEW COURSE
</button>

</div>


<div class="course" id="class12">

<h3>CLASS XII</h3>

<p>
Strengthen your concepts and prepare confidently for
your board examinations.
</p>

<button class="btn" onclick="showCourse('Class XII')">
VIEW COURSE
</button>

</div>


<div class="course" id="bcom">

<h3>B.COM</h3>

<p>
Develop deeper knowledge of accounting, business,
economics and commerce.
</p>

<button class="btn" onclick="showCourse('B.Com')">
VIEW COURSE
</button>

</div>


<div class="course" id="bba">

<h3>BBA</h3>

<p>
Learn business fundamentals, management concepts and
practical decision-making skills.
</p>

<button class="btn" onclick="showCourse('BBA')">
VIEW COURSE
</button>

</div>


<div class="course" id="mba">

<h3>MBA</h3>

<p>
Build advanced knowledge of management and business
for higher education and career development.
</p>

<button class="btn" onclick="showCourse('MBA')">
VIEW COURSE
</button>

</div>


<div class="course" id="guidance">

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


<!-- ================= PORTAL ================= -->

<section class="portal" id="portal">

<div class="container">

<div class="section-title">

<h2>STUDENT PORTAL</h2>

<p>
Login or create your student account.
</p>

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

<p
id="portalMessage"
style="margin-top:15px;color:#20d9ff;text-align:center;">
</p>

</div>

</div>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

<div class="container">

<div class="section-title">

<h2>CONTACT US</h2>

<p>
Start your learning journey today.
</p>

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

<button
class="btn"
onclick="sendWhatsApp()">

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

/* ================= MENU ================= */

function toggleMenu(){

    document
    .getElementById("navLinks")
    .classList.toggle("active");

}


/* ================= COURSE MENU ================= */

function toggleCourses(event){

    event.preventDefault();

    const courseMenu = document.getElementById("courseMenu");
    const navLinks = document.getElementById("navLinks");

    courseMenu.classList.toggle("open");

    if(window.innerWidth <= 900){
        navLinks.classList.add("active");
    }

}


/* ================= CLOSE MOBILE MENU ================= */

document.querySelectorAll(".nav-links > li > a").forEach(function(link){

    link.addEventListener("click",function(){

        if(
            !this.parentElement.classList.contains("course-menu")
        ){

            document
            .getElementById("navLinks")
            .classList.remove("active");

        }

    });

});


/* ================= COURSE OPTIONS ================= */

function showCourse(course){

    document.getElementById("courseMenu").classList.remove("open");

    let message="";

    if(course==="Class XI"){

        message=
        "CLASS XI OPTIONS\n\n"+
        "✓ Accountancy\n"+
        "✓ Business Studies\n"+
        "✓ Economics\n"+
        "✓ Commerce Foundation\n\n"+
        "Contact KV Sir for batch timings and fees.";

    }

    else if(course==="Class XII"){

        message=
        "CLASS XII OPTIONS\n\n"+
        "✓ Accountancy\n"+
        "✓ Business Studies\n"+
        "✓ Economics\n"+
        "✓ Board Exam Preparation\n\n"+
        "Contact KV Sir for batch timings and fees.";

    }

    else if(course==="B.Com"){

        message=
        "B.COM OPTIONS\n\n"+
        "✓ Financial Accounting\n"+
        "✓ Business Studies\n"+
        "✓ Economics\n"+
        "✓ Commerce Subjects\n\n"+
        "Contact KV Sir for details.";

    }

    else if(course==="BBA"){

        message=
        "BBA OPTIONS\n\n"+
        "✓ Business Management\n"+
        "✓ Marketing\n"+
        "✓ Accounting\n"+
        "✓ Economics\n\n"+
        "Contact KV Sir for details.";

    }

    else if(course==="MBA"){

        message=
        "MBA OPTIONS\n\n"+
        "✓ Management\n"+
        "✓ Business Strategy\n"+
        "✓ Finance\n"+
        "✓ Marketing\n\n"+
        "Contact KV Sir for details.";

    }

    else{

        message=
        "PERSONAL GUIDANCE\n\n"+
        "✓ Academic Guidance\n"+
        "✓ Subject Selection\n"+
        "✓ Study Planning\n"+
        "✓ Career Guidance";

    }

    alert(message);

}


/* ================= WHATSAPP ================= */

function whatsapp(){

    window.open(
        "https://wa.me/917987116714?text=Hello%20KV%20Sir,%20I%20want%20information%20about%20your%20Commerce%20Classes.",
        "_blank"
    );

}


/* ================= SIGNUP ================= */

function signup(){

    const name=
    document.getElementById("studentName").value.trim();

    const email=
    document.getElementById("studentEmail").value.trim();

    const password=
    document.getElementById("studentPassword").value;

    const message=
    document.getElementById("portalMessage");

    if(!name || !email || !password){

        message.innerText=
        "Please fill all fields.";

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

    message.innerText=
    "Account created successfully!";

}


/* ================= LOGIN ================= */

function login(){

    const email=
    document.getElementById("studentEmail").value.trim();

    const password=
    document.getElementById("studentPassword").value;

    const message=
    document.getElementById("portalMessage");

    const student=
    JSON.parse(localStorage.getItem("kvStudent"));

    if(
        student &&
        student.email===email &&
        student.password===password
    ){

        message.innerText=
        "Welcome "+student.name+"! Login successful.";

    }

    else{

        message.innerText=
        "Invalid email or password.";

    }

}


/* ================= CONTACT ================= */

function sendWhatsApp(){

    const name=
    document.getElementById("contactName").value.trim();

    const course=
    document.getElementById("contactCourse").value.trim();

    const msg=
    document.getElementById("contactMessage").value.trim();

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
