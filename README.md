# webdevtask2.0
html code-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>portfolio website - anuj tomer</title>
    <link rel ="stylesheet" href="style.css">
</head>
<body>
<div id="header">
    <div class="container">
        <nav>
            
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">About</a></li>
                <li><a href="#">Services</a></li>
                <li><a href="#">Portfolio</a></li>
                <li><a href="#">Contact</a></li>

                
            </ul>
        </nav>
        <div class="header-text">
            <p>data science enthusiast</p>
            <h1>Hi, I'm <span>Anuj</span><br>from Ajay Kumar Garg Engineering College</h1>
        </div>

    </div>
</div>
<div id="about">
    <div class="container">
        <div class="row">
            <div class="about-col-1">
                <img src="images/logo.jpg">

            </div>
            <div class="about-col-2">
                <hl class="sub-title">About Me</hl>
                <p>Hey , Anuj here , this is my first ever portfolio website . I am hereby look forward to share more about me and update myself throught this personal portfolio website showcasing my skills and qualifications

                </p>
                <div class="tab-titles">
                    <p class="tab-links active-link">Skills</p>
                    <p class="tab-links">Experience</p>
                    <p class="tab-links">Education</p>
                </div>
                <div class="tab-contents">
                    <ul>
                        <li><span>Web Designing</span><br>Designing web pages</li>
                        <li><span>Data Science</span><br>Statistics</li>
                        <li><span>Data Structures</span><br>Language efficiency</li>
                    </ul>
                </div>

            </div>

            </div>

        </div>
    </div>
</div>

    
</body>
</html>
css code-
*{
    margin: 0;
    padding:0;
    font-family: 'Poppins ', sans-serif;
    box-sizing: border-box;


}
body{
    background: #080808;
    color:#fff;

}
#header{
    width:100%;
    height:100vh;
    background-image:url(images/backgroundimg.jpg);
    background-size: cover;
    background-position:center;
}
.container{
    padding: 10px 10%;

}
nav{
    display: flex;
    align-items:center ;
    justify-content: space-between;
    flex-wrap: wrap;

}
nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}
nav ul li a{
    color: #fff;
    text-decoration: none;
    font-size: 18px;
    position:relative;


}
nav ul li a::after{
    content:'';
    width:100%;
    height: 3px;
    background: #ff004f;
    position:absolute;
    left:0;
    bottom:-6px;
    transition:0.5s;
}
nav ul li a:hover::after{
    width:100%;
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
}
.header-text h1{
    font-size: 60px;
    margin-top:20px;

}
#about{
    padding: 80px 0;
    color:#ababab;
}
.row{
    display:flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width:100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}
.subtitle{
    font-size:100px;
    font-weight: 600;
    color:#fff;
}
.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor:pointer;
    position:relative;
}
.tab-links::after{
    content:'';
    width:0;
    height:3px;
    background: absolute;
    left:0;
    bottom:-8px;
    transition:0.5s;
}
.tab-links.active-link::after{
    width: 50%;
}
.tab-contents ul li{
    list-style: none;
    margin: 10px 0;
}
.tab-contents ul li span{
    color: #ff004f;
    font-size: 14px;
}

