<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="header">
        <div id="container">
            <nav>
                <img src="logo1.png" class="logo">
                <ul>
                    <li><a href="#">Home</a></li>
                    <li><a href="#">About</a></li>
                    <li><a href="#">Services</a></li>
                    <li><a href="#">Portfolio</a></li>
                    <li><a href="#">Contact</a></li>
                </ul>
            </nav>
            <div class="header-text">
                <p>UI/UX Designer</p>
                <h1>Hi, I'm <span>Raghav</span> <br> Sharma From India.</h1>
            </div>
        </div>
    </div>
<!-- --------------about------------- -->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="" alt="">
                </div>
                <div class="about-col-2">
                    <h1 class="subtitle">About Me</h1>
                    <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Unde saepe illo iusto laborum? Odit laudantium eaque necessitatibus voluptates maxime neque blanditiis sapiente, delectus ipsam soluta, asperiores distinctio, fugit officiis sed.</p>
                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('experience')">Experience</p>
                        <p class="tab-links" onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>UI/UX</span><br>Designing web/App Interfaces</li>
                            <li><span>Web Development</span><br>Web app Development</li>
                            <li><span>App Development</span><br>Building Android/IOS apps</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>UI/UX</span><br>Designing web/App Interfaces</li>
                            <li><span>UI/UX</span><br>Designing web/App Interfaces</li>
                            <li><span>UI/UX</span><br>Designing web/App Interfaces</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2021-2026</span><br>B.E. Manufacturing Engineering from BITS Pilani</li>
                            <li><span>2021-2026</span><br>Msc Hons. Biological Sciences from BITS Pilani</li>
                            <!-- <li><span>UI/UX</span><br>Designing web/App Interfaces</li> -->
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </div>
<!-- -----------------------------services------------------------ -->
<div id="services">
    <div class="container">
        <h1 class="subtitle">Services</h1>
        <div class="services-list">
            <div>
                <h2>Web Design</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore consequuntur atque ullam totam, nulla accusamus sit, soluta, ab sequi quos accusantium beatae consequatur deserunt omnis ea officiis culpa quibusdam corporis!</p>
                <a href="#">learn more</a>
            </div>
            <div>
                <h2>UI/UX</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore consequuntur atque ullam totam, nulla accusamus sit, soluta, ab sequi quos accusantium beatae consequatur deserunt omnis ea officiis culpa quibusdam corporis!</p>
                <a href="#">learn more</a>
            </div>
            <div>
                <h2>App Development</h2>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolore consequuntur atque ullam totam, nulla accusamus sit, soluta, ab sequi quos accusantium beatae consequatur deserunt omnis ea officiis culpa quibusdam corporis!</p>
                <a href="#">learn more</a>
            </div>
        </div>
    </div>
</div>
    <script>
        var tablinks = document.getElementsByClassName("tab-links") ;
        var tabcontents = document.getElementsByClassName("tab-contents") ;

        function opentab(tabname){
            for(tablink of tablinks){
                tablink.classList.remove("active-link");
            }
            for(tabcontent of tabcontents){
                tabcontent.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link") ;
            document.getElementById(tabname).classList.add("active-tab") ;
        }
    </script>
</body>
</html>
