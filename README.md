# Ex02 Commercial Website
## Date:15-10-2025

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
## HTML
``
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Solutions Hub</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#contact">Contact</a></li>
                <li><a href="#account">Account</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="section">
        <div class="home-content">
            <h1>Welcome to AI Solutions Hub</h1>
            <p>Your one-stop solution for cutting-edge AI and machine learning services.</p>
            <button class="cta-button" >Explore Our Services</button>
            <div class="featured-services">
                <h2>Our Services</h2>
                <ul>
                    <li>AI Chatbot Development</li>
                    <li>Machine Learning Models</li>
                    <li>Data Analytics Solutions</li>
                </ul>
            </div>
            <div class="benefits">
                <h3>Why Choose Us?</h3>
                <p>Innovative Solutions | Expert Team | Scalable Infrastructure</p>
            </div>
        </div>
    </section>

    <section id="services" class="section">
        <div class="services-content">
            <h2>Our Services</h2>
            <p>We offer a wide range of AI and machine learning solutions to help your business grow:</p>
            <ul>
                <li><strong>AI Chatbot Development:</strong> Enhance customer engagement with intelligent conversational agents.</li>
                <li><strong>Machine Learning Models:</strong> Advanced predictive analytics and data-driven insights.</li>
                <li><strong>Data Analytics Solutions:</strong> Extract valuable insights from big data for better decision-making.</li>
                <li><strong>Natural Language Processing:</strong> Improve text analysis and language understanding.</li>
                <li><strong>Computer Vision:</strong> Automate visual data analysis with deep learning.</li>
            </ul>
        </div>
    </section>

    <section id="about" class="section">
        <div class="about-content">
            <h2>About Us</h2>
            <p>At AI Solutions Hub, we are dedicated to revolutionizing businesses with cutting-edge AI technologies and machine learning solutions. Our team of experts specializes in developing advanced AI chatbots, predictive models, and data analytics tools to help organizations achieve better efficiency and smarter decision-making. With a passion for innovation and a commitment to excellence, we aim to deliver scalable and customized AI solutions tailored to meet your business needs.</p>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="contact-content">
            <h2>Contact Us</h2>
            <p>Email:rishi@gmail.com</p>
            <p>Phone: +123 456 7890</p>
            <p>Address: 123 AI Street, Tech City, TX 45678</p>
            <form>
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <section id="account" class="section">
        <div class="account-content">
            <h2>User Account</h2>
            <p>Login to access exclusive content and manage your profile.</p>
            <form>
                <input type="email" placeholder="Email" required>
                <input type="password" placeholder="Password" required>
                <button type="submit">Login</button>
                <p><a href="#">Forgot Password?</a></p>
                <p><a href="#">Create an Account</a></p>
            </form>
        </div>
    </section>

    <footer>
        <div class="social-media">
            <a href="#">LinkedIn</a>
            <a href="#">GitHub</a>
            <a href="#">Instagram</a>
        </div>
        <p>Name: RISHI CHANDRAN R</p>
        <p>Registration No: 212223043005</p>
        <p>&copy; 2025 AI Solutions Hub. All rights reserved.</p>
    </footer>
</body>
</html>
```
## CSS
```
/* General Page Styling */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    line-height: 1.6;
    background-color: #65dde6;
    color: #333;
}

/* Header and Navigation */
header {
    background: #222;
    padding: 20px 0;
}

nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
}

nav ul li {
    margin: 0 20px;
}

nav ul li a {
    color: #f3f770;
    text-decoration: none;
    font-size: 16px;
}

nav ul li a:hover {
    text-decoration: underline;
}

/* Section Styling */
.section {
    padding: 50px 20px;
    max-width: 1000px;
    margin: auto;
    text-align: center;
}

.section h1 {
    font-size: 36px;
    margin-bottom: 15px;
}

.section h2 {
    font-size: 28px;
    margin-bottom: 10px;
}

.section h3 {
    font-size: 22px;
    margin-bottom: 8px;
}

.section p {
    font-size: 16px;
    margin-bottom: 15px;
}

/* Lists */
ul {
    padding: 0;
    list-style: none;
}

ul li {
    font-size: 16px;
    padding: 5px 0;
}

/* Buttons */
.cta-button, button {
    padding: 10px 20px;
    font-size: 16px;
    background: #0073e6;
    color: #fff;
    border: none;
    cursor: pointer;
    border-radius: 4px;
}

.cta-button:hover, button:hover {
    background: #005bb5;
}

/* Forms */
form {
    display: flex;
    flex-direction: column;
    gap: 10px;
    max-width: 400px;
    margin: 20px auto;
}

form input, form textarea {
    padding: 10px;
    font-size: 16px;
    border: 1px solid #ccc;
    border-radius: 4px;
}

form textarea {
    resize: vertical;
}

/* Footer */
footer {
    background: #222;
    color: #fff;
    padding: 20px;
    text-align: center;
}

footer .social-media a {
    color: #fff;
    margin: 0 10px;
    text-decoration: none;
}

footer .social-media a:hover {
    text-decoration: underline;
}
```

## OUTPUT

![WhatsApp Image 2025-11-05 at 08 53 49_8c8ede70](https://github.com/user-attachments/assets/e4fc4de8-1daf-44b2-834e-b11fc81f373b)

![WhatsApp Image 2025-11-05 at 08 53 48_8590644f](https://github.com/user-attachments/assets/ff38e28e-46ff-4dc6-b5e3-2875960492ae)



## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
