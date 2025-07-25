# initial-commit2
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Single-Page Website</title>
    <style>
        /* Basic CSS for the website styling */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box; /* Ensures padding and border are included in element's total width/height */
            scroll-behavior: smooth; /* Makes scrolling to sections smooth */
            background-color: #f4f4f4;
            color: #333;
        }

        /* Header Styling */
        header {
            background-color: #333;
            color: white;
            padding: 1rem 0;
            text-align: center;
        }

        header h1 {
            margin: 0;
            font-size: 2.5rem;
        }

        /* Navigation Bar Styling */
        nav {
            background-color: #444;
            padding: 0.5rem 0;
            text-align: center;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex; /* To display items side-by-side */
            justify-content: center; /* To center the items */
        }

        nav ul li {
            margin: 0 15px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            padding: 5px 10px;
            transition: background-color 0.3s ease;
        }

        nav ul li a:hover {
            background-color: #555;
            border-radius: 5px;
        }

        /* Main Sections Styling */
        section {
            padding: 60px 20px; /* Larger top/bottom padding */
            margin: 20px auto;
            max-width: 900px;
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            text-align: center; /* Center content within the section */
        }

        section:nth-of-type(even) { /* Different styling for even-numbered sections */
            background-color: #e9e9e9;
        }

        section h2 {
            color: #0056b3;
            font-size: 2rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }

        section h2::after { /* Underline effect for section titles */
            content: '';
            position: absolute;
            left: 50%;
            bottom: 0;
            transform: translateX(-50%);
            width: 80px;
            height: 3px;
            background-color: #007bff;
            border-radius: 5px;
        }

        /* Footer Styling */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 30px;
        }

        /* Specific styling for the Contact section form */
        #contact form {
            display: flex;
            flex-direction: column;
            gap: 15px;
            max-width: 500px;
            margin: 0 auto;
        }

        #contact label {
            text-align: left; /* Align labels to the left */
            margin-bottom: 5px;
            font-weight: bold;
        }

        #contact input[type="text"],
        #contact input[type="email"],
        #contact textarea {
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
            width: 100%; /* Ensures it takes 100% of available width in flex column */
            box-sizing: border-box; /* To maintain width with padding */
        }

        #contact textarea {
            resize: vertical; /* Allow vertical resizing only */
            min-height: 100px;
        }

        #contact button {
            background-color: #007bff;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 1.1rem;
            transition: background-color 0.3s ease;
        }

        #contact button:hover {
            background-color: #0056b3;
        }

        /* Additional styling for content within sections */
        .section-content {
            margin-top: 20px;
            line-height: 1.8;
            font-size: 1.1rem;
        }
    </style>
</head>
<body>

    <header>
        <h1>Our Amazing Website</h1>
        <p>Your perfect place to discover what we offer</p>
    </header>

    <nav>
        <ul>
            <li><a href="#about">About Us</a></li>
            <li><a href="#services">Our Services</a></li>
            <li><a href="#contact">Contact Us</a></li>
        </ul>
    </nav>

    <section id="about">
        <h2>About Us</h2>
        <div class="section-content">
            <p>Welcome to our website! We are a team of dedicated professionals committed to providing the best solutions and services to our clients. We always strive for innovation and excellence in everything we do, believing that quality is the key to success. Our mission is to build long-term relationships with our clients by delivering true value and continuous support.</p>
            <p>We have extensive experience in [mention your areas of expertise, e.g., web development, digital marketing, graphic design], and we work passionately to turn your ideas into tangible reality.</p>
        </div>
    </section>

    <section id="services">
        <h2>Our Services</h2>
        <div class="section-content">
            <p>We offer a wide range of services designed to meet your diverse needs. Here are some of our key services:</p>
            <ul>
                <li>**Web Development:** Designing and developing responsive and modern websites.</li>
                <li>**Digital Marketing:** Effective marketing strategies to boost your online presence.</li>
                <li>**Technical Consulting:** Providing advice and guidance for technical projects.</li>
                <li>**Graphic Design:** Creating attractive and innovative designs for your brand.</li>
            </ul>
            <p>We work with you every step of the way to ensure your goals are achieved in the best possible manner.</p>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <div class="section-content">
            <p>Do you have any questions or inquiries? Feel free to contact us. We are always happy to hear from you!</p>
            <form action="#" method="POST">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email Address:</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Your Message:</label>
                <textarea id="message" name="message" rows="5" required></textarea>

                <button type="submit">Send Message</button>
            </form>
            <p style="margin-top: 20px;">You can also reach us via: info@yourwebsite.com</p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Our Amazing Website. All rights reserved.</p>
    </footer>

</body>
</html>
