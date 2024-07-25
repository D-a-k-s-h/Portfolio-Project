@import url("https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@300&display=swap");

*{
    margin: 0%;
    padding: 0%;
    /* box-sizing: border-box; */
    font-family: be vietnam pro,sans-serif;
}

#wrapper{
    height: 100vh;
    overflow-x: hidden;
}

.container{
    width: 1200px;
    margin: 0 auto;
}

.navbar{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding-top: 1rem;
}

.logo{
    width: 80px;
}

.logo-container{
    display: flex;
    align-items: center;
}

.logo-text{
    margin-left: -1.25rem;
    font-size: 28px;
}

.nav-items{
    display: flex;
    gap: 2rem;
    padding: 0 4em;
}

a{
    text-decoration: none;
}

.nav-items div{
    font-size: 20px;
    font-weight: 500;
    cursor: pointer;
}

.nav-items div a{
    color: black;
    font-family: be vietnam pro,sans-serif;
}

.nav-items div:hover{
    transition: 1ms;
    font-weight: 600;
}

.hero-section{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;

    gap: 5rem;
    margin: 4rem auto;
    padding: 0 1rem;
    padding-bottom: 8rem;
}

.faded-text{
    user-select: none;

    font-size: 7rem;
    color: rgb(231,231,231);
    bottom: -16%;
    left: -5%;
    font-weight: bold;
    transition: all 3s;
}

.hero-section-left{
    display: flex;
    flex-direction: column;
    justify-content: center;
    gap: 2rem;
}

.hero-section-heading{
    font-weight: 500;
    font-size: 35px;
    color: #343d68;
}

.hero-section-sub-heading{
    font-size: 45px;
    line-height: 45px;
}

.running-text{
    color: #4e45d5;
    font-weight: 800;
}

.hero-section-description{
    margin-top: 1rem;
    width: 70%;
    font-weight: 500;
}

.button{
    background-color: orangered;
    width: fit-content;
    color: white;
    padding: 0.8rem 2.3rem;
    box-shadow: 5px 5px 7px 0px #0000003f;
    font-size: 18px;
    cursor: pointer;
    transition: all 0.5s;
    font-weight: 500;
    border: solid 3px transparent;
    position: relative;
    z-index: 1;
}

.button::before{
    content: "";
    position: absolute;
    z-index: -1;
    background-color: #fff;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    z-index: -1;
    transform: scaleX(0);
    transform-origin: left;
    transition: all 0.5s;
}

.button:hover::before{
    transform: scaleX(1);
}

.button:hover{
    color: black;
}

.hero-section-right{
    position: relative;
}

.absolute{
    position: absolute;
}

.user-image img{
    z-index: -8;
}

.user-image{
    padding: 2.5rem;
    filter: grayscale(1);
    transition: all 1s;
    animation: scaleImage 5s linear infinite;
}

@keyframes scaleImage {
    0%{
        filter: grayscale(0);
        transform: scale(1);    
    }
    50%{
        transform: scale(1.1);
        filter: grayscale(1);
        box-shadow: 3px 3px 10px black;
    }
    100%{
        transform: scale(1);
        filter: grayscale(0);
    }
}

.icon-dots{
    z-index: 1;
    bottom: -1rem;
    right: 0;
    animation-name: dots;
    animation-duration: 5s;
    animation-iteration-count: infinite;
}

@keyframes dots{
    0%{
        transform: translateY(0px);
    }
    50%{
        transform: translateY(-15px);
    }
    100%{
        transform: translateY(0px);
    }
}

.icon-cube{
    z-index: 1;
    top: -0.8rem;
    right: 1em;
    animation-name: cube;
    animation-duration: 1s;
    animation-iteration-count: infinite;
}

@keyframes cube {
    0%{
        transform: rotateY(0deg) translateY(0px);
    }
    50%{
        transform: rotateY(180deg) translateY(-12px);
    }
    100%{
        transform: rotateY(360deg) translateY(0px);
    }
}

.icon-circle{
    z-index: 1;
    left: 0;
    bottom: 0;
    animation-name: circle;
    animation-duration: 4s;
    animation-iteration-count: infinite;
}

@keyframes circle {
    0%{
        left: 0;
        bottom: 0;
    }
    50%{
        left: 5%;
        bottom: 10%;
    }
    100%{
        left: 0;
        bottom: 0;
    }
}

.icon-zigzag{
    z-index: 1;
    top: 1.5em;
    left: 0.3em;
    animation-name: zigzag;
    animation-iteration-count: infinite;
    animation-duration: 5s;
}

@keyframes zigzag {
    0%{
        left: 0;
        top: 0;
    }
    50%{
        left: 5%;
        top: 2%;
    }
    100%{
        left: 0;
        top: 0;
    }
}

.icon-plus{
    z-index: 1;
    top: 0.8rem;
    left: 50%;
    animation-name: plus;
    animation-duration: 4s;
    animation-iteration-count: infinite;
}

@keyframes plus{
    50%{
        left: 48%;
        top: 3%;
    }
}

.project-section{
    background-color: rgb(231, 231, 231);
    margin-top: 4rem;
}

.page-header{
    color: rgb(245, 114, 13);
    font-size: 90px;
    text-align: center;
    padding-top: 30px;
}

.project-container{
    max-width: 1200px;
    margin: 0 auto;
    padding: 3rem 0;

    display: flex;
    flex-direction: column;
    gap: 20px;
}

.project-card{
    width: 90%;
    height: 550px;
    background-image: url(images/projects/Project1.png);
    background-size: cover;
    position: relative;
    box-shadow: 0px 0px 40px #1f1f1f;
    margin-bottom: 4.5rem;
}

.project-card::after{
    content: "";
    position: absolute;
    left: 0;
    right: 0;
    bottom: 0;
    top: 0;
    background-color: #1f1f1f9a;
    z-index: 0;
}

.project-card::before{
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: linear-gradient(45deg, #343d68,#343d68be,#343d687c);
    transform: scaleX(0);
    transform-origin: bottom;
    transition: all 0.4s;
    z-index: 1;
}

.project-card:hover::before{
    transform: scaleX(1);
}

.project-number{
    position: absolute;
    font-size: 200px;
    font-weight: 600;
    color: white;
    z-index: 5;
    opacity: 0;
    transition: opacity 0.3s;
}

.project-card:hover .project-number{
    opacity: 1;
}

.project-number-left{
    top: -45px;
    left: -40px;
}


.project-number-right{
    top: -45px;
    right: -40px;
}

.project-content{
    position: absolute;
    display: flex;
    flex-direction: column;
    color: white;
    padding: 2em;
    bottom: 20%;
    z-index: 1;
    gap: 1em;
    transition: all 0.4s;
    transform: scale(1);
}

.project-card:hover .project-content{
    transform: scale(1.1);
}

.project-content-left{
    left: 10%;
}

.project-content-right{
    right: 10%;
}

.project-skills-icons{
    width: 60%;
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
}

.project-skills{
    width: 40px;
}

.project-heading{
    font-size: 50px;
    font-weight: bold;
    line-height: 3rem;
}

.project-sub-heading{
    width: 70%;
    font-style: italic;
    font-size: 16px;
}

.button-grp{
    display: flex;
    gap: 0.9rem;
    align-items: center;
}

.btn-project:hover{
    border: none;
}


.icon{
    display: flex;
    color: white;
    font-size: 35px;
    cursor: pointer;
    transition: color 0.4s;
}

.icon:hover{
    color: orangered;
}

#project2{
    margin-left: 120px;
    background-image: url(images/projects/Project2.png);
}

#project3{
    background-image: url(images/projects/Project3.png);
}

#project4{
    margin-left: 120px;
    background: url(images/projects/Project4.png);
}

.skills-container{
    display: flex;
    position: relative;
    padding: 5rem;
    margin: 10rem auto;
    gap: 30px;
}

.skill-container-left{
    width: 50%;
    display: flex;
    flex-direction: column;
}

.skill-container-right{
    display: flex;
    position: relative;
    width: 50%;
    flex-wrap: wrap;
    gap: 2rem;
}

.skill-fade-text{
    position: absolute;
    font-size: 15em;
    font-style: bold;
    color: rgb(231,231,231);
    bottom: -34.5%;
    right: -25%;
    user-select: none;
    overflow-y: hidden;
}

.blob-style{
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%,-50%);
    z-index: -1;
    animation-name: blob;
    animation-duration: 4s;
    animation-iteration-count: infinite;
}

@keyframes blob {
    50%{
        top: 54%;
        left: 56%;
    }
}

.skills-logo{
    width: 90px;
    transform: scale(1);
    transition: all 0.3s;
}

.skills-logo:hover{
    transform: scale(1.1);
}

.skill-heading{
    font-size: 50px;
    font-style: bold;
    color: orangered;
    line-height: 50px;
}

.caps{
    font-size: 90px;
}

.skill-sub-heading{
    margin-top: 1rem;
    width: 85%;
    text-align: justify; 
}

.contactus-form-container{
    width: 100%;
    background-color: rgb(231, 231, 231);
}

.contactus-heading{
    font-size: 5em;
    color: orangered;
    padding-top: 2rem;
}

.contactus-sub-heading{
    font-size: 3rem;
    color: #343d68aa;
    text-transform: capitalize;
}

.contactus-form-container{
    margin-top: 25px;
    display: flex;
    justify-content: center;
    align-items: center;
}

form{
    display: flex;
    flex-direction: column;
    gap:30px;
    width: 70%;
    margin: 2rem 5rem;
}

.formfield-container{
    width: 100%;
}

.formfield{
    width: 100%;
    height: 42px;
    padding: 0 2rem;
    font-size: 18px;
    border-radius: 5px;
    box-shadow: 2px 2px 10px #1f1f1f;
    font-weight: 500;
    border: none;
    margin-top: 27px;
}

.formfield-textarea{
    height: auto;
    padding-top: 1rem;
}

#submit-btn{
    border: none;
    font-size: 1.4rem;
    margin: 1rem 0;
}

#submit-btn:hover{
    transform: scale(0.9);
}

.submit-icon{
    padding: 0 1rem;
    font-size: 1.5rem;
}

footer{
    position: relative;
    padding: 5rem;
    margin-top: -1px;
    background-color: #343d68;
}

.footer-wrapper{
    display: flex;
    gap: 1rem;
    padding: 1.2rem;
    justify-content: space-between;
    align-items: center;
}

.footer-faded-text{
    position: absolute;
    left: 0;
    bottom: 0;
    color: #535c87;
    user-select: none;
    font-size: 5em;
}

.link-wrapper{
    display: flex;
    gap: 1.2rem;
}

.link-wrapper div a{
    color: white;
    text-decoration: none;
    transition: all 0.4s;
}

.link-wrapper div a:hover{
    color: orangered;
}

.icons-wrapper{
    display: flex;
    gap: 1rem;
}

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio | Codedaksh</title>
    <link rel="stylesheet" href="portfolio.css">
</head>
<body>
    
    <div id="wrapper">

        <div class="container">

            <div class="navbar"> 

                <div class="logo-container">
                    <img src="images/userAsset/NavLogo.jpg" class="logo"/>
                    <div class="logo-text">ohn doe</div>
                </div>

                <div class="nav-items">
                    <div><a href="#projects">Projects</a></div>
                    <div><a href="#skills">Skills</a></div>
                    <div><a href="#contactme">Contact Me</a></div>
                </div>

            </div>

            <div class="hero-section">

                <div class="hero-section-left">

                    <div class="hero-section-heading">Hi!! John Doe </div>
    
                    <div class="hero-section-heading hero-section-sub-heading">
                        I am a <span class="running-text"></span> 
                    </div>
    
                    <div class="hero-section-description">
                        I'm a software developer and here is my portfolio website. 
                        Here you'll learn about my journey as a software developer.
                    </div>
    
                    <div><button class="button">Hire Me</button></div>
    
                </div>
    
                <div class="hero-section-right">
                    <div class="absolute icons icon-dots">
                        <img src="images/userAsset/dots.png" alt="">
                    </div>
    
                    <div class="absolute icons icon-cube">
                        <img src="images/userAsset/cube.png" alt="">
                    </div>

                    <div class="absolute icons icon-circle">
                        <img src="images/userAsset/circle.png" alt="">
                    </div>
    
                    <div class="absolute icons icon-zigzag">
                        <img src="images/userAsset/zigzags.png" alt="">
                    </div>
    
                    <div class="absolute icons icon-plus">
                        <img src="images/userAsset/plus.png" alt="">
                    </div>
    
                    <div class="user-image">
                        <img src="images/userAsset/UserImage.png" alt="">
                    </div>
    
                </div>

                <div class="absolute faded-text">John Doe</div>

            
            </div>

        </div>  

        <div class="project-section" id="projects">
            <h2 class="page-header">Projects</h2>

            <div class="project-container">
                <div class="project-card" id="project1">
                    <div class="project-number project-number-right">01</div>

                    <div class="project-content project-content-left">

                        <div class="project-skills-icons">
                            <img src="images/stack/HTML.png" class="project-skills">
                            <img src="images/stack/CSS.png" class="project-skills">
                            <img src="images/stack/Express.png" class="project-skills">
                            <img src="images/stack/Javascript.svg" class="project-skills">
                            <img src="images/stack/MongoDB.svg" class="project-skills">
                            <img src="images/stack/Redux.svg" class="project-skills">
                            <img src="images/stack/Vercel.svg" class="project-skills">
                            <img src="images/stack/NextJsCircle.png" class="project-skills">
                            <img src="images/stack/Tailwind.png" class="project-skills">
                            <img src="images/stack/NodeJs.svg" class="project-skills">
                        </div>

                        <h2 class="project-heading">Tint & Orange</h2>

                        <div class="project-sub-heading">It's a car modification company which provides 
                            sheets to protect your car from scratch
                        </div>
                        
                        <div class="button-grp">
                            <button class="button btn-project">Read More</button>
                            <a href="" >
                            <i title="GitHubLink" class="fa-brands fa-github icon"></i>
                            </a>
                            <a href="">
                            <i title="Live Link" class="fa-solid fa-link icon"></i>
                            </a>
                        </div>

                    </div>

                </div>

                <div class="project-card" id="project2">
                    <div class="project-number project-number-left">02</div>

                    <div class="project-content project-content-right">

                        <div class="project-skills-icons">
                            <img src="images/stack/HTML.png" class="project-skills">
                            <img src="images/stack/CSS.png" class="project-skills">
                            <img src="images/stack/Javascript.svg" class="project-skills">
                            <img src="images/stack/Redux.svg" class="project-skills">
                            <img src="images/stack/NextJsCircle.png" class="project-skills">
                            <img src="images/stack/Tailwind.png" class="project-skills">
                        </div>

                        <h2 class="project-heading">Breaking Copyrights</h2>

                        <div class="project-sub-heading">A platform to download copyright free youtube music</div>
                        
                        <div class="button-grp">
                            <button class="button btn-project">Read More</button>
                            <a href="">
                            <i title="GitHubLink" class="fa-brands fa-github icon"></i>
                            <span class="sr-only">GitHubLink</span>
                            </a>
                            <a href="">
                            <i title="Live Link" class="fa-solid fa-link icon"></i>
                            <span class="sr-only">Live Link</span>
                            </a>
                        </div>

                    </div>

                </div>

                <div class="project-card" id="project3">
                    <div class="project-number project-number-right">03</div>

                    <div class="project-content project-content-left">

                        <div class="project-skills-icons">
                            <img src="images/stack/HTML.png" class="project-skills">
                            <img src="images/stack/CSS.png" class="project-skills">
                            <img src="images/stack/Javascript.svg" class="project-skills">
                            <img src="images/stack/Vercel.svg" class="project-skills">
                            <img src="images/stack/NextJsCircle.png" class="project-skills">
                            <img src="images/stack/Tailwind.png" class="project-skills">
                        </div>

                        <h2 class="project-heading">Isha Tattva</h2>

                        <div class="project-sub-heading">A website for interior designer to showcase her works and
                            samples
                        </div>
                        
                        <div class="button-grp">
                            <button class="button btn-project">Read More</button>
                            <a href="">
                            <i title="GitHubLink" class="fa-brands fa-github icon"></i>
                            <span class="sr-only">GitHubLink</span>
                            </a>
                            <a href="">
                            <i title="Live Link" class="fa-solid fa-link icon"></i>
                            <span class="sr-only">Live Link</span>
                            </a>
                        </div>

                    </div>

                </div>

                <div class="project-card" id="project4">
                    <div class="project-number project-number-left">04</div>

                    <div class="project-content project-content-right">

                        <div class="project-skills-icons">
                            <img src="images/stack/Vercel.svg" class="project-skills">
                            <img src="images/stack/NextJsCircle.png" class="project-skills">
                            <img src="images/stack/Tailwind.png" class="project-skills">
                        </div>

                        <h2 class="project-heading">Grannit</h2>

                        <div class="project-sub-heading">A architectural website to plan your buildings or home
                            (Hebrew Language)
                        </div>
                        
                        <div class="button-grp">
                            <button class="button btn-project">Read More</button>
                            <a href="">
                            <i title="GitHubLink" class="fa-brands fa-github icon"></i>
                            <span class="sr-only">GitHubLink</span>
                            </a>
                            <a href="">
                            <i title="Live Link" class="fa-solid fa-link icon"></i>
                            <span class="sr-only">Live Link</span>
                            </a>
                        </div>

                    </div>

                </div>

            </div>
            
        </div>

        <div id="skills" class="container skills-container">
            <div class="skill-fade-text">Skills</div>

            <div class="skill-container-left">
                
                <h2 class="skill-heading"><span class="caps">M</span>e and
                    <br>
                    MyTech Stack
                </h2>

                <div class="skill-sub-heading">
                    <p>
                        Hi Everyone My name is John Doe I am a Full Stack Web Developer I
                        have been working for last 3 Years and Currently I am working with a
                        Budding Startup in USA and a full Time Freelancer. Currently I am
                        working on NextJs and Making Beautiful UI-UX are my fey features
                    </p>
                    <br>
                    <p>
                        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Non
                        doloremque aspernatur, maiores voluptatum minus laudantium?
                        Perspiciatis accusamus minima porro dolores necessitatibus, magni
                        dolorem et qui veniam nulla sequi molestiae maxime.
                    </p>
                    <br>
                    <p>
                        Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis quidem
                        quos ullam veritatis voluptates tenetur qui ipsa nulla culpa itaque?
                    </p>

                </div>

            </div>

            <div class="skill-container-right">
                <img src="./images/userAsset/blob vector.png" class="blob-style" alt="" />

                <img src="./images/stack/HTML.png" alt="" class="skills-logo" />
                <img src="./images/stack/CSS.png" alt="" class="skills-logo" />
                <img src="./images/stack/Javascript.svg" alt="" class="skills-logo" />
                <img src="./images/stack/React.png" alt="" class="skills-logo" />
                <img src="./images/stack/NodeJs.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Next.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Redux.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Tailwind.png" alt="" class="skills-logo" />
                <img src="./images/stack/Bootstrap.svg" alt="" class="skills-logo" />
                <img src="./images/stack/MaterialUI.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Express.png" alt="" class="skills-logo" />
                <img src="./images/stack/Git.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Github.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Graphql.svg" alt="" class="skills-logo" />
                <img src="./images/stack/MongoDB.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Vercel.svg" alt="" class="skills-logo" />
                <img src="./images/stack/ChartJs.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Bash.svg" alt="" class="skills-logo" />
                <img src="./images/stack/Docker.svg" alt="" class="skills-logo" />
                <img src="./images/stack/K8s.svg" alt="" class="skills-logo" />
            </div>

        </div>

        <div class="contactus-form-container" id="contactme">
            <div class="container">
                <h2 class="contactus-heading">Contact Us</h2>
                <h3 class="contactus-sub-heading">Questions, thoughts, or just want to say hello?</h3>

                <div class="contactus-form">
                    <form action="">
                        <div class="formfield-container">
                            <input type="text" class="formfield" placeholder="Enter Your Name">
                            <input type="email" class="formfield" placeholder="Enter Your Email">
                            <input type="text" class="formfield" placeholder="Enter Your Subject">
                            <textarea class="formfield formfield-textarea" id="" rows="10" cols="30" 
                            placeholder="Enter Your Text"></textarea>
                        </div>

                        <button type="submit" class="button btn-project" id="submit-btn">Send Message<i class="submit-icon fa-solid fa-paper-plane"></i></button>

                    </form>
                </div>
                


            </div>
        </div>

        <footer>
            <div class="container">
                <div class="footer-wrapper">
                    <div class="footer-faded-text">John Doe</div>

                    <div class="link-wrapper">
                        <div><a href="#projects">Projects</a></div>
                        <div><a href="#skills">Skills</a></div>
                        <div><a href="#contactme">Contact Me</a></div>
                    </div>

                    <div class="icons-wrapper">
                        <i class="fa-brands fa-linkedin icon"></i>
                        <i class="fa-brands fa-github icon"></i>
                        <i class="fa-brands fa-twitter icon"></i>
                        <i class="fa-brands fa-instagram icon"></i>
                        <i class="fa-solid fa-envelope icon"></i>
                    </div>
                </div>
            </div>
        </footer>

    </div>
    <script src="https://cdn.jsdelivr.net/npm/typed.js@2.0.12"></script>
    <script src="https://kit.fontawesome.com/58a810656e.js" crossorigin="anonymous"></script>
    <script>
    var typeData = new Typed(".running-text", {
    strings: [
    "Full Stack Developer",
    "Web Developer",
    "Backend Developer",
    "Coder",
    ],

    loop: true,
    typeSpeed: 50,
    backSpeed: 50,
    backDelay: 1000,
    });
    </script>


</body>
</html>
