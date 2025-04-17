<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Rapid Deal Group</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header>
    <nav>
      <h1>Rapid Deal Group</h1>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#deals">Deals</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <section class="hero">
    <h2>Fast Off-Market Real Estate Deals</h2>
    <p>Wholesale. Direct. Reliable. Welcome to Rapid Deal Group.</p>
  </section>

  <section id="about">
    <h2>About Us</h2>
    <p>We connect investors with profitable wholesale real estate deals. Whether you're buying or submitting, we move fast and keep it real.</p>
  </section>

  <section id="deals">
    <h2>Available Deals</h2>

    <div class="deal-card">
      <h3>123 Main St, Atlanta GA</h3>
      <p><strong>ARV:</strong> $250,000</p>
      <p><strong>Asking Price:</strong> $150,000</p>
      <p><strong>Repair Estimate:</strong> $25,000</p>
      <p><strong>Description:</strong> Great investment opportunity in an upcoming neighborhood.</p>
    </div>

  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <form action="submit_form.php" method="POST">
      <input type="text" name="name" placeholder="Your Name" required/>
      <input type="email" name="email" placeholder="Your Email" required/>
      <textarea name="message" placeholder="Your Message" required></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Rapid Deal Group. All rights reserved.</p>
  </footer>
</body>
</html>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background-color: #121212;
  color: #f1f1f1;
}

header {
  background-color: #1f1f1f;
  padding: 20px;
  text-align: center;
}

nav h1 {
  margin: 0;
  font-size: 28px;
}

nav ul {
  list-style: none;
  padding: 0;
  display: flex;
  justify-content: center;
  gap: 15px;
  margin-top: 10px;
}

nav ul li a {
  color: #fff;
  text-decoration: none;
}

.hero {
  text-align: center;
  padding: 60px 20px;
  background-color: #333;
}

section {
  padding: 40px 20px;
  text-align: center;
}

.deal-card {
  border: 1px solid #444;
  padding: 20px;
  margin: 20px auto;
  max-width: 500px;
  background-color: #1e1e1e;
  border-radius: 8px;
}

form {
  max-width: 600px;
  margin: 0 auto;
  display: flex;
  flex-direction: column;
  gap: 15px;
}

form input, form textarea {
  padding: 10px;
  border: none;
  border-radius: 5px;
}

form button {
  background-color: #4CAF50;
  color: white;
  padding: 12px;
  border: none;
  cursor: pointer;
  font-weight: bold;
}

form button:hover {
  background-color: #45a049;
}

footer {
  text-align: center;
  padding: 20px;
  background-color: #1f1f1f;
}
