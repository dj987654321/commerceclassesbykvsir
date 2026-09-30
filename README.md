<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>COMMERCE CLASSES BY KV SIR</title>
<style>
*{
    box-sizing:border-box;
    margin:0;
    padding:0;
}

html{
    scroll-behavior:smooth;
}

body{
    font-family:Arial,Helvetica,sans-serif;
    background:#f5f7fb;
    color:#142033;
    line-height:1.6;
}

/* ================= NAVBAR ================= */

nav{
    position:sticky;
    top:0;
    z-index:1000;
    background:#071426;
    box-shadow:0 3px 15px rgba(0,0,0,.2);
}

.navbar{
    max-width:1200px;
    margin:auto;
    min-height:72px;
    padding:10px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
}

.logo{
    color:white;
    font-size:18px;
    font-weight:900;
}

.logo span{
    color:#29d6ff;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:18px;
    list-style:none;
}

.nav-links a{
    color:white;
    text-decoration:none;
    font-size:13px;
    font-weight:bold;
}

.nav-links a:hover{
    color:#29d6ff;
}

.sign-btn{
    background:#29d6ff;
    color:#071426 !important;
    padding:10px 16px;
    border-radius:8px;
}

/* ================= HERO ================= */

.hero{
    background:linear-gradient(135deg,#061326,#165279);
    color:white;
    padding:70px 20px;
}

.hero-container{
    max-width:1200px;
    margin:auto;
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:45px;
    align-items:center;
}

.badge{
    display:inline-block;
    padding:8px 15px;
    border:1px solid #5fe5ff;
    color:#5fe5ff;
    border-radius:30px;
    font-weight:bold;
    margin-bottom:15px;
}

.hero h1{
    font-size:clamp(42px,6vw,72px);
    line-height:1;
    margin:15px 0 20px;
}

.blue{
    color:#29d6ff;
}

.hero p{
    color:#dce6ef;
    font-size:17px;
    line-height:1.8;
    margin-bottom:20px;
}

.btn{
    display:inline-block;
    border:none;
    border-radius:9px;
    padding:13px 20px;
    margin:5px;
    font-weight:bold;
    cursor:pointer;
    text-decoration:none;
}

.primary{
    background:#29d6ff;
    color:#071426;
}

.primary:hover{
    background:#65e5ff;
}

.outline{
    color:white;
    border:1px solid rgba(255,255,255,.5);
}

.hero-image{
    width:100%;
    max-height:620px;
    object-fit:contain;
    background:white;
    border-radius:20px;
    box-shadow:0 20px 60px rgba(0,0,0,.35);
}

/* ================= COMMON ================= */

.section{
    padding:80px 20px;
}

.white{
    background:white;
}

.container{
    max-width:1200px;
    margin:auto;
}

.heading{
    text-align:center;
    margin-bottom:45px;
}

.heading small{
    color:#0088aa;
    font-weight:bold;
    letter-spacing:2px;
}

.heading h2{
    font-size:40px;
    margin:8px 0;
}

.heading p{
    color:#687588;
}

/* ================= ABOUT ================= */

.about-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:50px;
    align-items:center;
}

.teacher-image{
    width:100%;
    height:520px;
    object-fit:cover;
    border-radius:22px;
    box-shadow:0 15px 40px rgba(0,0,0,.15);
}

.about-text h2{
    font-size:35px;
    margin-bottom:15px;
}

.about-text p{
    color:#687588;
    line-height:1.9;
}

.quote{
    margin:25px 0;
    padding:18px;
    background:#eefbfe;
    border-left:5px solid #29d6ff;
    font-weight:bold;
}

/* ================= COURSES ================= */

.course-grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:16px;
}

.course-card{
    background:white;
    border:1px solid #e2e8f0;
    border-radius:18px;
    padding:22px 14px;
    text-align:center;
    box-shadow:0 8px 25px rgba(0,0,0,.06);
    transition:.3s;
}

.course-card:hover{
    transform:translateY(-6px);
    box-shadow:0 15px 35px rgba(0,0,0,.12);
}

.course-icon{
    font-size:35px;
}

.course-card h3{
    margin:10px 0 4px;
}

.course-card p{
    color:#687588;
}

.price{
    color:#087d9d;
    font-size:28px;
    font-weight:900;
    margin:12px;
}

.course-card ul{
    list-style:none;
    color:#687588;
    font-size:13px;
    line-height:2;
    margin-bottom:15px;
}

/* ================= SUBSCRIPTION ================= */

.steps{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:18px;
}

.step{
    background:#f8fafc;
    border:1px solid #e3e9ef;
    border-radius:18px;
    padding:28px 20px;
    text-align:center;
}

.number{
    width:45px;
    height:45px;
    margin:auto;
    display:grid;
    place-items:center;
    background:#29d6ff;
    border-radius:50%;
    font-weight:900;
    font-size:18px;
}

/* ================= GALLERY ================= */

.gallery{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:28px;
}

.gallery-card{
    background:white;
    border-radius:20px;
    padding:15px;
    box-shadow:0 8px 25px rgba(0,0,0,.1);
}

.gallery-card img{
    width:100%;
    height:500px;
    object-fit:contain;
    background:#f3f5f7;
    border-radius:15px;
}

.gallery-card h3{
    padding:15px 5px 5px;
}

/* ================= FEATURES ================= */

.features{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.feature{
    background:white;
    padding:25px;
    border-radius:18px;
    border:1px solid #e3e9ef;
}

.feature h3{
    margin-bottom:8px;
}

.feature p{
    color:#687588;
}

/* ================= CONTACT ================= */

.contact-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:20px;
}

.contact-box{
    background:white;
    padding:30px;
    border-radius:18px;
    box-shadow:0 8px 25px rgba(0,0,0,.07);
}

.contact-box p{
    margin:18px 0;
}

.contact-box a{
    color:#0088aa;
    text-decoration:none;
}

form{
    display:grid;
    gap:13px;
}

input,
select,
textarea{
    width:100%;
    padding:14px;
    border:1px solid #d8e0e8;
    border-radius:8px;
    font-size:15px;
}

textarea{
    min-height:120px;
    resize:vertical;
}

/* ================= FOOTER ================= */

footer{
    background:#050d18;
    color:#b5c0cc;
    text-align:center;
    padding:40px 20px;
}

footer strong{
    color:white;
}

/* ================= MODAL ================= */

.modal{
    display:none;
    position:fixed;
    inset:0;
    z-index:2000;
    background:rgba(0,0,0,.75);
    align-items:center;
    justify-content:center;
    padding:20px;
}

.modal.show{
    display:flex;
}

.modal-box{
    width:min(440px,100%);
    background:white;
    border-radius:20px;
    padding:30px;
    position:relative;
}

.close{
    position:absolute;
    right:18px;
    top:8px;
    font-size:30px;
    cursor:pointer;
}

.tabs{
    display:flex;
    gap:8px;
    margin:20px 0;
}

.tabs button{
    flex:1;
    padding:12px;
    border:none;
    border-radius:8px;
    cursor:pointer;
    background:#edf2f6;
    font-weight:bold;
}

.tabs button.active{
    background:#29d6ff;
}

/* ================= RESPONSIVE ================= */

@media(max-width:1000px){

    .hero-container,
    .about-grid,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .course-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .steps{
        grid-template-columns:repeat(2,1fr);
    }

    .features{
        grid-template-columns:1fr 1fr;
    }
}

@media(max-width:650px){

    .navbar{
        flex-direction:column;
        gap:12px;
    }

    .nav-links{
        flex-wrap:wrap;
        justify-content:center;
        gap:10px;
    }

    .nav-links a{
        font-size:11px;
    }

    .hero{
        padding:45px 15px;
    }

    .hero-container{
        gap:25px;
    }

    .hero h1{
        font-size:43px;
    }

    .section{
        padding:60px 15px;
    }

    .heading h2{
        font-size:30px;
    }

    .course-grid,
    .steps,
    .features,
    .gallery{
        grid-template-columns:1fr;
    }

    .teacher-image,
    .gallery-card img{
        height:auto;
        max-height:600px;
    }
}

/* ===== SEPARATE VIEWS + STUDENT ACCOUNT ===== */
.view{display:none;min-height:calc(100vh - 72px);animation:fadeIn .22s ease}
.view.active{display:block}
@keyframes fadeIn{from{opacity:.2;transform:translateY(5px)}to{opacity:1;transform:none}}
.page-head{background:linear-gradient(135deg,#061326,#165279);color:#fff;padding:55px 20px}
.page-head h1{font-size:clamp(34px,5vw,58px);margin-bottom:8px}
.page-head p{color:#dce6ef}
.nav-link-btn{background:none;border:0;color:#fff;font:inherit;font-weight:bold;cursor:pointer;padding:8px}
.nav-link-btn:hover{color:#29d6ff}
.account-layout{display:grid;grid-template-columns:260px 1fr;gap:24px}
.account-menu{background:#071426;color:#fff;border-radius:18px;padding:15px;height:max-content}
.account-menu button{width:100%;border:0;background:transparent;color:#fff;text-align:left;padding:13px;border-radius:10px;cursor:pointer;font-weight:bold;margin:2px 0}
.account-menu button:hover,.account-menu button.active{background:#12304d;color:#29d6ff}
.account-card{background:#fff;border:1px solid #e2e8f0;border-radius:18px;padding:25px;box-shadow:0 8px 25px rgba(0,0,0,.06)}
.course-detail-grid{display:grid;grid-template-columns:1fr 1fr;gap:25px}
.course-detail{background:#fff;border-radius:22px;padding:30px;box-shadow:0 12px 35px rgba(0,0,0,.08)}
.course-detail .big-icon{font-size:70px}
.course-detail ul{margin:18px 0 20px;padding-left:20px;line-height:2}
.action-row{display:flex;gap:10px;flex-wrap:wrap}
.stat-grid{display:grid;grid-template-columns:repeat(3,1fr);gap:15px;margin-top:20px}
.stat{background:#f4f8fb;border-radius:14px;padding:18px}
.stat strong{display:block;font-size:25px;color:#087d9d}
.empty-state{text-align:center;padding:40px 20px;background:#f8fafc;border-radius:15px}
@media(max-width:800px){.account-layout,.course-detail-grid{grid-template-columns:1fr}.stat-grid{grid-template-columns:1fr}}
</style>
</head>

<body>
<nav>
 <div class="navbar">
  <div class="logo">COMMERCE <span>CLASSES BY KV SIR</span></div>
  <ul class="nav-links">
   <li><button class="nav-link-btn" onclick="showView('home')">HOME</button></li>
   <li><button class="nav-link-btn" onclick="showView('about')">ABOUT</button></li>
   <li><button class="nav-link-btn" onclick="showView('courses')">COURSES</button></li>
   <li><button class="nav-link-btn" onclick="showView('subscription')">SUBSCRIPTIONS</button></li>
   <li><button class="nav-link-btn" onclick="showView('gallery')">GALLERY</button></li>
   <li><button class="nav-link-btn" onclick="showView('contact')">CONTACT</button></li>
   <li><button class="nav-link-btn sign-btn" id="accountNav" onclick="openAccount()">SIGN IN</button></li>
  </ul>
 </div>
</nav>

<main id="view-home" class="view active">
 <section class="hero"><div class="hero-container">
  <div><span class="badge">PROFESSIONAL COMMERCE EDUCATION</span>
   <h1>COMMERCE CLASSES<br><span class="blue">BY KV SIR</span></h1>
   <p>CLASS 11 • CLASS 12 • CBSE • ICSE<br>ACCOUNTS • ECONOMICS • BUSINESS STUDIES<br>HOME TUITION AVAILABLE</p>
   <button class="btn primary" onclick="showView('courses')">VIEW COURSES</button>
   <button class="btn outline" onclick="openAccount()">STUDENT ACCOUNT</button>
  </div>
  <img src="kv-sir-poster.png" class="hero-image" alt="COMMERCE CLASSES BY KV SIR">
 </div></section>
 <section class="section white"><div class="container">
  <div class="heading"><small>QUICK ACCESS</small><h2>EXPLORE THE WEBSITE</h2><p>Open each major section separately.</p></div>
  <div class="features">
   <div class="feature"><h3>📚 COURSES</h3><p>Open Class 11, Class 12, B.Com, BBA or MBA separately.</p><button class="btn primary" onclick="showView('courses')">OPEN COURSES</button></div>
   <div class="feature"><h3>👤 STUDENT ACCOUNT</h3><p>Create an account, sign in and manage your student dashboard.</p><button class="btn primary" onclick="openAccount()">OPEN ACCOUNT</button></div>
   <div class="feature"><h3>📝 SUBSCRIPTIONS</h3><p>View the course subscription process and enquire.</p><button class="btn primary" onclick="showView('subscription')">OPEN SUBSCRIPTIONS</button></div>
  </div>
 </div></section>
</main>

<section id="view-about" class="view">
 <div class="page-head"><div class="container"><h1>ABOUT US</h1><p>COMMERCE CLASSES BY KV SIR</p></div></div>
 <section class="section white"><div class="container"><div class="about-grid">
  <img src="kv-sir-photo.png" class="teacher-image" alt="KV SIR">
  <div class="about-text"><h2>LEARN COMMERCE WITH KV SIR</h2>
   <p>OUR TEACHING APPROACH FOCUSES ON CLEAR CONCEPTS, SIMPLE EXPLANATIONS, REGULAR PRACTICE, TESTS, FEEDBACK AND DOUBT-CLEARING SESSIONS.</p>
   <div class="quote">GIVE YOUR CHILD THE RIGHT LEARNING SUPPORT.</div>
   <button class="btn primary" onclick="showView('courses')">EXPLORE COURSES</button>
  </div>
 </div></div></section>
</section>

<section id="view-courses" class="view">
 <div class="page-head"><div class="container"><h1>COURSES</h1><p>Click any course to open its own dedicated page.</p></div></div>
 <section class="section"><div class="container"><div class="course-grid">
  <div class="course-card"><div class="course-icon">📘</div><h3>CLASS 11</h3><p>CBSE / ICSE</p><div class="price">₹2,000</div><ul><li>ACCOUNTS</li><li>ECONOMICS</li><li>BUSINESS STUDIES</li></ul><button class="btn primary" onclick="openCourse('class11')">OPEN COURSE</button></div>
  <div class="course-card"><div class="course-icon">🎓</div><h3>CLASS 12</h3><p>CBSE / ICSE</p><div class="price">₹2,000</div><ul><li>ACCOUNTS</li><li>ECONOMICS</li><li>BUSINESS STUDIES</li></ul><button class="btn primary" onclick="openCourse('class12')">OPEN COURSE</button></div>
  <div class="course-card"><div class="course-icon">📊</div><h3>B.COM</h3><p>COLLEGE</p><div class="price">₹2,000</div><ul><li>COMMERCE SUBJECTS</li><li>DOUBT SUPPORT</li><li>REGULAR PRACTICE</li></ul><button class="btn primary" onclick="openCourse('bcom')">OPEN COURSE</button></div>
  <div class="course-card"><div class="course-icon">💼</div><h3>BBA</h3><p>COLLEGE</p><div class="price">₹2,000</div><ul><li>BUSINESS SUBJECTS</li><li>DOUBT SUPPORT</li><li>REGULAR PRACTICE</li></ul><button class="btn primary" onclick="openCourse('bba')">OPEN COURSE</button></div>
  <div class="course-card"><div class="course-icon">🚀</div><h3>MBA</h3><p>COLLEGE</p><div class="price">₹2,000</div><ul><li>MANAGEMENT SUBJECTS</li><li>DOUBT SUPPORT</li><li>REGULAR PRACTICE</li></ul><button class="btn primary" onclick="openCourse('mba')">OPEN COURSE</button></div>
 </div></div></section>
</section>

<section id="view-course" class="view">
 <div class="page-head"><div class="container"><h1 id="coursePageTitle">COURSE</h1><p id="coursePageSubtitle"></p></div></div>
 <section class="section"><div class="container"><div class="course-detail-grid">
  <div class="course-detail"><div class="big-icon" id="courseIcon">📚</div><h2 id="courseDetailTitle"></h2><p id="courseDetailText"></p><div class="price">₹2,000</div><ul id="courseDetailList"></ul>
   <div class="action-row"><button class="btn primary" onclick="subscribeCurrentCourse()">SUBSCRIBE / ENQUIRE</button><button class="btn" onclick="showView('courses')">← ALL COURSES</button></div>
  </div>
  <div class="account-card"><h3>🎓 COURSE AREA</h3><p>This separate course page can contain course videos, notes, tests, assignments and announcements.</p>
   <div class="stat-grid"><div class="stat"><strong>₹2,000</strong>Subscription</div><div class="stat"><strong>✓</strong>Doubt Support</div><div class="stat"><strong>📝</strong>Practice</div></div>
   <button class="btn primary" onclick="openAccount()">OPEN STUDENT ACCOUNT</button>
  </div>
 </div></div></section>
</section>

<section id="view-subscription" class="view">
 <div class="page-head"><div class="container"><h1>SUBSCRIPTIONS</h1><p>Course-wise subscription process.</p></div></div>
 <section class="section white"><div class="container"><div class="heading"><small>SUBSCRIPTION PROCESS</small><h2>COURSE-WISE SUBSCRIPTION</h2><p>EVERY COURSE IS ₹2,000.</p></div>
  <div class="steps">
   <div class="step"><div class="number">1</div><h3>SELECT COURSE</h3><p>CHOOSE YOUR COURSE.</p></div>
   <div class="step"><div class="number">2</div><h3>SIGN IN</h3><p>CREATE OR USE YOUR STUDENT ACCOUNT.</p></div>
   <div class="step"><div class="number">3</div><h3>SEND ENQUIRY</h3><p>SHARE STUDENT AND COURSE DETAILS.</p></div>
   <div class="step"><div class="number">4</div><h3>CONFIRM</h3><p>CONFIRM ENROLLMENT AND PAYMENT DETAILS.</p></div>
  </div>
  <div style="text-align:center;margin-top:30px"><button class="btn primary" onclick="showView('contact')">START SUBSCRIPTION</button><button class="btn" onclick="openAccount()">CREATE ACCOUNT</button></div>
 </div></section>
</section>

<section id="view-gallery" class="view">
 <div class="page-head"><div class="container"><h1>GALLERY</h1><p>COMMERCE CLASSES BY KV SIR</p></div></div>
 <section class="section"><div class="container"><div class="gallery">
  <div class="gallery-card"><img src="kv-sir-poster.png" alt="COMMERCE CLASSES BY KV SIR POSTER"><h3>COMMERCE CLASSES BY KV SIR</h3></div>
  <div class="gallery-card"><img src="kv-sir-photo.png" alt="KV SIR"><h3>KV SIR</h3></div>
 </div></div></section>
</section>

<section id="view-contact" class="view">
 <div class="page-head"><div class="container"><h1>CONTACT</h1><p>ANAND NAGAR, BAHODAPUR, GWALIOR</p></div></div>
 <section class="section"><div class="container"><div class="contact-grid">
  <div class="contact-box"><h3>CONTACT DETAILS</h3><p>📞 <a href="tel:7987116714">7987116714</a></p><p>📍 ANAND NAGAR, BAHODAPUR, GWALIOR, MADHYA PRADESH</p><p>💰 COURSE PRICE: <strong>₹2,000</strong></p></div>
  <div class="contact-box"><form onsubmit="sendWhatsApp(event)">
   <input type="text" id="studentName" placeholder="STUDENT NAME" required>
   <input type="tel" id="phone" placeholder="PHONE NUMBER" required>
   <select id="courseName" required><option value="">SELECT COURSE</option><option>CLASS 11 - ₹2,000</option><option>CLASS 12 - ₹2,000</option><option>B.COM - ₹2,000</option><option>BBA - ₹2,000</option><option>MBA - ₹2,000</option></select>
   <textarea id="enquiry" placeholder="YOUR ENQUIRY" required></textarea>
   <button type="submit" class="btn primary">SEND ENQUIRY ON WHATSAPP</button>
  </form></div>
 </div></div></section>
</section>

<section id="view-account" class="view">
 <div class="page-head"><div class="container"><h1>STUDENT ACCOUNT</h1><p id="accountWelcome">Sign in or create your student account.</p></div></div>
 <section class="section"><div class="container">
  <div id="authBox" class="account-card" style="max-width:520px;margin:auto">
   <div class="tabs"><button id="loginTab" class="active" onclick="setAuthMode('login')">SIGN IN</button><button id="signupTab" onclick="setAuthMode('signup')">CREATE ACCOUNT</button></div>
   <form onsubmit="submitAuth(event)">
    <input type="text" id="fullName" placeholder="FULL NAME" style="display:none">
    <input type="email" id="email" placeholder="EMAIL" required>
    <input type="password" id="password" placeholder="PASSWORD" required>
    <button class="btn primary" id="authButton" type="submit">SIGN IN</button>
    <small>Demo account system: data is stored in this browser.</small>
   </form>
  </div>

  <div id="dashboard" style="display:none">
   <div class="account-layout">
    <div class="account-menu">
     <button class="active" onclick="accountPanel('dashboardPanel',this)">🏠 Dashboard</button>
     <button onclick="accountPanel('profilePanel',this)">👤 My Profile</button>
     <button onclick="accountPanel('coursesPanel',this)">📚 My Courses</button>
     <button onclick="accountPanel('studyPanel',this)">📝 Study Area</button>
     <button class="logout-btn" onclick="logout()">↪ Logout</button>
    </div>
    <div>
     <div id="dashboardPanel" class="account-card account-panel"><h2>WELCOME, <span id="dashName"></span>!</h2><p>Your student account is active on this browser.</p><div class="stat-grid"><div class="stat"><strong id="courseCount">0</strong>Active Courses</div><div class="stat"><strong>₹2,000</strong>Course Price</div><div class="stat"><strong>✓</strong>Account</div></div></div>
     <div id="profilePanel" class="account-card account-panel" style="display:none"><h2>MY PROFILE</h2><p><strong>Name:</strong> <span id="profileName"></span></p><p><strong>Email:</strong> <span id="profileEmail"></span></p></div>
     <div id="coursesPanel" class="account-card account-panel" style="display:none"><h2>MY COURSES</h2><div id="myCourses" class="empty-state">No course selected yet.<br><button class="btn primary" onclick="showView('courses')">BROWSE COURSES</button></div></div>
     <div id="studyPanel" class="account-card account-panel" style="display:none"><h2>STUDY AREA</h2><p>Course videos, notes, tests and assignments can be connected here.</p><button class="btn primary" onclick="showView('courses')">OPEN COURSES</button></div>
    </div>
   </div>
  </div>
 </div></section>
</section>

<footer><strong>COMMERCE CLASSES BY KV SIR</strong><p>© 2026 COMMERCE CLASSES BY KV SIR</p><p>ANAND NAGAR, BAHODAPUR, GWALIOR</p></footer>

<script>
const courses={
 class11:{title:"CLASS 11",subtitle:"CBSE / ICSE",icon:"📘",text:"Commerce learning for Class 11 with Accounts, Economics and Business Studies.",items:["ACCOUNTS","ECONOMICS","BUSINESS STUDIES"]},
 class12:{title:"CLASS 12",subtitle:"CBSE / ICSE",icon:"🎓",text:"Focused Class 12 commerce support with Accounts, Economics and Business Studies.",items:["ACCOUNTS","ECONOMICS","BUSINESS STUDIES"]},
 bcom:{title:"B.COM",subtitle:"COLLEGE",icon:"📊",text:"Commerce subject support with doubt solving and regular practice.",items:["COMMERCE SUBJECTS","DOUBT SUPPORT","REGULAR PRACTICE"]},
 bba:{title:"BBA",subtitle:"COLLEGE",icon:"💼",text:"Business-focused learning support with practice and doubt solving.",items:["BUSINESS SUBJECTS","DOUBT SUPPORT","REGULAR PRACTICE"]},
 mba:{title:"MBA",subtitle:"COLLEGE",icon:"🚀",text:"Management subject support with practice and doubt solving.",items:["MANAGEMENT SUBJECTS","DOUBT SUPPORT","REGULAR PRACTICE"]}
};
let authMode="login",currentCourse=null,currentUser=null;

function showView(name){
 document.querySelectorAll(".view").forEach(v=>v.classList.remove("active"));
 const el=document.getElementById("view-"+name);
 if(el)el.classList.add("active");
 window.scrollTo({top:0,behavior:"smooth"});
}
function openAccount(){showView("account");refreshAccountUI();}
function setAuthMode(mode){
 authMode=mode;
 document.getElementById("fullName").style.display=mode==="signup"?"block":"none";
 document.getElementById("fullName").required=mode==="signup";
 document.getElementById("authButton").textContent=mode==="signup"?"CREATE ACCOUNT":"SIGN IN";
 document.getElementById("loginTab").classList.toggle("active",mode==="login");
 document.getElementById("signupTab").classList.toggle("active",mode==="signup");
}
function submitAuth(e){
 e.preventDefault();
 const email=document.getElementById("email").value.trim().toLowerCase();
 const password=document.getElementById("password").value;
 const name=document.getElementById("fullName").value.trim();
 const key="kvSirAccount_"+email;
 if(authMode==="signup"){
  if(!name)return alert("PLEASE ENTER YOUR NAME.");
  if(localStorage.getItem(key))return alert("ACCOUNT ALREADY EXISTS. PLEASE SIGN IN.");
  const account={name,email,password,courses:[]};
  localStorage.setItem(key,JSON.stringify(account));
  alert("ACCOUNT CREATED SUCCESSFULLY. NOW SIGN IN.");
  document.getElementById("password").value="";
  setAuthMode("login");
 }else{
  const saved=localStorage.getItem(key);
  if(!saved)return alert("ACCOUNT NOT FOUND. PLEASE CREATE AN ACCOUNT FIRST.");
  const account=JSON.parse(saved);
  if(account.password!==password)return alert("INCORRECT PASSWORD.");
  currentUser=account;
  sessionStorage.setItem("kvSirLoggedIn",email);
  refreshAccountUI();
  alert("WELCOME, "+account.name+"!");
 }
}
function refreshAccountUI(){
 const email=sessionStorage.getItem("kvSirLoggedIn");
 if(!email){currentUser=null;document.getElementById("authBox").style.display="block";document.getElementById("dashboard").style.display="none";document.getElementById("accountNav").textContent="SIGN IN";return;}
 const saved=localStorage.getItem("kvSirAccount_"+email);
 if(!saved){sessionStorage.removeItem("kvSirLoggedIn");return refreshAccountUI();}
 currentUser=JSON.parse(saved);
 document.getElementById("authBox").style.display="none";
 document.getElementById("dashboard").style.display="block";
 document.getElementById("accountWelcome").textContent="Welcome, "+currentUser.name;
 document.getElementById("dashName").textContent=currentUser.name;
 document.getElementById("profileName").textContent=currentUser.name;
 document.getElementById("profileEmail").textContent=currentUser.email;
 document.getElementById("accountNav").textContent="ACCOUNT";
 renderCourses();
}
function logout(){
 sessionStorage.removeItem("kvSirLoggedIn");currentUser=null;
 setAuthMode("login");refreshAccountUI();showView("home");
}
function accountPanel(id,btn){
 document.querySelectorAll(".account-panel").forEach(x=>x.style.display="none");
 document.getElementById(id).style.display="block";
 document.querySelectorAll(".account-menu button").forEach(x=>x.classList.remove("active"));
 if(btn)btn.classList.add("active");
}
function openCourse(id){
 currentCourse=id;const c=courses[id];
 document.getElementById("coursePageTitle").textContent=c.title;
 document.getElementById("coursePageSubtitle").textContent=c.subtitle;
 document.getElementById("courseIcon").textContent=c.icon;
 document.getElementById("courseDetailTitle").textContent=c.title+" COURSE";
 document.getElementById("courseDetailText").textContent=c.text;
 document.getElementById("courseDetailList").innerHTML=c.items.map(x=>"<li>"+x+"</li>").join("");
 showView("course");
}
function subscribeCurrentCourse(){
 if(!currentCourse)return;
 if(!currentUser){alert("PLEASE SIGN IN OR CREATE A STUDENT ACCOUNT FIRST.");openAccount();return;}
 const c=courses[currentCourse];
 if(!currentUser.courses)currentUser.courses=[];
 if(!currentUser.courses.includes(c.title))currentUser.courses.push(c.title);
 localStorage.setItem("kvSirAccount_"+currentUser.email,JSON.stringify(currentUser));
 document.getElementById("courseName").value=c.title+" - ₹2,000";
 alert(c.title+" added to your student account. Please use Contact to complete the enquiry.");
 showView("contact");renderCourses();
}
function renderCourses(){
 if(!currentUser)return;
 const box=document.getElementById("myCourses");
 const list=currentUser.courses||[];
 document.getElementById("courseCount").textContent=list.length;
 if(!list.length){box.innerHTML='No course selected yet.<br><button class="btn primary" onclick="showView(\\'courses\\')">BROWSE COURSES</button>';return;}
 box.className="";
 box.innerHTML=list.map(c=>'<div class="account-card" style="margin:10px 0"><strong>'+c+'</strong><p>₹2,000 • Student course</p></div>').join("");
}
function sendWhatsApp(e){
 e.preventDefault();
 const name=document.getElementById("studentName").value;
 const phone=document.getElementById("phone").value;
 const course=document.getElementById("courseName").value;
 const enquiry=document.getElementById("enquiry").value;
 const message="HELLO KV SIR%0A%0ASTUDENT NAME: "+encodeURIComponent(name)+"%0APHONE: "+encodeURIComponent(phone)+"%0ACOURSE: "+encodeURIComponent(course)+"%0AENQUIRY: "+encodeURIComponent(enquiry);
 window.open("https://wa.me/917987116714?text="+message,"_blank");
}
window.addEventListener("load",()=>{
 const email=sessionStorage.getItem("kvSirLoggedIn");
 if(email)refreshAccountUI();
});
</script>
</body>
</html>
