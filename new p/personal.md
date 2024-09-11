### Personal Portfolio Website

Below is a basic structure of a personal portfolio website that includes all the requested elements. We'll structure the website using proper semantic HTML, include an image gallery, a contact form, and ensure the website is responsive.

---

#### **Project Structure**

1. **Home (index.html)**: Introduction, navigation bar, and links to other pages.
2. **Contact (contact.html)**: Contact form with proper validation.
3. **Gallery (gallery.html)**: Image gallery with multimedia elements.

---

### **index.html** – Homepage

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Personal Portfolio of [Your Name]">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>[Your Name] - Portfolio</title>
    <style>
        /* Basic styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            text-align: center;
        }

        nav ul li {
            display: inline-block;
            margin-right: 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
        }

        section {
            padding: 20px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        /* Responsive design */
        @media (max-width: 768px) {
            nav ul li {
                display: block;
                margin-right: 0;
                padding: 10px 0;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Portfolio</h1>
    </header>

    <nav>
        <ul>
            <li><a href="index.html">Home</a></li>
            <li><a href="gallery.html">Gallery</a></li>
            <li><a href="contact.html">Contact</a></li>
        </ul>
    </nav>

    <section>
        <h2>Introduction</h2>
        <p>Hello, I'm [Your Name], a [Your Profession]. Welcome to my personal portfolio where you can explore my work, projects, and get in touch with me.</p>

        <h3>Explore More</h3>
        <ul>
            <li><a href="gallery.html">View my gallery</a></li>
            <li><a href="contact.html">Contact me</a></li>
        </ul>
    </section>

    <footer>
        <p>&copy; 2024 [Your Name] | All Rights Reserved</p>
    </footer>
</body>
</html>
```

---

### **contact.html** – Contact Form

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Contact [Your Name]">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Me</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }

        section {
            padding: 20px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        form {
            max-width: 600px;
            margin: 0 auto;
            background: #f4f4f4;
            padding: 20px;
            border-radius: 8px;
        }

        form input, form textarea, form button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
        }
    </style>
</head>
<body>
    <header>
        <h1>Contact Me</h1>
    </header>

    <section>
        <h2>Get in Touch</h2>
        <form action="submit_form.php" method="POST">
            <label for="name">Your Name:</label>
            <input type="text" id="name" name="name" required>

            <label for="email">Your Email:</label>
            <input type="email" id="email" name="email" required>

            <label for="message">Your Message:</label>
            <textarea id="message" name="message" rows="4" required></textarea>

            <label for="file">Upload your resume (optional):</label>
            <input type="file" id="file" name="file">

            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 [Your Name] | All Rights Reserved</p>
    </footer>
</body>
</html>
```

---

### **gallery.html** – Image Gallery and Multimedia

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="description" content="Gallery of [Your Name]">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gallery</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        header {
            background-color: #333;
            color: white;
            padding: 10px 0;
            text-align: center;
        }

        section {
            padding: 20px;
        }

        .gallery img {
            width: 30%;
            margin: 10px;
            border-radius: 8px;
        }

        .media {
            margin-top: 20px;
        }

        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>
    <header>
        <h1>My Gallery</h1>
    </header>

    <section>
        <h2>Image Gallery</h2>
        <div class="gallery">
            <img src="image1.jpg" alt="Project 1 description">
            <img src="image2.jpg" alt="Project 2 description">
            <img src="image3.jpg" alt="Project 3 description">
        </div>

        <div class="media">
            <h2>Watch My Introduction Video</h2>
            <video controls width="500">
                <source src="intro.mp4" type="video/mp4">
                Your browser does not support the video tag.
            </video>

            <h2>Listen to My Podcast</h2>
            <audio controls>
                <source src="podcast.mp3" type="audio/mpeg">
                Your browser does not support the audio tag.
            </audio>
        </div>
    </section>

    <footer>
        <p>&copy; 2024 [Your Name] | All Rights Reserved</p>
    </footer>
</body>
</html>
```

---

### **Responsive Design & Semantic HTML**

Each page includes the **meta viewport** tag to ensure responsive design:
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

In addition:
- The layout adapts to smaller screens using **media queries**.
- Images and media elements scale appropriately, and the navigation bar changes structure for mobile screens.

### Final Thoughts

This structure offers a simple, professional, and responsive personal portfolio website that includes multimedia, forms, and optimized elements for accessibility and SEO. You can expand it further by adding more sections like **projects**, **blog**, or **testimonials** to showcase your work or experience.
