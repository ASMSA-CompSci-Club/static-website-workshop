# CompSci Club - Building Static Websites Workshop #1

**Objective**: build a simple, static website using HTML and CSS with the constraints below.
- This intitial site will take advantage of [Github Pages](https://pages.github.com).
- The site must have at least three pages interlinked using `<a>` tags. Some page ideas are:
  - Bio/About
  - Schedule
  - Work/Portfolio
  - Contact
  - FAQ
  - 404
  
---

## Setting up Github Pages

Github Pages is a low-tech webhost that serves the HTML, CSS, and JS files in a repository straight to visitors. Github Pages is free and very convenient since changes to the site are automatically updated when the repository is updated. Every user, organization, and project gets one Github Pages site. You can have unlimited project sites. 

Simply create a repository named *username.github.io* and you are good to go!

You can optionally add a custom domain, but you will always be able to access your site via *username.github.io*.

## HTML Basics

HTML syntax is fairly straightforward. A page consists of many HTML elements, each with an opening tag (`<tag>`) and an end tag (`</tag>`). From there, you just need to be aware of the different types of HTML tags. [w3schools](https://www.w3schools.com/html/default.asp) is a great resource for this and some common tags are listed below. 

- `<p>` = paragraph
- `<h1>`,`<h2>`,`<h3>`,`<h4>`,`<h5>`,`<h6>` = headings
- `<a href="https://example.com">Link</a>` = link
- `<img src="example.png" />` = image
- `<div>` = section of the page
- `<span>` = inline section

A general outline of a simple HTML page is:
```
<!DOCTYPE html>
    <head>
        <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
        <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
        <meta http-equiv="X-UA-Compatible" content="ie=edge"/>
        <link rel="stylesheet" href="style.css"/>
        <title>Example Template</title>
    </head>
    <body>
    
        <nav>
          <a href="home.html">Home</a>
        </nav>
        
        <div class="body-card">
          <h1>An Example Site</h1>
          <p>Lorem Ipsum.</p>
        </div>
        
        <footer>
            <p>Copyright Example.</p>
        </footer>
        
    </body>
    
</html>

```
When making the homepage (example.com/) of a site, the file is named index.html. If you do not wish for pages to have .html at the end of its URL, you can abuse this fact by using multiple index.html files in different folder so index.html in the *cool* directory will be served as example.com/cool/.

HTML elements also have classes and IDs. While both of these are mostly used for CSS and JS functionality, it is important to know the difference. Classes are applied to multiple elements while IDs are unique identifiers. Therefore, any styling imposed on an ID trumps the styling enforced by a class. Additionally, you can create a link to a certain ID on the page by using `<a href="example.html#exampleID">Example ID</a>`. 
