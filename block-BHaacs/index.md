<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <script src="script.js"></script>
   <header>
    <div class="container">
<div class="brand">
<h3>TrackL</h3></div>

<div class= "navbar">
    <div class="another">
    <span onclick="hamburgerMenu()">&#9776;</span>
<ul id="menu">
<li><a href="#">Feature</a></li>
<li><a href="#">Pricing</a></li>
<li><a href="#">About</a></li>
<li><a href="#">Help</a></li>
</ul>
    </div>
</div>
</div>
<div class="hero">
<h1>Track The Learning  <br> Process schedule</h1>
<button>Get 30 Days Trial</button>
</div>
   </header>
<div class="hero-img">
<img src="hero (1).png" alt="error"/></div>

</body>
</html>


/* http://meyerweb.com/eric/tools/css/reset/ 
   v2.0 | 20110126
   License: none (public domain)
*/

html, body, div, span, applet, object, iframe,
h1, h2, h3, h4, h5, h6, p, blockquote, pre,
a, abbr, acronym, address, big, cite, code,
del, dfn, em, img, ins, kbd, q, s, samp,
small, strike, strong, sub, sup, tt, var,
b, u, i, center,
dl, dt, dd, ol, ul, li,
fieldset, form, label, legend,
table, caption, tbody, tfoot, thead, tr, th, td,
article, aside, canvas, details, embed, 
figure, figcaption, footer, header, hgroup, 
menu, nav, output, ruby, section, summary,
time, mark, audio, video {
	margin: 0;
	padding: 0;
	border: 0;
	font-size: 100%;
	font: inherit;
	vertical-align: baseline;
}
/* HTML5 display-role reset for older browsers */
article, aside, details, figcaption, figure, 
footer, header, hgroup, menu, nav, section {
	display: block;
}
body {
	line-height: 1;
}
ol, ul {
	list-style: none;
}
blockquote, q {
	quotes: none;
}
blockquote:before, blockquote:after,
q:before, q:after {
	content: '';
	content: none;
}
table {
	border-collapse: collapse;
	border-spacing: 0;
}

/*starts here*/
@font-face{font-family: "open sans regular";
    src: url(Inter-Medium.ttf);
}
body{
    font-family: "open sans regular";
}
header{background-color: rgb(9, 154, 190);
    max-width: 1370px;
    height: 600px;
    position: relative;
}
h3{
    font-size: 20px;
    color: white;
}
.container{
    display: flex;
    justify-content: space-around;
}
ul,li,a{display: inline;
margin-left: 8px;
text-decoration: none;
color: white;
}
.brand{ margin-top: 10px;
}

.navbar{margin-top: 10px;}

h1{font-size: 40px;
    color: white;
    text-align: center;
}

button{margin-left: 580px;
margin-top: 20px;
padding: 20px 40px;
color: navy;
border-radius: 8px;
border: none;
font-size: 15px;
font-weight: 600;
}
.hero{margin-top: 100px;}

img{width: 700px;
    height: 500px;

}
.hero-img{ margin-left:330px ;
position: absolute;
top: 240px;
max-width: 100%;
}

span{margin-left: 80px;
margin-top: 10px;
font-size: 20px;
color: white;
cursor: pointer;
display: none;
}

@media (max-width :800px) {
    span{display: block;}
ul,li,a{
    display: block;
    font-size: 10px;
}
ul{display: none;}
span{margin:0px 0px;
margin-right: 20px;
vertical-align: middle;
}
li{margin-top: 10px;
margin-right: 30px;
}

header{background-color: rgb(9, 154, 190);
    max-width: 800px;
    height: 400px;
    position: relative;
}
button{
    margin-top: 20px;
    padding: 10px 20px;
    color: navy;
    border-radius: 8px;
    border: none;
    font-size: 10px;
    font-weight: 400;
    }

h1{font-size: 14px;
        color: white;
        text-align: center;
    }
    img{
        width: 300px ;
        height: 300px;
position: none;
display: block;
margin-top: 50px;
    }
.hero-img{
    max-width: 100%;
}

}
function hamburgerMenu(){
let menu = document.getElementById("menu");
if(menu.style.display === "block"){
    menu.style.display = "none";
}else{
    menu.style.display = "block";
}
}


