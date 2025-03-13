# Ex01 Portfolio
## Date:

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Roop Sagar S L - Portfolio</title>
  <link rel="stylesheet" href="style.css">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&family=Roboto:wght@400;700&display=swap"
    rel="stylesheet">
</head>
<body>
  <header class="header">
    <div class="container">
      <div class="profile-image">
        <img src="my.jpg" alt="Your Name">
      </div>
      <div class="header-content">
        <h1>Roop Sagar S L</h1>
        <p class="tagline">Creative Designer | Front-End Developer</p>
        <nav>
          <ul>
            <li><a href="">About</a></li>
            <li><a href="">Projects</a></li>
            <li><a href="">Contact</a></li>
          </ul>
        </nav>
      </div>
    </div>
  </header>
  <main>
    <section id="about" class="about">
      <div class="container">
        <h2>About Me</h2>
        <p>
          I am a passionate and creative individual with a strong background in design and front-end development. My goal is to craft innovative and user-friendly digital experiences. I am constantly learning and seeking new challenges to expand my skillset.
        </p>
        <p>
          I am proficient in HTML, CSS, JavaScript, and various design tools. I am also a team player and enjoy collaborating on projects.
        </p>
      </div>
    </section>
    <section id="projects" class="projects">
      <div class="container">
        <h2>Projects</h2>
        <div class="projects-grid">
          <div class="project-card">
            <img src="project1.jpg" alt="Project 1">
            <h3>Rental and Booking System Services</h3>
            <p>Django-based Car Rental and Booking System Services. The main project developed during the training was a Django-based Car Rental and Booking System Services application. The project aimed to create a web-based platform for users to book rental cars and for administrators to manage the listings and bookings.</p>
            <div class="project-details">
              <p>Technologies: HTML, CSS, Bootstrap</p>
              <a href="#" class="button">View Project</a>
            </div>
          </div>
          <div class="project-card">
            <img src="project2.jpg" alt="Project 2">
            <h3>Drestein '24</h3>
            <p>This project involved developing the front-end using React, HTML, JavaScript, and SCSS to create a seamless online registration process. Through this project, I gained valuable experience in front-end development, user interface design, and working with a Node.js backend."</p>
            <div class="project-details">
              <p>Technologies: React, Node.js, HTML, SCSS</p>
              <a href="#" class="button">View Project</a>
            </div>
          </div>
          </div>
      </div>   
    </section>
    <section id="contact" class="contact">
      <div class="container">
        <h2>Contact</h2>
        <p>Get in touch! Feel free to reach out to me.</p>
        <div class="contact-info">
          <p>Email : roopsagarofficial@gmailcom</p>
          <p>LinkedIn : <a href="https://www.linkedin.com/in/roop-sagar-s-l-602aa8290/">linkedin.com/in/roop-sagar-s-l-602aa8290</a></p>
          <p>GitHub: <a href="https://github.com/Roopsagar23001830">github.com/Roopsagar23001830</a></p>
        </div>
      </div>
    </section>
  </main>
</body>
</html>
```
style.css
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  font-family: 'Roboto', sans-serif;
  line-height: 1.6;
  background-color: #f8f8ff;
  color: #333;
}
.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}
a {
  text-decoration: none;
  color: #007bff;
}
a:hover {
  text-decoration: underline;
}
img {
  max-width: 100%;
  height: auto;
  display: block;
}
.header {
  background: linear-gradient(to right, #a8b8db, #d3cce3); 
  padding: 20px 0;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000; 
}
.header .container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.profile-image {
  margin-right: 20px;
}
.profile-image img {
  border-radius: 50%;
  width: 120px;
  height: 120px;
  object-fit: cover;
  border: 3px solid #fff;
}
.header-content h1 {
  font-size: 1.5em;
  font-family: 'Montserrat', sans-serif;
  margin-bottom: 5px;
}
.header-content .tagline {
  font-size: 0.9em;
  color: #555;
}
.header nav ul {
  list-style: none;
  display: flex;
}
.header nav ul li {
  margin-left: 20px;
}
.header nav ul li a {
  color: #333;
  font-weight: bold;
}
.header nav ul li a:hover {
  color: #007bff;
}
main {
  padding-top: 100px; 
}
section {
  padding: 80px 0;
}
section h2 {
  font-size: 2.5em;
  font-family: 'Montserrat', sans-serif;
  margin-bottom: 40px;
  text-align: center;
  color: #333;
}
.about {
  background-color: #fff;
}
.about .container {
  max-width: 800px;
  margin: 0 auto;
}
.about p {
  margin-bottom: 20px;
}
.projects {
  background: linear-gradient(to bottom, #d3cce3, #fff);
}
.projects .projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  grid-gap: 30px;
}
.project-card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s ease-in-out;
}
.project-card:hover {
  transform: translateY(-5px);
}
.project-card img {
  width: 100%;
  height: 200px;
  object-fit: cover;
}
.project-card h3 {
  font-size: 1.2em;
  font-family: 'Montserrat', sans-serif;
  padding: 15px;
}
.project-card p {
  padding: 0 15px;
  margin-bottom: 15px;
}
.project-details {
  padding: 15px;
  border-top: 1px solid #eee;
  display: flex;
  justify-content: space-between;
  align-items: center;
}
.project-details .button {
  background-color: #007bff;
  color: #fff;
  padding: 8px 15px;
  border-radius: 5px;
  text-decoration: none;
  display: inline-block;
}
.project-details .button:hover {
  background-color: #0056b3;
}
.contact {
  background: linear-gradient(to bottom, #fff, #d3cce3);
}
.contact .container {
  max-width: 600px;
  margin: 0 auto;
  text-align: center;
}
.contact p {
  margin-bottom: 20px;
}
.contact-info {
  margin-top: 30px;
}
.contact-info p {
  margin-bottom: 10px;
}
```

## OUTPUT
About Page
![about](https://github.com/user-attachments/assets/c3ce8ac9-a168-46c0-9cbe-0c0d2e471b0c)

Project Page
![project](https://github.com/user-attachments/assets/ce7ca79e-15bd-409a-ad26-1df30c4941d8)

Contact Page
![contact](https://github.com/user-attachments/assets/2168bc9e-7b6e-4e1f-ae38-e2465e37c4a8)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
