<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rapid Deal Group - Wholesale Real Estate</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">
                <h1>Rapid Deal Group</h1>
            </div>
            <ul>
                <li><a href="#about">About</a></li>
                <li><a href="#deals">Deals</a></li>
                <li><a href="#contact">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="hero-content">
            <h2>Exclusive Off-Market Deals Fast</h2>
            <p>Get exclusive access to wholesale real estate opportunities.</p>
        </div>
    </section>

    <section id="about">
        <div class="container">
            <h2>About Us</h2>
            <p>We specialize in fast, off-market wholesale real estate deals that connect investors with profitable opportunities.</p>
        </div>
    </section>

    <section id="deals">
        <div class="container">
            <h2>Current Deals</h2>
            <p>Browse our available deals. You can also submit your own property for review.</p>
        </div>
    </section>

    <section id="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <form action="submit_form.php" method="POST">
                <label for="name">Name:</label>
                <input type="text" id="name" name="name" required>
                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>
                <textarea id="message" name="message" placeholder="Your message..." required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <p>© 2025 Rapid Deal Group | All rights reserved.</p>
    </footer>
</body>
</html>

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #1a1a1a;
    color: white;
}

header {
    background-color: #333;
    padding: 20px 0;
    text-align: center;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 20px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

.hero {
    background: url('hero-bg.jpg') no-repeat center center/cover;
    height: 60vh;
    color: white;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}

.hero h2 {
    font-size: 3em;
    margin: 0;
}

.hero p {
    font-size: 1.2em;
}

section {
    padding: 40px 0;
}

.container {
    width: 80%;
    margin: 0 auto;
    text-align: center;
}

footer {
    background-color: #333;
    padding: 20px 0;
    text-align: center;
}

footer p {
    margin: 0;
}

form {
    display: flex;
    flex-direction: column;
    align-items: center;
}

form input, form textarea {
    margin: 10px 0;
    padding: 10px;
    width: 80%;
    max-width: 600px;
}

form button {
    padding: 10px 20px;
    background-color: #4CAF50;
    color: white;
    border: none;
    cursor: pointer;
}

form button:hover {
    background-color: #45a049;
}

<?php
if ($_SERVER["REQUEST_METHOD"] == "POST") {
    $name = $_POST['name'];
    $email = $_POST['email'];
    $message = $_POST['message'];

    // Save or send the form data (e.g., store in Google Sheets)
    // For now, this is a simple email handler
    $to = "youremail@example.com";
    $subject = "New Contact Form Submission";
    $body = "Name: $name\nEmail: $email\nMessage: $message";
    mail($to, $subject, $body);
    echo "Thank you for your message!";
}
?>
