<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#07111f">
<title>Commerce Classes by KV Sir</title>

<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

html,body{
    width:100%;
    min-width:100%;
    overflow-x:hidden;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#07111f;
    color:#fff;
}

header{
    position:fixed;
    top:0;
    left:0;
    width:100%;
    z-index:9999;
    background:rgba(4,12,23,.96);
    border-bottom:1px solid #18324d;
}

.navbar{
    width:100%;
    max-width:1400px;
    min-height:76px;
    margin:auto;
    padding:0 35px;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
    font-weight:800;
    font-size:18px;
}

.logo-box{
    width:44px;
    height:44px;
    border-radius:12px;
    background:#20d9ff;
    color:#06111e;
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:900;
}

.logo span{
    color:#20d9ff;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:30px;
    list-style:none;
}

.nav-links a{
    color:#fff;
    text-decoration:none;
    font-size:14px;
    font-weight:700;
}

.nav-links a:hover{
    color:#20d9ff;
}

.login-btn{
    background:#20d9ff;
    color:#06111e!important;
    padding:14px 22px;
    border-radius:10px;
}

.menu-btn{
    display:none;
    color:#20d9ff;
    font-size:30px;
    cursor:pointer;
}

.hero{
    width:100vw;
    min-height:100vh;
    padding:150px 25px 80px;
    display:flex;
    align-items:center;
    justify-content:center;
    text-align:center;
    background:
    radial-gradient(
        circle at 50% 50%,
        rgba(0,100,255,.35) 0%,
        rgba(7,17,31,.95) 50%,
        #020914 100%
    );
}

.hero-content{
    width:100%;
    max-width:1100px;
}

.hero-small{
    color:#20d9ff;
    font-size:14px;
    font-weight:800;
    letter-spacing:3px;
    margin-bottom:25px;
}

.hero h1{
    font-size:clamp(48px,8vw,100px);
    line-height:.98;
    font-weight:900;
    letter-spacing:-3px;
    margin-bottom:30px;
}

.hero h1 span{
    color:#20d9ff;
}

.hero-line{
    width:100%;
    max-width:1000px;
    height:1px;
    background:rgba(255,255,255,.35);
    margin:0 auto 28px;
}

.hero p{
    max-width:850px;
    margin:auto;
    color:#c5d4e3;
    font-size:19px;
}

.hero-buttons{
    margin-top:35px;
}

.btn{
    display:inline-block;
    padding:15px 28px;
    margin:5px;
    border-radius:9px;
    background:#20d9ff;
    color:#04101c;
    text-decoration:none;
    font-weight:800;
    border:2px solid #20d9ff;
    cursor:pointer;
}

.btn:hover{
    background:transparent;
    color:#20d9ff;
}

.btn-outline{
    background:transparent;
    color:#20d9ff;
}

section{
    width:100vw;
    padding:110px 30px;
}

.container{
    width:100%;
    max-width:1250px;
    margin:auto;
}

.section-title{
    text-align:center;
    margin-bottom:60px;
}

.section-title h2{
    font-size:clamp(35px,5vw,55px);
    margin-bottom:12px;
}

.section-title p{
    color:#9eb1c5;
    font-size:17px;
}

.about{
    background:#091827;
}

.about-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:30px;
}

.about-box{
    padding:45px;
    background:#0e2136;
    border:1px solid #1b3b59;
    border-radius:18px;
}

.about-box h3{
    color:#20d9ff;
    font-size:27px;
    margin-bottom:15px;
}

.about-box p{
    color:#c5d3df;
    font-size:17px;
}

.courses{
    background:#07111f;
}

.course-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:25px;
}

.course{
    padding:35px;
    background:#0d2035;
    border:1px solid #1b3b59;
    border-radius:18px;
    transition:.3s;
}

.course:hover{
    transform:translateY(-8px);
    border-color:#20d9ff;
}

.course h3{
    color:#20d9ff;
    font-size:25px;
    margin-bottom:15px;
}

.course p{
    color:#b9c9d9;
    margin-bottom:25px;
}

.portal{
    background:#091827;
}

.portal-box{
    width:100%;
    max-width:650px;
    margin:auto;
    padding:40px;
    background:#0e2136;
    border:1px solid #1b3b59;
    border-radius:18px;
}

.input{
    width:100%;
    padding:15px;
    margin-bottom:14px;
    background:#07111f;
    color:#fff;
    border:1px solid #31506d;
    border-radius:8px;
    outline:none;
    font-size:16px;
}

.input:focus{
    border-color:#20d9ff;
}

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
    font-size:25px;
    margin-bottom:20px;
}

.contact-box p{
    color:#c6d4e0;
    margin:12px 0;
}

footer{
    width:100%;
    padding:30px 20px;
    background:#020812;
    color:#879db2;
    text-align:center;
    border-top:1px solid #172d44;
}

@media(max-width:900px){

    .navbar{
        padding:0 20px;
    }

    .menu-btn{
        display:block;
    }

    .nav-links{
        position:absolute;
        top:76px;
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
}

@media(max-width:600px){

    section{
        padding:85px 18px;
    }

    .logo{
        font-size:14px;
    }

    .hero{
        min-height:100svh;
        padding:120px 18px 60px;
    }

    .hero h1{
        font-size:48px;
        letter-spacing:-2px;
    }

    .hero p{
        font-size:16px;
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

    .btn{
        width:100%;
        margin:5px 0;
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

<section class="hero" id="home">
<div class="hero-content">

<div class="hero-small">
SMART COMMERCE LEARNING • BUILD YOUR FUTURE
</div>

<h1>
LEARN TODAY.<br>
<span>LEAD TOMORROW.</span>
</h1>

<div class="hero-line"></div>

<p>
COMMERCE CLASSES BY KV SIR helps students turn difficult
concepts into clear understanding, confidence and consistent progress.
</p>

<div class="hero-buttons">
<a href="#courses" class="btn">EXPLORE COURSES →</a>
<a href="#contact" class="btn btn-outline">START YOUR JOURNEY</a>
</div>

</div>
</section>

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

<section class="courses" id="courses">
<div class="container">

<div class="section-title">
<h2>OUR COURSES</h2>
<p>Choose your course and start your journey.</p>
</div>

<div class="course-grid">

<div class="course">
<h3>CLASS XI</h3>
<p>Build your foundation in Accountancy, Business Studies, Economics and Commerce.</p>
<button class="btn" onclick="courseInfo('Class XI')">VIEW DETAILS</button>
</div>

<div class="course">
<h3>CLASS XII</h3>
<p>Strengthen your concepts and prepare confidently for your board examinations.</p>
<button class="btn" onclick="courseInfo('Class XII')">VIEW DETAILS</button>
</div>

<div class="course">
<h3>B.COM</h3>
<p>Develop deeper knowledge of accounting, business, economics and commerce.</p>
<button class="btn" onclick="courseInfo('B.Com')">VIEW DETAILS</button>
</div>

<div class="course">
<h3>BBA</h3>
<p>Learn business fundamentals, management concepts and practical decision-making skills.</p>
<button class="btn" onclick="courseInfo('BBA')">VIEW DETAILS</button>
</div>

<div class="course">
<h3>MBA</h3>
<p>Build advanced knowledge of management and business for higher education and career development.</p>
<button class="btn" onclick="courseInfo('MBA')">VIEW DETAILS</button>
</div>

<div class="course">
<h3>PERSONAL GUIDANCE</h3>
<p>Get academic guidance and support according to your learning requirements.</p>
<button class="btn" onclick="whatsapp()">ENQUIRE NOW</button>
</div>

</div>
</div>
</section>

<section class="portal" id="portal">
<div class="container">

<div class="section-title">
<h2>STUDENT PORTAL</h2>
<p>Login or create your student account.</p>
</div>

<div class="portal-box">

<input class="input" type="text" id="studentName" placeholder="Student Name">

<input class="input" type="email" id="studentEmail" placeholder="Email Address">

<input class="input" type="password" id="studentPassword" placeholder="Password">

<button class="btn" onclick="signup()">CREATE ACCOUNT</button>
<button class="btn btn-outline" onclick="login()">LOGIN</button>

<p id="portalMessage" style="margin-top:15px;color:#20d9ff;text-align:center;"></p>

</div>
</div>
</section>

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

<input class="input" id="contactName" placeholder="Your Name">
<input class="input" id="contactCourse" placeholder="Course / Class">
<input class="input" id="contactMessage" placeholder="Your Message">

<button class="btn" onclick="sendWhatsApp()">SEND ENQUIRY</button>
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
