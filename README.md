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
