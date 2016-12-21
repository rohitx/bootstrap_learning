## Bootstrap 3 Essential Training

### Chapter 1: Getting Started

What is Bootstrap? 

* A framework
* Mobile First
* Responsive Design
* Has been tested 
* Uses modern web technologies such as HTML, CSS, and JS

What is a Framework? 

* A way to organize your code
* If you follow a certain structure
* A framework gives you many abilities
	* Pre-built CSS styles
	* JavaScript Functionality

When Should I use Bootstrap?

* Excellent for small, quick projects
* Prototyping and scaffolding sites
* Great for larger projects
	* Customize your installation if you work on larger projects
	* It is very modular

Bootstrap uses a CDN, which is content delivery network. This means that CDN hosts common libraries like bootstrap, and when someone visits a site that uses CDN link, their browser checks its cache or memory to see if the visitor has been to a similar site that is also using the same link. In that case, the browser will load the cached version of the library which allows the site to load fast. 

Bootstrap requires jQuery so you can either download it or use jQuery CDN.

The easiest way to install Bootstrap 3 is to use CDN. Let's create a template. We create an index.html page

```{html}
<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Bootstrap</title>
	<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">

</head>
<body>
<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>
</body>
</html>

```

We found the lines to add at the following [place](https://gist.github.com/planetoftheweb/884b9bff2f84d4134020). In here you will find all the necessary lines of code that will go in the `header` and in the `body` of the page. Let's go through some of them: 

* `<meta http-equiv="X-UA-Compatible" content="IE=edge">` tells the browser, especially Internet Explorer which version to use. The IE=edge says to use the latest and greatest version. 
* `<meta name="viewport" content="width=device-width, initial-scale=1">` tells the browser that if it is using a mobile device then it should render the browser page accordingly. The `initial-scale=1` means that it should use the scale at 100%. 
* `<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap.min.css">`. This link uses the CDN for bootstrap CSS. 
* If you do not want to use Bootstrap default flat version, you should use the following theme `<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/css/bootstrap-theme.min.css">`. 
* `<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>` Bootstrap requires jQuery so we should add this at the footer, right before the body closing tag. 
* `<script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.5/js/bootstrap.min.js"></script>` Bootstrap also uses JS so you should include this in the footer as well. 