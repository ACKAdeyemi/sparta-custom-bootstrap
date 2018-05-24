#<p align="center">Sparta Custom Bootstrap Project</p> 
<hr>
####Group Task (in pairs):
To create a 3 page website using Bootstrap about a topic of our own choice.

####It must have:
* Consistency and must look 'stylish'
* Wireframe and plan first, before coding
* At least 3 Pages
* Consistent Colour Scheme

####Top Tips:

* Can use coolors.co to create colour scheme
* Agree on each page before doing ANY coding
* Get the core of the site finished as a pair before working seperately
* Plan out a File structure, Git branch structure, and how you will be interacting with GitHub/your group member

Presenting Tomorrow Morning - **24th May 9:30am**
<hr>

#<p align="center">Our Website - Easy Cook Meals</p>

**Description** - This website presents easy cook meal solutions for people with a busy schedule/those without the time to cook a standard meal.

**GitHub URL:** 
[https://github.com/ACKAdeyemi/sparta-custom-bootstrap](https://github.com/ACKAdeyemi/sparta-custom-bootstrap)

**How to Download** - click 'clone or download' button, download a zip of our project, unzip and enjoy.

####Challenges:
* We got lucky that we were able to communicate face-2-face, comms remotely would have made confirmations and discussions more difficult, adding to time taken to complete the project.
* We worked really well together as we discussed our ideas equally, listened to each other well, we planned effectively at beginning and we paid attention to the project scope and time
* We could have tried to add more features to make things a bit more exciting – mainly the features that we discussed earlier
* Textarea for 'Message' box on Contact page doesn't allow the user to resize even though the CSS states **“resize: both;”**  - we also tried input[type=textarea]{resize:vertical} and it still didn't work

Code Snippet of our Message Box on our contact page:

```html
<!-- HTML CODE-->
<div class="form-inputs col-lg-9 col-md-9 col-sm-9 col-xs-9">
	<input class="message-textbox" type="textarea" placeholder="Hi there...">
</div>
```

```css
/* CSS CODE */
.message-textbox {
  resize:both;
}
```
<hr>

#<p align="center">How we built our index/Home page:</p>
###index/Home page screenshot
![Screenshot of index/Home Page](images/screenshot-of-index-page.png)

###index.html Code Snippet (linked to style/global.css)
```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="Easy Cook Meals Website for people">
    <meta name="author" content="Isabel and Chris">
    <title>Easy Cook Meals</title>

    <!-- ICON FOR THE TAB WINDOW -->
    <link rel="icon" type="image/png"  href="../images/site-favicon.png">

    <!-- BOOTSTRAP and JQUERY -->
    <link rel="stylesheet" href="css/bootstrap-3.3.7-dist/css/bootstrap.css">
    <script src="js/jquery-3.3.1.min.js" charset="utf-8"></script>
    <script src="css/bootstrap-3.3.7-dist/js/bootstrap.js" charset="utf-8"></script>

    <!-- OTHER CSS - ALWAYS BELOW BOOTSTRAP-->
    <link rel="stylesheet" type="text/css" href="css/global.css">
    <link rel="stylesheet" type="text/css" href="css/style.css">
  </head>

  <body>
    <nav class="navbar navbar-inverse navbar-fixed-top">
      <div class="container">
        <div class="navbar-header">
          <button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#navbar" aria-expanded="false" aria-controls="navbar">
            <span class="sr-only">Toggle navigation</span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </button>
          <a class="navbar-brand" href="index.html">Easy Cook Meals</a>
        </div>
        <div id="navbar" class="collapse navbar-collapse">
          <ul class="nav navbar-nav">
            <li class="active"><a href="#">Home</a></li>
            <li><a href="pages/about.html">About</a></li>
            <li><a href="pages/contact.html">Contact</a></li>
          </ul>
        </div><!--/.nav-collapse -->
      </div>
    </nav>

    <!-- Main jumbotron for a primary marketing message or call to action -->
    <div class="jumbotron">
      <div class="custom-filter">
        <div class="container">
          <h1>Hello, world!</h1>
          <p>This is a template for a simple marketing or informational website. It includes a large callout called a jumbotron and three supporting pieces of content. Use it as a starting point to create something more unique.</p>
        </div>
      </div>
    </div>

    <div class="container">
      <!-- Example row of columns -->
      <div class="row">
        <div class="col-md-4">
          <img class="showcase-food" src="https://source.unsplash.com/1600x900/?culinary" alt="">
          <h3>Heading</h3>
          <p>Donec id elit non mi porta gravida at eget metus.</p>
        </div>
        <div class="col-md-4">
          <img class="showcase-food" src="https://source.unsplash.com/1600x900/?food" alt="">
          <h3>Heading</h3>
          <p>Donec id elit non mi porta gravida at eget metus.</p>
       </div>
        <div class="col-md-4">
          <img class="showcase-food" src="https://source.unsplash.com/1600x900/?cook" alt="">
          <h3>Heading</h3>
          <p>Donec id elit non mi porta gravida at eget metus.</p>
        </div>
      </div>

      <hr>

      <footer>
        <div class="pull-left">
        <p>&copy; 2018 Easy Cook Meals Ltd.</p>
      </div>
      <div class="pull-right">
        <img src="images/facebook-square.svg" alt="">
        <img src="images/instagram.svg" alt="">
        <img src="images/twitter-square.svg" alt="">
      </div>
      </footer>
    </div> <!-- /container -->
  </body>
</html>
```
###style.css Code Snippet (only applies to index.html)
```css
.jumbotron{
  background-image: url("../images/jumbotron-backg.jpg");
  width: 100%;
  background-repeat: no-repeat;
  background-size:cover;
  padding: 0;
}
.jumbotron .custom-filter {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 30px 0 50px 0;
}
.jumbotron {
  color: white;
  text-shadow: 2px 2px rgb(52, 51, 51);
}
.showcase-food {
  width: 100%;
}
.container {
  text-align: center;
}
```

###global.css Code Snippet (applies to all .html docs)
```css
body {
  padding-top: 50px;
}
.starter-template {
  padding: 40px 15px;
  text-align: center;
}
.pull-right img {
  width: 25px;
  margin-left: 20px;
}
```