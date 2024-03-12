---
title: "Weave a Web of Memories: Creating a Photo Collage with HTML & CSS"
datePublished: Tue Mar 12 2024 07:08:58 GMT+0000 (Coordinated Universal Time)
cuid: clto177qw000m09ju780lbju8
slug: weave-a-web-of-memories-creating-a-photo-collage-with-html-css
canonical: https://blog.techlearnindia.com/weave-a-web-of-memories-creating-a-photo-collage-with-html-css
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1710220317992/610d3d6b-be9e-4257-b1c2-70c3a09f1c34.png
tags: css3, css, javascript, html5

---

### **Introduction**

Cherished memories with loved ones deserve a special place. In the digital age, photos capture these moments beautifully. But what if you could transform them into a stunning visual tapestry? With HTML and CSS, you can create a personalized photo collage to celebrate your family and friends.

This blog post will guide you through the steps of building a webpage showcasing your precious memories as a collage. No prior coding experience is necessary, and the process is surprisingly easy!

### **What you'll need**

* **Text Editor:** Any basic text editor like Notepad or Sublime Text will work.
    
* **Images:** Select photos representing your favorite memories with friends and family. Ensure they are saved in a folder on your computer.
    
* **Patience and Creativity!**
    

### **Getting Started: Building the Foundation with HTML**

1. **Create an HTML File:** Open your text editor and create a new file. Save it as "collage.html".
    
2. **Basic Structure:** Type the following code into your file. This creates the fundamental structure of your webpage:
    
3. **Create CSS file** : Create css in notepad and name it as style.css in same folder
    
4. **JavaScript Entry**: Enter the JavaScript code for adding functionality and event listener from below code and name your file as "myscripts.js".
    
5. **Remember** by creating this file add this file link path in your html file for css &lt;link rel="stylesheet" href="style.css"&gt; and for JavaScript &lt;script src="myscripts.js"&gt;&lt;/script&gt;
    

```xml
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Memories Collaget</title>
<!-- CSS   File                   -->
    <link rel="stylesheet" href="style.css">
<!-- JavaScript File                 -->
<script src="myscripts.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/sweetalert2@9"></script>
</head>
<body>
    <h1>My Memories Collage</h1>
    <div class="images">
    <img src="https://www.dropbox.com/s/e8d0qsnukvp97p6/whatsapp%20image%202022-05-28%20at%206.45.40%20pm.jpeg?dl=1" alt="1.png">
    
    <img src="https://www.dropbox.com/s/txxxhomvuadi03p/whatsapp%20image%202022-05-28%20at%204.54.21%20pm.jpeg?dl=1" alt="2.png">
    
    <img src="https://www.dropbox.com/s/ft7l79kqkor0xry/whatsapp%20image%202022-05-28%20at%206.45.38%20pm.jpeg?dl=1" alt="3.png">
    
    <img src="https://www.dropbox.com/s/3sds541a7zq16n3/whatsapp%20image%202022-05-28%20at%206.45.40%20pm%20%281%29.jpeg?dl=1" alt="4.png">
   
    <img src="https://www.dropbox.com/s/a6qs8q79fq2y7y8/img_20220528_164151.jpg?dl=1" alt="5.png">
    
    <img src="https://www.dropbox.com/s/1cr1xdz8na8nid5/whatsapp%20image%202022-05-28%20at%204.24.41%20pm%20%281%29.jpeg?dl=1" alt="6.png">
   
    <img src="https://www.dropbox.com/s/gawf6or0ds1hpxg/whatsapp%20image%202022-05-28%20at%204.24.41%20pm.jpeg?dl=1" alt="7.png">
    
    <img src="https://www.dropbox.com/s/swvu3ieq9i9nevg/whatsapp%20image%202022-05-28%20at%204.26.13%20pm.jpeg?dl=1" alt="8.png">
    
    <img src="https://www.dropbox.com/s/tr8leqnb299sxg1/whatsapp%20image%202022-05-28%20at%204.27.20%20pm.jpeg?dl=1" alt="9.png">
    <audio controls style=" display:none;" loop   id="a"  >
    <source  src=" https://www.dropbox.com/s/8yybzaos18wt531/bhool%20bhulaiyaa%202.mp3?dl=1">
    </audio>
   
    </div>
    
</body>
<script>
    Swal.fire('☺️')
        </script>
</html>
```

1. `<!DOCTYPE html>`: Declares the document type and version of HTML.
    
2. `<html lang="en">`: The root element of the HTML document, indicating that the document is in English.
    
3. `<head>`: Contains meta-information about the HTML document, such as character encoding, viewport settings, title, and links to external resources.
    
    * `<meta charset="UTF-8">`: Defines the character encoding of the document as UTF-8.
        
    * `<meta http-equiv="X-UA-Compatible" content="IE=edge">`: Instructs Internet Explorer to use the latest rendering engine available.
        
    * `<meta name="viewport" content="width=device-width, initial-scale=1.0">`: Sets the viewport width to the device width and initial zoom level to 1.0.
        
    * `<title>My Memories Collage</title>`: Sets the title of the HTML document.
        
    * `<link rel="stylesheet" href="style.css">`: Links the HTML file to an external CSS file named "style.css".
        
    * `<script src="`[`https://cdn.jsdelivr.net/npm/sweetalert2@9"></script>`](https://cdn.jsdelivr.net/npm/sweetalert2@9%22%3E%3C/script%3E): Loads the SweetAlert2 library from a CDN.
        
4. `<body>`: Contains the visible content of the HTML document.
    
    * `<h1>My Memories Collage</h1>`: Displays a heading "My Memories Collage".
        
    * `<div class="images">`: A container for images in the collage.
        
        * Several `<img>` tags: Each represents an image in the collage, sourced from different URLs and with corresponding alternative text.
            
    * `<audio controls style=" display:none;" loop id="a">`: Defines an audio element with controls hidden, set to loop, and with an ID "a".
        
        * `<source src="URL">`: Specifies the audio source URL.
            
5. `<script>`: Contains JavaScript code.
    
    * [`Swal.fire`](http://Swal.fire)`('☺️')`: Invokes SweetAlert2 to display a smiley face when the page loads.
        

```css
@import url('https://fonts.googleapis.com/css2?family=Carter+One&display=swap');

*{
    box-sizing: border-box;
    margin: 0;
    padding: 0;
   
}

body{
    text-align: center;
    background-color:#000;
    color: white;
    text-transform: uppercase;
    font-family: 'Carter One', cursive;

background-image: radial-gradient( circle 610px at 5.2% 51.6%,  rgba(5,8,114,1) 0%, rgba(7,3,53,1) 97.5% ); 
}

.images{
    display: grid;
    padding: 25px;
    align-items: center;
    justify-content: center;
    overflow:hidden ;
    grid-template-columns: repeat(3,129px);
    grid-template-rows: repeat(3,129px);
    grid-auto-flow: column dense;
}


img{
    height: 100%;
    width: 100%;
    object-fit: cover;
    transition:0.3s;
    -webkit-mask:
    linear-gradient(red 0 0) center/calc(100% - 1.85*30px) calc(100% - 1.85*30px) no-repeat,
    radial-gradient(farthest-side,red 98%,#0000) 0 0/60px 60px round;
          mask:
    linear-gradient(red 0 0) center/calc(100% - 1.85*30px) calc(100% - 1.85*30px) no-repeat,
    radial-gradient(farthest-side,red 98%,#0000) 0 0/60px 60px round;
}

img:hover{
    height: 200px;
    width: 200px;
    transform:rotateZ(300deg);
    z-index: 1;
}

footer{
  position: fixed;
  width: 100%;
  bottom: 0;
  left: 0;
  background:black;
  padding:20px;
  text-align: center;
  font-family:monospace;
}
.footer a{
  padding:5px 5px;
  text-decoration:none;
  font-size: 25px;
  font-weight:bold;
  color:  #fff;
  animation:anim 3.2s linear infinite ;
}
@keyframes anim{
    0%{
        border-top:3px solid #fff;
    }
    25%{
        border-left:3px solid #fff;
    }
    50%{
        border-bottom:3px solid #fff;
    }
    75%{
        border-right:3px solid #fff;
    }
}
```

1. `@import url('`[`https://fonts.googleapis.com/css2?family=Carter+One&display=swap`](https://fonts.googleapis.com/css2?family=Carter+One&display=swap)`');`: Imports a Google Font named "Carter One" to be used in the document.
    
2. `*`: Selects all elements in the document.
    
    * `box-sizing`, `margin`, `padding`: Sets box-sizing to border-box and resets margin and padding for all elements.
        
3. `body`: Styles applied to the `<body>` element.
    
    * `text-align`, `background-color`, `color`: Aligns text to the center, sets background color to black, and text color to white.
        
    * `text-transform`: Transforms text to uppercase.
        
    * `font-family`: Specifies the font family.
        
    * `background-image`: Sets a radial gradient background.
        
4. `.images`: Styles applied to the container of images.
    
    * `display`: Sets the display property to grid.
        
    * `padding`: Adds padding around the container.
        
    * `align-items`, `justify-content`: Centers items inside the container.
        
    * `overflow`: Specifies how to handle content overflow.
        
    * `grid-template-columns`, `grid-template-rows`: Defines the grid layout.
        
5. `img`: Styles applied to the `<img>` elements.
    
    * `height`, `width`, `object-fit`: Sets dimensions and object-fit property.
        
    * `transition`: Specifies transition effects.
        
    * `-webkit-mask`, `mask`: Creates a circular mask for images.
        
6. `img:hover`: Styles applied when hovering over an `<img>` element.
    
    * Increases the size of the image and applies a rotation effect.
        
7. `footer`, `.footer a`, `@keyframes anim`: Styles applied to the footer section and its links, including an animation for the links.
    

```javascript
window.addEventListener("mouseover",play);
window.addEventListener("click",play);
function play() { document.getElementById("a").play();
}
```

1. `window.addEventListener("mouseover", play);`: Listens for mouseover events and calls the `play` function.
    
2. `window.addEventListener("click", play);`: Listens for click events and calls the `play` function.
    
3. `function play() { document.getElementById("a").play(); }`: Defines the `play` function, which plays the audio referenced by the ID "a". This function is triggered by mouseover and click events on the window.
    

* This JavaScript code adds interactivity to the webpage.
    
* It listens for mouseover and click events on the window.
    
* When either of these events occurs, it calls the `play` function.
    
* The `play` function plays the audio referenced by the ID "a" when called.
    

### **Summary:**

* **HTML** provides the structure and content of the webpage.
    
* **CSS** styles the elements to make the webpage visually appealing.
    
* **JavaScript** adds functionality to the webpage, making it interactive.
    
* Together, these languages work to create a webpage that displays a collage of images, plays audio, and responds to user actions like clicking and hovering.
    

### **TechLearn India's Approach**

This course is designed for learners of all levels, with a focus on practical application. You won't be bombarded with complex jargon; instead, you'll learn by doing. Here's what sets TechLearn India apart:

* **Project-Based Learning:** The entire course revolves around building your memory collage. Each lesson is designed to equip you with the skills needed for the next step in your project.
    
* **Interactive Learning:** Get ready for engaging video tutorials, quizzes, and hands-on exercises that solidify your understanding.
    

### **Beyond the Collage**

The skills you acquire in this course extend far beyond memory collages. With your newfound knowledge of CSS & JavaScript, you'll be able to:

* **Design stunning websites:** Whether it's a personal portfolio or a blog, you'll have the tools to create visually appealing and interactive web experiences.
    
* **Enhance existing websites:** Can you imagine adding cool animations or hover effects to your favorite websites? With your CSS skills, you can customize your web experience!
    
* **Open doors to future learning:** CSS & JavaScript are fundamental building blocks for web development. This course acts as a springboard to explore more advanced web technologies.
    

**So, are you ready to turn your digital memories into a vibrant collage and unlock a world of creative possibilities? Enroll in 👉👉👉** [TechLearn India's CSS](https://app.techlearnindia.com/css/?coupon=LEARNING28) **course today! Remember, learning to code isn't just about technical skills; it's about empowering yourself to express your creativity and build something truly special.**