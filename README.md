

<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>College Website</title>

  <style>

    *{
      margin:0;
      padding:0;
      box-sizing:border-box;
      font-family:Arial;
    }

    body{
      background:#f1f5f9;
    }

    /* NAVBAR */

    nav{
      width:100%;
      background:#0f172a;
      padding:20px 8%;
      display:flex;
      justify-content:space-between;
      align-items:center;
      position:fixed;
      top:0;
      z-index:1000;
    }

    .logo{
      color:white;
      font-size:30px;
      font-weight:bold;
    }

    .logo span{
      color:#38bdf8;
    }

    nav ul{
      display:flex;
      list-style:none;
      gap:25px;
    }

    nav ul li a{
      color:white;
      text-decoration:none;
      font-size:18px;
      transition:.3s;
    }

    nav ul li a:hover{
      color:#38bdf8;
    }

    /* HERO SECTION */

    .hero{
      width:100%;
      height:100vh;
      background:
      linear-gradient(rgba(0,0,0,.6),rgba(0,0,0,.6)),
      url("https://images.unsplash.com/photo-1523050854058-8df90110c9f1?q=80&w=2070&auto=format&fit=crop");
      background-size:cover;
      background-position:center;
      display:flex;
      justify-content:center;
      align-items:center;
      text-align:center;
      color:white;
      padding:20px;
    }

    .hero-content h1{
      font-size:65px;
      margin-bottom:20px;
    }

    .hero-content span{
      color:#38bdf8;
    }

    .hero-content p{
      max-width:700px;
      margin:auto;
      line-height:1.8;
      font-size:18px;
      margin-bottom:30px;
    }

    .btn{
      display:inline-block;
      padding:14px 35px;
      background:#38bdf8;
      color:white;
      text-decoration:none;
      border-radius:8px;
      margin:10px;
      transition:.3s;
      font-weight:bold;
    }

    .btn:hover{
      background:#0284c7;
      transform:translateY(-5px);
    }

    /* COURSES */

    .courses{
      padding:100px 8%;
    }

    .title{
      text-align:center;
      margin-bottom:50px;
    }

    .title h2{
      font-size:40px;
      color:#0f172a;
    }

    .title p{
      color:gray;
      margin-top:10px;
    }

    .course-box{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
      gap:30px;
    }

    .card{
      background:white;
      padding:30px;
      border-radius:15px;
      box-shadow:0 5px 20px rgba(0,0,0,.1);
      transition:.4s;
    }

    .card:hover{
      transform:translateY(-10px);
    }

    .card h3{
      margin-bottom:15px;
      color:#0f172a;
    }

    .card p{
      color:#555;
      line-height:1.7;
    }

    /* NOTICE */

    .notice{
      background:#dbeafe;
      padding:100px 8%;
    }

    .notice-box{
      background:white;
      padding:30px;
      border-radius:15px;
      box-shadow:0 5px 20px rgba(0,0,0,.1);
    }

    .notice-item{
      display:flex;
      justify-content:space-between;
      padding:18px 0;
      border-bottom:1px solid #ddd;
    }

    /* GALLERY */

    .gallery{
      padding:100px 8%;
    }

    .gallery-box{
      display:grid;
      grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
      gap:20px;
    }

    .gallery-box img{
      width:100%;
      height:250px;
      object-fit:cover;
      border-radius:15px;
      transition:.4s;
    }

    .gallery-box img:hover{
      transform:scale(1.05);
    }

    /* FOOTER */

    footer{
      background:#0f172a;
      color:white;
      text-align:center;
      padding:30px;
    }

    footer p{
      margin-top:10px;
      color:#cbd5e1;
    }

    /* RESPONSIVE */

    @media(max-width:900px){

      nav{
        flex-direction:column;
      }

      nav ul{
        margin-top:15px;
        flex-wrap:wrap;
        justify-content:center;
      }

      .hero-content h1{
        font-size:42px;
      }

    }

  </style>

</head>

<body>

  <!-- NAVBAR -->

  <nav>

    <div class="logo">
      Vidya<span>Tech</span>
    </div>

    <ul>
      <li><a href="#">Home</a></li>
      <li><a href="#">Courses</a></li>
      <li><a href="#">Notice</a></li>
      <li><a href="#">Gallery</a></li>
      <li><a href="#">Contact</a></li>
    </ul>

  </nav>

  <!-- HERO SECTION -->

  <section class="hero">

    <div class="hero-content">

      <h1>
        Build Your <span>Future</span>
      </h1>

      <p>
        VidyaTech College provides quality education,
        modern labs, industry training and excellent placements.
      </p>

      <a href="#" class="btn">Apply Now</a>
      <a href="#" class="btn">Explore Courses</a>

    </div>

  </section>

  <!-- COURSES -->

  <section class="courses">

    <div class="title">
      <h2>Our Courses</h2>
      <p>Professional courses for successful careers.</p>
    </div>

    <div class="course-box">

      <div class="card">
        <h3>BCA</h3>
        <p>
          Learn programming, web development,
          databases and software engineering.
        </p>
      </div>

      <div class="card">
        <h3>B.Tech</h3>
        <p>
          Modern engineering education with
          innovation and placement opportunities.
        </p>
      </div>

      <div class="card">
        <h3>BBA</h3>
        <p>
          Build management and leadership skills
          for future business success.
        </p>
      </div>

    </div>

  </section>

  <!-- NOTICE -->

  <section class="notice">

    <div class="title">
      <h2>Notice Board</h2>
      <p>Latest announcements and updates.</p>
    </div>

    <div class="notice-box">

      <div class="notice-item">
        <span>Semester Exams Start From 15 August</span>
        <span>New</span>
      </div>

      <div class="notice-item">
        <span>Admissions Open For 2026</span>
        <span>10 Aug</span>
      </div>

      <div class="notice-item">
        <span>Campus Placement Drive Next Week</span>
        <span>8 Aug</span>
      </div>

      <div class="notice-item">
        <span>Independence Day Celebration</span>
        <span>5 Aug</span>
      </div>

    </div>

  </section>

  <!-- GALLERY -->

  <section class="gallery">

    <div class="title">
      <h2>Campus Gallery</h2>
      <p>Explore our beautiful campus.</p>
    </div>

    <div class="gallery-box">

      <img src="https://images.unsplash.com/photo-1523240795612-9a054b0db644?q=80&w=1974&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1517486808906-6ca8b3f04846?q=80&w=1974&auto=format&fit=crop">

      <img src="https://images.unsplash.com/photo-1498243691581-b145c3f54a5a?q=80&w=2070&auto=format&fit=crop">

    </div>

  </section>

  <!-- FOOTER -->

  <footer>

    <h2>VidyaTech College</h2>

    <p>
      Empowering students with education and innovation.
    </p>

    <p>
      © 2026 All Rights Reserved
    </p>

  </footer>

  <!-- JAVASCRIPT -->

  <script>

    // NAVBAR SHADOW

    window.addEventListener("scroll",function(){

      let nav=document.querySelector("nav");

      if(window.scrollY>50){

        nav.style.boxShadow="0 5px 20px rgba(0,0,0,.3)";

      }

      else{

        nav.style.boxShadow="none";

      }

    });

    // BUTTON CLICK

    let btn=document.querySelectorAll(".btn");

    btn.forEach(function(button){

      button.addEventListener("click",function(){

        alert("Admission Form Coming Soon!");

      });

    });

  </script>

</body>

</html>
