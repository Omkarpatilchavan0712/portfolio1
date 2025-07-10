<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>students - devloper pertfolio</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Manufacturing+Consent&display=swap" rel="stylesheet">
    <style>
        *{
            margin: 0;
            padding: 0;
        }
    body
    {
        background-color: rgb(0,0,33);
        color: white;
        font-family: 'poppins',sans-serif;
    }
    nav {
        display: flex;
        justify-content: space-around;
        align-items: center;
        height: 80px;
        background-color: rgb(0, 0, 68);
    }
    nav ul{
        display: flex;
        justify-content: center;
    }
    nav ul li{
        list-style: none;
        margin: 0 23px;
    }
    nav ul li a{
        text-decoration: none;
        color: white;
    }
    nav ul li a:hover{
        color: rgb(230, 137, 137);
        font-size: 1.02rem;
    }
    main hr{
        border: 0;
        background: #9c97f1;
        height: 1.2px;
        margin: 40px,84px;
    }
    .left{
        font-size: 1.5rem;
    }
    .firstsection{
        display: flex;
        justify-content: space-around;
        margin: 130px 0;
        align-items: center;

        }
    .firstsection > div{
        width: 30%;
    }
    .leftsection{
        font-size: 2rem;
        width: 34%;
        margin: 50px,0;
    }
    .leftsection .buttons{
        padding: 25px 0;
    }
    .leftsection .btn{
        padding: 12px;
        background: rgb(133, 103, 232);
        color: white;
        border: 2px solid white;
        border-radius: 9px 14px;
        font-size: 12px;
        cursor: pointer;
    }
    .rightsection{
        width: 34%;
    }
    .rightsection img{
        width: 80%;
        margin: 50%,0;
    }
    .purple{
        color: rgb(86, 57, 189);
    }
    .text-gray{
       color: gray;
    }
    #element{
        color: rgb(86, 57, 189);
    }
    .secondsection{
        max-width: 80vw;
        margin: auto;
        height: 80vh;
    }
    .secondsection h1{
        font-size: 1.5rem;
    }
    .secondsection .box{
        background: rgb(251, 250, 252);
        width: 70vw;
        height: 2px;
        margin: 56px 0;
        display: flex;
    }
    .secondsection .vertical{
        height: 93px;
        width: 1px;
        background-color: rgb(254, 252, 255);
        margin: 0 100px;
    }
    .vertical-title{
        position: relative;
        top: 75px;
        width: 150;
        font-size: 20px;
        
    }
    .vertical-desc{
        position: relative;
        top: 86px;
        color: gray;
        width: 180px;
        font-size: 9px;
    }
    footer{
        background-color: rgb(0, 8, 85);
        height: 220px;
    }
    .footer{
        display: flex;
        padding:  23px 122px;
        justify-content: space-evenly;
    }
    .footer ul{
        list-style: none;
    }
    .footer> div{
        width: 223px;
    }
    footer .footer-rights{
        text-align: center;
        color: white;
        padding: 12px 0;
    }
    </style>
</head>
<body>
    <header>
        <nav>
            <div class="left">Priya's portfolio</div>
            <div class="right">
                <ul>
                    <li><a href="/">HOME</a></li>
                    <li><a href="/About.html">ABOUT</a></li>
                    <li><a href="/Service.html">SERVICES</a></li>
                    <li><a href="/Project.html">PROJECTS</a></li>
                    <li><a href="/Contact Me.html">CONTACTS ME</a></li>
                </ul>
            </div>
        </nav>
    </header>
    
</body>
<header>
    <main>
        <main>
        <section class="firstsection">
            <div class="leftsection">
            HI,my name is <span class="purple">PRIYA</span>
            <div>
                and i am a Passionate
                <div>web Devaloper</div>
                 <span id="element"></span>
                 <div class="buttons">
                    <button class="btn">Download Resume</button>
                    <button class="btn"> Visit Github</button>
                 </div>
            </div>
            </div>
            <div class="rightsection">
        <img src="bg.png3.png">
            </div>
        </section>
        <hr>
    <section class="secondsection">
        <span class="text-gray">what i have done so far</span>
        <h1>
            Past experience
        <div class="box">
            <div class="vertical">
                <img class="image-top" src="" alt="">
                <div class="vertical-title">
                    HTML Devaloper 
                    <span>(2010-2012)</span>
                </div>
                <div class="vertical-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Debitis pariatur necessitatibus voluptas porro illum reiciendis autem deleniti enim est error in quos,
                    quia molestias, dolore hic incidunt. Illum, nesciunt ipsam.
        
                </div>
            </div>
        <div class="vertical">
            <img class="image-top" src="" alt="">
                <div class="vertical-title">
                    Frontend Devaloper 
                    <span>(2012-2014)</span>
                </div>
                <div class="vertical-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Debitis pariatur necessitatibus voluptas porro illum reiciendis autem deleniti enim est error in quos,
                    quia molestias, dolore hic incidunt. Illum, nesciunt ipsam.
        
                </div>
        </div>
        <div class="vertical">
            <img class="image-top" src="" alt="">
                <div class="vertical-title">
                    Node.js Devaloper 
                    <span>(2014-2016)</span>
                </div>
                <div class="vertical-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Debitis pariatur necessitatibus voluptas porro illum reiciendis autem deleniti enim est error in quos,
                    quia molestias, dolore hic incidunt. Illum, nesciunt ipsam.
        
                </div>
        </div>
        <div class="vertical">
            <img class="image-top" src="" alt="">
                <div class="vertical-title">
                    Backend devloper
                    <span>(2016-2018)</span>
                </div>
                <div class="vertical-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Debitis pariatur necessitatibus voluptas porro illum reiciendis autem deleniti enim est error in quos,
                    quia molestias, dolore hic incidunt. Illum, nesciunt ipsam.
        
                </div>
        </div>
        <div class="vertical">
            <img class="image-top" src="" alt="">
                <div class="vertical-title">
                    HTML Devaloper
                    <span>(2018-2020)</span> 
                </div>
                <div class="vertical-desc">
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. 
                    Debitis pariatur necessitatibus voluptas porro illum reiciendis autem deleniti enim est error in quos,
                    quia molestias, dolore hic incidunt. Illum, nesciunt ipsam.
        
                </div>
        </div>
        </div>
    </section>
    </main>
    </main>
    <footer>
        <div class="footer">
            <div class="footer-first">
                PRIYA'S Devaloper portfolio
            </div>
            <div class="footer-second">
            <ul>
            <li>HOME</li>
            <li>ABOUT</li>
            <li>SERVICES</li>
            <li>CONTACTS</li>
            </ul>
            </div>
            <div class="footer-third"><ul>
            <li>HOME</li>
            <li>ABOUT</li>
            <li>SERVICES</li>
            <li>CONTACTS</li>
            </ul></div>
            <div class="footer-fourth"><ul>
            <li>HOME</li>
            <li>ABOUT</li>
            <li>SERVICES</li>
            <li>CONTACTS</li>
            </ul></div>
        </div>
        <div class="footer"></div>
        <div class="footer-rights">
        Copyrights &#169; www.priya's portfolio.com | All Right Reserved
        </div>
    </footer>
    <script src="https://unpkg.com/typed.js@2.1.0/dist/typed.umd.js"></script>
    <!-- Setup and start animation! -->
  <script>
    var typed = new Typed('#element', {
      strings: ['Web Devaloper','Video editor','Web Designer','video editor'],
      typeSpeed: 50,
    });
  </script>
</header>
</html>
<section id="about" 
style="background-color: rgb(156, 131, 246);
        display: flex;
        justify-content: space-around;
        margin: 110px 0;
        align-items: center;
  <h2>About Me</h2>">
  <div class="about-content">
    <img src="piu.png" alt="" class="profile-photo">
    <div class="about-text">
      <h3>Hello! I'm Priya Rajegore</h3>
      <p>
        I'm a passionate <strong>Frontend Web Developer</strong> with 3+ years of experience building
        modern, responsive websites and web applications using technologies like
        <strong>HTML</strong>, <strong>CSS</strong>, <strong>JavaScript</strong>, and <strong>React</strong>.
      </p>
      <p>
        I love solving real-world problems through clean code and elegant design. I'm also familiar with UI/UX principles and love collaborating with designers to bring ideas to life.
      </p>
      <p>
        When I'm not coding, I enjoy reading tech blogs, exploring design trends, and learning new tools to improve my craft.
      </p>
      <p>
        📬 I'm currently open to freelance and full-time opportunities. <a href="#contact">Contact me here</a>!
      </p>
    </div>
  </div>
</section>
<style>
     *{
            margin: 0;
            padding: 0;
        }
    body
    {
        background-color: rgb(156, 131, 246);
        color: white;
        font-family: 'poppins',sans-serif;
    }
#about {
  padding: 50px 20px;
  background-color: #f9f9f9;
}

.about-content {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 20px;
}

.profile-photo {
  width: 200px;
  border-radius: 10px;
}

.about-text {
  max-width: 600px;
}

.about-text h3 {
  margin-top: 0;
  color: #333;
}
</style>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Services</title>
</head>
<body>

    <section class="services-section"
    style="background-color:#00bcd4
    color: #333;
    line-height: 1.6;">
        <h2 class="section-title">My Services</h2>
        <div class="services-container">

            <div class="service-card">
                <div class="icon">💻</div>
                <h3>Web Development</h3>
                <p>I create responsive and high-performing websites using HTML, CSS, JavaScript, and modern frameworks.</p>
            </div>

            <div class="service-card">
                <div class="icon">🎨</div>
                <h3>UI/UX Design</h3>
                <p>I design intuitive user interfaces with a focus on user experience and accessibility.</p>
            </div>

            <div class="service-card">
                <div class="icon">⚙️</div>
                <h3>SEO Optimization</h3>
                <p>I optimize websites for better ranking and performance on search engines like Google.</p>
            </div>

        </div>
    </section>

</body>
</html>
<style>
/* General Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'poppins',sans-serif;
}

/* Background and Layout */
body {
    background-color: #f4f6f8;
    color: #333;
    box-sizing: border-box;
    font-family: sans-serif;
}

.services-section {
    background-color: #1e1e2f; /* Dark background */
    color: #fff;
    padding: 60px 20px;
    text-align: center;
}

.section-title {
    font-size: 2.5rem;
    margin-bottom: 40px;
    color: #00bcd4;
}

/* Services Grid */
.services-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
}

/* Individual Card */
.service-card {
    background-color: #2e2e42;
    border-radius: 10px;
    padding: 30px;
    width: 300px;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
}

.service-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 25px rgba(0, 188, 212, 0.3);
}

.icon {
    font-size: 3rem;
    margin-bottom: 15px;
}

h3 {
    font-size: 1.5rem;
    margin-bottom: 15px;
    color: #00bcd4;
}

p {
    font-size: 1rem;
    color: #ccc;
}
</style>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Projects</title>
    <link rel="stylesheet" href="projects.css">
</head>
<body>

    <section class="projects-section">
        <h2 class="section-title">My Projects</h2>
        <div class="projects-container">

            <!-- Project 1 -->
            <div class="project-card">
                <img src="project1.jpg" alt="Project 1 Screenshot">
<style>
/* Basic Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

/* Body */
body {
    background-color: #f4f6f8;
    color: #333;
}

/* Projects Section */
.projects-section {
    background-color: #121212; /* Dark theme */
    color: #fff;
    padding: 60px 20px;
    text-align: center;
}

.section-title {
    font-size: 2.5rem;
    margin-bottom: 40px;
    color: #ff9800;
}

/* Project Container */
.projects-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 30px;
}

/* Project Card */
.project-card {
    background-color: #1e1e1e;
    border-radius: 10px;
    width: 300px;
    padding: 20px;
    text-align: left;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.4);
}

.project-card:hover {
    transform: translateY(-10px);
    box-shadow: 0 10px 25px rgba(255, 152, 0, 0.3);
}

.project-card img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 8px;
    margin-bottom: 15px;
}

.project-card h3 {
    font-size: 1.3rem;
    margin-bottom: 10px;
    color: #ff9800;
}

.project-card p {
    font-size: 1rem;
    color: #ccc;
}
</style>
 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Me</title>
    <link rel="stylesheet" href="contact.css">
</head>
<body>

    <section class="contact-section">
        <div class="container">
            <h2 class="contact-title">Contact Me</h2>
            <p class="contact-subtitle">Feel free to reach out using the form below.</p>

            <form class="contact-form">
                <input type="text" name="name" placeholder="Your Name" required>
                <input type="email" name="email" placeholder="Your Email" required>
                <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

</body>
</html>
<style>
    /* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Segoe UI', sans-serif;
}

/* Full Page Background */
body {
    background-color: #0f172a; /* Dark navy background */
    color: #ffffff;
}

/* Contact Section */
.contact-section {
    min-height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 60px 20px;
}

.container {
    max-width: 600px;
    width: 100%;
    background-color: #1e293b;
    padding: 40px;
    border-radius: 12px;
    box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
}

/* Title and Subtitle */
.contact-title {
    font-size: 2.5rem;
    margin-bottom: 10px;
    color: #38bdf8;
    text-align: center;
}

.contact-subtitle {
    text-align: center;
    margin-bottom: 30px;
    color: #cbd5e1;
}

/* Form Styles */
.contact-form input,
.contact-form textarea {
    width: 100%;
    padding: 12px 15px;
    margin-bottom: 20px;
    border: none;
    border-radius: 8px;
    background-color: #334155;
    color: #fff;
    font-size: 1rem;
}

.contact-form input::placeholder,
.contact-form textarea::placeholder {
    color: #94a3b8;
}

.contact-form button {
    width: 100%;
    padding: 12px;
    border: none;
    background-color: #38bdf8;
    color: #0f172a;
    font-size: 1.1rem;
    border-radius: 8px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

.contact-form button:hover {
    background-color: #0ea5e9;
}

</style>


 
# portfolio1
personal portfolio1
