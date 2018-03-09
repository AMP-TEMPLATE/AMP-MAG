Contents of the documentation

Steps | Title
------------ | -------------
1 | Preparing basic html structure
2 | Adding Scripts and Styles with <head></head> tags
3 | Adding basic styles 
4 | Design Section 1
5 | Design Section 2
6 | Design Section 3

![Image of Section1](https://github.com/iwilfried/AMP-MAG/blob/master/images/full_image.PNG)

### Step 1:Preparing basic html structure
```
<html>
<head>
<title> <!-- Give appropriate title to the page  --> </title>
<!-- Required scripts and styles -->
</head>
<body>
<!-- Page contents -->
</body>
</html>
```
### Step 2:Adding Scripts and Styles with ```<head></head>``` tags
```
<meta charset="utf-8">
<meta http-equiv="X-UA-Compatible" content="IE=Edge"/>
<meta name="viewport" content="width=device-width,minimum-scale=1,initial-scale=1">
<link rel="canonical" href="https://amp-mag.firebaseapp.com/">
<script custom-element="amp-font" src="https://cdn.ampproject.org/v0/amp-font-0.1.js" async></script>
<script custom-element="amp-sidebar" src="https://cdn.ampproject.org/v0/amp-sidebar-0.1.js" async></script>
<script custom-element="amp-accordion" src="https://cdn.ampproject.org/v0/amp-accordion-0.1.js" async></script>
<script src="https://cdn.ampproject.org/v0.js" async></script>

```

### Step 3:Adding basic styling to custom.css
```
html{
    -moz-osx-font-smoothing:grayscale;
    -webkit-font-smoothing:antialiased
}
body{
    font-family:Georgia, serif;
    font-size:100%;
    line-height:1.5;
    color:#121212;
    background:rgba(51,51,51,0.05)
}
.main-body{
    background:#ffffff;
    max-width:37.5rem;
    margin:0 auto;
    
    overflow-x:hidden;
}
html,body{
    text-rendering:optimizeSpeed
}
h1,h2,h3,h4,h5,h6{
    margin:0
}
p{
    font-size:1rem;
    font-weight:300;
    margin-top:0;
    margin-bottom:0.5rem;
    text-align: justify;
}
h3{
    font-size:1rem;
    line-height:1.5rem;
    font-weight:normal;
    margin-bottom:0.4375rem
}


a{
    color:#005689;
    cursor:pointer;
    text-decoration:none
}
a:hover,a:focus{
    text-decoration:underline
}
a:active{
    color:#4bc6df;
    text-decoration:none
}

menu,ol,ul{
    padding:0;
    margin-left:1.5625rem
}
nav ul,nav ol{
    list-style:none;
    list-style-image:none
}

```
# Step 4: Design Section 1
![Image of Section1](https://github.com/iwilfried/AMP-MAG/blob/master/images/section1.PNG)

### Code:
```
<header class="header">
<nav>
<div class="header_position">
<a class="header_linkstyle" href="">
<span class="header_drawcircle"></span>
<span class="header_circletext">
Support The <br>Ipsum</span>
</span>
</a>
</div>
<a href="" class="header_logo">
<span class="header_logo">
<svg viewbox="0 0 297 95" class="header_logo_svg">
<path fill="#121212" d="M66.8 50.7l5-2.6V8.4H68l-9.3 12.4h-1L58.2 7h40.5l.6 13.8h-1.1L89 8.4h-3.9V48l5 2.7V52H66.9v-1.3zm37-1.8V5L100 3.5v-.9L114.2.1h1.5v20.8l.3-.4a19 19 0 0 1 12.2-4.5c6.2 0 9 3.5 9 10v23l3.3 1.7V52H122v-1.3l3.4-1.8V26c0-3.6-1.6-5-4.6-5a7.8 7.8 0 0 0-4.9 1.6V49l3.3 1.8V52h-18.5v-1.2zm48.4-13.4c.4 7.2 3.6 12.8 11.4 12.8 3.7 0 6.3-1.7 8.8-3v1.5a17.4 17.4 0 0 1-13.6 6.2c-12 0-18-6.6-18-18.1 0-11.3 6.6-18.3 17.4-18.3 10.2 0 15.5 5 15.5 18.4v.4zm-.2-1.7l10.5-.7c0-9-1.5-15-4.6-15-3.3 0-5.9 7-5.9 15.6M0 69.6c0-19.1 12.7-26 26.8-26 6 0 11.6 1 14.8 2.3l.3 13.4h-1.4l-8.3-13a12.2 12.2 0 0 0-5.2-.8c-7.5 0-11.3 8.7-11.2 22.9.1 17 3 24.7 10 24.7a10.7 10.7 0 0 0 4.1-.7V74.2l-4.5-2.6V70h22v1.7l-4.5 2.5v18A49.2 49.2 0 0 1 26.2 95C10.2 95 0 87.5 0 69.6m47.1-9v-1L62 57l1.6.1v29c0 3.6 1.7 4.6 4.5 4.6a6 6 0 0 0 4.8-2.2v-26l-4-1.8v-1.2L83.6 57l1.4.2v33.3l4 1.6v1.1L74.4 95l-1.4-.1v-4.4h-.4A16.4 16.4 0 0 1 61.5 95C54.4 95 51 90.8 51 84.5v-22zm94.5-3.7l1.2.1v10.8h.4c1.6-7.9 5-10.8 9.3-10.8a4.7 4.7 0 0 1 1.8.3v11a12.6 12.6 0 0 0-3-.3 18.6 18.6 0 0 0-8 1.6v21.2l3.4 1.9V94h-19.3v-1.3l3.5-1.9v-29l-4-1.2v-1zm37.1.9V46.5l-4-1.5v-.9l15-2.7 1.3.2v48.8l4.2 1.5V93l-14.8 2-1.1-.1v-4h-.4a13.1 13.1 0 0 1-9.8 4.1c-8 0-13.9-6.1-13.9-18.7 0-13.2 6.9-19.7 17.2-19.7a14.7 14.7 0 0 1 6.3 1.2m0 31.2V60a5.5 5.5 0 0 0-4-1.3c-4 .1-6.5 6.2-6.5 16.9 0 9.6 1.8 15 7 14.8a5.2 5.2 0 0 0 3.5-1.3M211.5 57h1.3v34l3.4 1.8V94H197v-1.3l3.4-1.9V62.4l-4-1.7v-1.1zm1.4-9.2a6.4 6.4 0 0 1-6.6 6.3 6.3 6.3 0 1 1 0-12.6 6.5 6.5 0 0 1 6.6 6.3m46.3 43.1V62l-4-1.4v-1.4l14.7-2.8 1.5.2v4.3h.4a19.4 19.4 0 0 1 12.5-4.7c6.4 0 9.3 3 9.3 9.8v24.8l3.4 1.9V94h-19.2v-1.3l3.5-1.9v-24c0-3.8-1.6-5.3-4.7-5.3a8 8 0 0 0-5 1.7v27.6l3.3 1.9V94h-19.1v-1.3zm-21.3-18V68c0-7.3-1.5-9.6-6-9.6a11.8 11.8 0 0 0-1.6 0l-8 11h-1.1v-10a43.3 43.3 0 0 1 13.5-2.4c9.8 0 15.5 2.7 15.5 11v23.5l3.5 1v.9a15 15 0 0 1-7.2 1.6c-4.9 0-7.2-1.6-8.3-4.2h-.3c-2 2.8-5 4.3-9.6 4.3-5.8 0-9.8-3.6-9.8-9.9 0-6 3.8-9.4 11.5-10.8zm0 16.2V74.5l-2.4.2c-3.9.3-5.2 2.7-5.2 8.2 0 5.9 1.9 7.4 4.6 7.4a3.6 3.6 0 0 0 3-1.3M109.7 72.7V68c0-7.3-1.6-9.7-6.1-9.7a11.8 11.8 0 0 0-1.5.2L94 69.2h-1v-10a43.3 43.3 0 0 1 13.4-2.3c9.8 0 15.5 2.7 15.5 11v23.5l3.5 1v.9a15 15 0 0 1-7.2 1.6c-4.9 0-7.2-1.6-8.3-4.2h-.3c-2 2.8-5 4.3-9.5 4.3-5.9 0-9.8-3.6-9.8-9.9 0-6 3.7-9.4 11.4-10.8zm0 16.3V74.5l-2.5.2c-3.8.3-5.2 2.7-5.2 8.2 0 5.9 2 7.4 4.6 7.4a3.6 3.6 0 0 0 3-1.3"/>
</svg>
</span>
</a>
<ul class="ul_nav">
<li class="li_nav">
<a class="nav_link" href="homepage.html" >
Home
</a>
</li>
<li class="li_nav">
<a class="nav_link" href="about.html">
About Us
</a>
</li>
<li class="li_nav">
<a class="nav_link" href="faq.html">
FAQs
</a>
</li>
<li class="li_nav">
<a class="nav_link" href="help.html">
Help
</a>
</li>
<li class="li_nav">
<a class="nav_link" href="blog.html">
Blogs
</a>
</li>
</ul>
<button class="menu-burger" on='tap:sidebar1.toggle'>
<span class="menu-burger_icon"></span>
</button>
</nav>
</header>
<amp-sidebar class="menu" layout="nodisplay" id="sidebar1">
  <amp-img class="amp-close-image cross-btn"
 src="images/cross.png"
 width="20"
 height="20"
 alt="close sidebar"
 on="tap:sidebar1.close"
 role="button"
 tabindex="0"></amp-img>
<amp-accordion disable-session-states class="top_padding_20">
  <section>
    <h2 class="c1 side_menu_1">Home<hr class="side_menu_2"></h2>
    <div class="side_menu_5">
      <ul>
        <li class="side_menu_3"><a href="news.html" class="side_menu_sub_link">News</a></li>
        <li class="side_menu_3"><a href="sports.html" class="side_menu_sub_link">Sports</a></li>
        <li class="side_menu_3"><a href="entertainment.html" class="side_menu_sub_link">Entertainment</a></li>
      </ul>
    </div>
  </section>
  <section>
    <h2 class="c2 side_menu_1">About Us<hr class="side_menu_2"></h2>
    <div class="side_menu_5">
      <ul>
        <li class="side_menu_3"><a href="how_we_work.html" class="side_menu_sub_link">How we Work</a></li>
      </ul>
    </div>
  </section>
  <section>
    <h2 class="c3 side_menu_1">FAQs<hr class="side_menu_2"></h2>
    <div class="side_menu_5">
      <ul>
        <li class="side_menu_3"><a href="find_answers.html" class="side_menu_sub_link">Find Answers Here</a></li>
      </ul>
    </div>
  </section>
  <section>
    <h2 class="c4 side_menu_1">Help<hr class="side_menu_2"></h2>
    <div class="side_menu_5">
      <ul>
        <li class="side_menu_3"><a href="need_help.html" class="side_menu_sub_link">Need Help ?</a></li>
      </ul>
    </div>
  </section>
  <section>
    <h2 class="c5 side_menu_1">Blogs<hr class="side_menu_2"></h2>
    <div class="side_menu_5">
      <ul>
        <li class="side_menu_3"><a href="article1.html" class="side_menu_sub_link">Article 1</a></li>
        <li class="side_menu_3"><a href="article2.html" class="side_menu_sub_link">Article 2</a></li>
        <li class="side_menu_3"><a href="article3.html" class="side_menu_sub_link">Article 3</a></li>
      </ul>
    </div>
  </section>
</amp-accordion>

</amp-sidebar>
```
### Add classes to custom.css:
```
.header{
    background-color:#e9eff1;
    border-bottom:0.0625rem solid #abc2c9;
    color:#121212;
    position:relative;
    max-width:37.5rem;
    margin:0 auto
}
.header_position{
    left:-0.625rem;
    position:absolute;
    top:0
}
@media (min-width: 30em){
    .header_position{
        left:0
    }
}
.header_logo{
    display:-webkit-box;
    display:-webkit-flex;
    display:-ms-flexbox;
    display:flex;
    float:none;
    margin-left:auto
}
.header_logo_svg{
    display:block;
    height:3.25rem;
    width:9.9375rem;
    margin-bottom:0.9375rem;
    margin-right:2.8125rem;
    margin-top:0.1875rem
}
@media (min-width: 22.5em){
    .header_logo_svg{
        height:3.5625rem;
        margin-right:0.625rem;
        width:10.9375rem
    }
}
@media (min-width: 30em){
    .header_logo_svg{
        margin-right:1.25rem
    }
}
.header_linkstyle{
    color:#e9eff1
}
.header_circletext{
    -webkit-box-sizing:border-box;
    -moz-box-sizing:border-box;
    box-sizing:border-box;
    display:block;
    padding:0.5625rem 1.25rem 0.1875rem;
    position:relative;
    font-size:0.8125rem;
    line-height:1.2;
    text-align:center
}

.header_drawcircle{
    bottom:-0.75rem;
    left:0;
    overflow:hidden;
    position:absolute;
    right:0;
    top:0;
    -webkit-transition:-webkit-transform 250ms ease-out;
    transition:-webkit-transform 250ms ease-out;
    transition:transform 250ms ease-out;
    transition:transform 250ms ease-out, -webkit-transform 250ms ease-out;
    -webkit-transform-origin:top center;
    transform-origin:top center
}
.header_drawcircle:before{
    background:#121212;
    -webkit-border-radius:50%;
    border-radius:50%;
    bottom:0;
    content:'';
    display:block;
    left:0;
    padding-top:100%;
    position:absolute;
    right:0
}
.ul_nav{
    height:1.875rem;
    margin:0;
    padding:0 0.625rem
}
@media (min-width: 30em){
    .ul_nav{
        padding-left:1.25rem;

    }
}
.li_nav{
    display:block;
    float:left;
    font-weight:500;
}
.li_nav:first-child .nav_link{
    padding-left:0;
    
}
.li_nav:first-child .nav_link:before{
    content:none
}
.li_nav:nth-child(1){
    color:#c70000;
}
.li_nav:nth-child(2){
    color:#e05e00;
}
.li_nav:nth-child(3){
    color:#0084c6
}
.li_nav:nth-child(4){
    color:#a1845c
}
.li_nav:nth-child(5){
    color:#bb3b80
}
.nav_link{

    font-size:0.9375rem;
    font-weight:900;
    display:block;
    height:1.875rem;
    line-height:1;
    padding:0 0.25rem;
    position:relative;
    color:currentColor;
    cursor:pointer
}
@media (min-width: 22.5em){
    .nav_link{
       /* font-size:1rem*/
    }
}
.nav_link:before{
    content:'';
    display:block;
    left:0;
    bottom:0;
    position:absolute;
    border-left:0.0625rem solid #abc2c9;
    top:0.1875rem
}
.menu-burger{
    background-color:#121212;
    top:1.5rem;
    -webkit-box-shadow:0 0 0 0.0625rem rgba(0,0,0,0.08);
    box-shadow:0 0 0 0.0625rem rgba(0,0,0,0.08);
    color:#e9eff1;
    cursor:pointer;
    height:2.5rem;
    min-width:2.5rem;
    position:absolute;
    border:0;
    -webkit-border-radius:50%;
    border-radius:50%;
    outline:none;
    right:0.3125rem
}
@media (min-width: 22.5em){
    .menu-burger{
        bottom:-0.375rem;
        height:3rem;
        min-width:3rem;
        top:auto
    }
}
@media (min-width: 30em){
    .menu-burger{
        right:3.1875rem
    }
}
.menu-burger_icon{
    margin-top:-0.0625rem;
    right:0;
    margin-left:auto;
    margin-right:auto
}
.menu-burger_icon,.menu-burger_icon:before,.menu-burger_icon:after{
    background-color:currentColor;
    content:'';
    height:0.125rem;
    left:0;
    position:absolute;
    width:1.25rem
}
.menu-burger_icon:before{
    top:-0.375rem
}
.menu-burger_icon:after{
    bottom:-0.375rem
}
.menu{
    background-color:#e9eff1;
    color:#121212;
    width:80vw
}
.menu div:first-of-type{
    overflow-y:scroll
}


.cross-btn
{
    float:right;
}
 .top_padding_20 {
     margin-top: 20px;
}
 .menu_style {
     padding-left: 10px;
     margin-top:-30px;
}
}

 .link_style {
     border-right: 1px solid #999;
     padding-right: 3px;
     height: 30px;
}

 .side_menu {
     margin-top: 15px;
}

 .side_menu_1 {
     display: inline-block;
     padding-left:28px;
     padding-bottom: 5px;
     font-size: 18px;
     background:transparent;
     border:1px solid #EFEFEF;
}

 .side_menu_2 {
     margin-top: 5px;
     margin-left: 0px;
}

 .side_menu_3 {
     list-style: none;
     margin-bottom: 8px;
}
 .top_padding_20 {
     margin-top: 20px;
}
 .side_menu_4 {
     margin-left: 25px;
}

 .side_menu_5 {
     background-color:lightgray;
}

 .side_menu_sub_link{
     text-decoration: none;
     color:black;
     font-weight:100;
}

.side_menu_sub_link_1
{    margin-left: 5px;
     color:#c70000;
}
 .side_menu_sub_link_2 {
     margin-left: 5px;
     color:#e05c00;
}
 .side_menu_sub_link_3 {
     margin-left: 5px;
     color:#0084c6;
}
 .side_menu_sub_link_4 {
     margin-left: 5px;
     color:#a1845c;
}
 .side_menu_sub_link_5 {
     margin-left: 5px;
     color:#bb3b80;
}

.side_menu_sub_link_active
{
  margin-left:5px;
  color:black;
  font-weight: bold;
  text-decoration: none;
}
.c1, .c2, .c3, .c4, .c5 {
     text-decoration: none;
     font-weight: bold;
     font-size:1.5rem;
     color:#c70000;
     display: inline-block;
     
}
 .c2 {
     color:#e05c00;
}
 .c3 {
     color:#0084c6;
}
 .c4 {
     color:#a1845c;
}
 .c5 {
     color:#bb3b80;
}
<style amp-boilerplate>body{-webkit-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-moz-animation:-amp-start 8s steps(1,end) 0s 1 normal both;-ms-animation:-amp-start 8s steps(1,end) 0s 1 normal both;animation:-amp-start 8s steps(1,end) 0s 1 normal both}@-webkit-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-moz-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-ms-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@-o-keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}@keyframes -amp-start{from{visibility:hidden}to{visibility:visible}}</style><noscript><style amp-boilerplate>body{-webkit-animation:none;-moz-animation:none;-ms-animation:none;animation:none}</style></noscript>
```
# Step 5: Design Section 2

![Image of Section 2](https://github.com/iwilfried/AMP-MAG/blob/master/images/section%202.PNG)

### Code:
```
<div class="main-body">
<div class="side-margins">
<article id="article">
<header>
<div class="content__header">
<div class="container">


<div>
  <a href="news.html" class="side_menu_sub_link_1">News</a>
  <a href="sports.html" class="side_menu_sub_link_1">Sports</a>
  <a href="entertainment.html" class="side_menu_sub_link_1">Entertainment</a>
</div>

```
### Add classes to custom.css
```
.side-margins
{
    margin-left: 10px;
}
.content__header{
    background-image:-webkit-repeating-linear-gradient(top, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
    background-image:repeating-linear-gradient(to bottom, #dcdcdc, #dcdcdc 0.0625rem, transparent 0.0625rem, transparent 0.25rem);
    background-repeat:repeat-x;
    background-position:bottom;
    -webkit-background-size:0.0625rem 1.8125rem;
    background-size:0.0625rem 1.8125rem
}
.container
{
   padding-left:0.625rem;
   padding-right:0.625rem;
   -webkit-box-sizing:border-box;
   -moz-box-sizing:border-box;
   box-sizing:border-box
}
```
# Step 6: Design Section 3

![Image of Section 2](https://github.com/iwilfried/AMP-MAG/blob/master/images/section%203.PNG)

### Code:
```
<h1 class="content__headline">
FAQ Article
</h1>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.</p>
<amp-img src="images/scene2.jpg" layout="responsive" width="266" height="150"></amp-img>
<p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.Lorem ipsum dolor sit amet, consectetur adipiscing elit. Etiam egestas tortor sapien, non tristique ligula accumsan eu.</p>

</div>
</div>

</header>
</article>

</div>
</div>
```
### Add Classes to custom.css:
```
.content__headline{
    font-size:1.75rem;
    line-height:2rem;
    font-weight:400;
    letter-spacing:-.02rem;
    padding-top:0.375rem;
    padding-bottom:1.5rem
}
.content__headline a,.content__headline a:hover,.content__headline a:active,.content__headline a:focus{
    color:#333
}
.content__headline em{
    font-style:normal
}
.content__headline strong{
    font-weight:normal
}
.content__headline--byline{
    display:block;
    padding-top:0;
    margin-top:-1.5rem;
    padding-bottom:1.5rem
}
```
