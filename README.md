Sure! Here’s the complete updated code for your Kaimana Car Rental & Travel website, including the WhatsApp contact, booking form, and improved design.


---

1. index.html (Main Page)

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kaimana Car Rental & Travel</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header class="hero">
        <div class="container">
            <h1>Welcome to Kaimana Car Rental & Travel</h1>
            <p>Explore Kaimana with the best car rental and tour services.</p>
            <a href="#booking" class="btn">Book Now</a>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#gallery">Gallery</a></li>
            <li><a href="#booking">Booking</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>

    <section id="about" class="section">
        <div class="container">
            <h2>About Us</h2>
            <p>Kaimana Car Rental & Travel offers reliable car rentals and tour packages to explore Papua's natural beauty.</p>
        </div>
    </section>

    <section id="services" class="section">
        <div class="container">
            <h2>Our Services</h2>
            <div class="services-grid">
                <div class="service">
                    <h3>Car Rental</h3>
                    <ul>
                        <li>Daily Rental</li>
                        <li>Weekly Rental</li>
                        <li>Monthly Rental</li>
                    </ul>
                </div>
                <div class="service">
                    <h3>Tour Packages</h3>
                    <ul>
                        <li>3-Day Triton Bay Package</li>
                        <li>1-Day Marsi Skywalk & Air Bubara Tour</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="gallery" class="section">
        <div class="container">
            <h2>Gallery</h2>
            <div class="gallery-grid">
                <img src="car.jpg" alt="Car Rental">
                <img src="kaimana.jpg" alt="Kaimana Beach">
                <img src="bubara.jpg" alt="Kali Bubara">
            </div>
        </div>
    </section>

    <section id="booking" class="section">
        <div class="container">
            <h2>Booking Form</h2>
            <form id="bookingForm">
                <label for="name">Full Name:</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Email:</label>
                <input type="email" id="email" name="email" required>

                <label for="phone">Phone Number:</label>
                <input type="tel" id="phone" name="phone" required>

                <label for="service">Service Type:</label>
                <select id="service" name="service" required>
                    <option value="Car Rental">Car Rental</option>
                    <option value="3-Day Triton Bay Package">3-Day Triton Bay Package</option>
                    <option value="1-Day Marsi Skywalk & Air Bubara Tour">1-Day Marsi Skywalk & Air Bubara Tour</option>
                </select>

                <label for="date">Booking Date:</label>
                <input type="date" id="date" name="date" required>

                <label for="message">Additional Notes:</label>
                <textarea id="message" name="message"></textarea>

                <button type="submit">Submit</button>
            </form>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="container">
            <h2>Contact Us</h2>
            <p>Email: <a href="mailto:jemaatkaimanaq@gmail.com">jemaatkaimanaq@gmail.com</a></p>
            <p>Phone: <a href="tel:+6282197718876">+62 821 9771 8876</a></p>
            <p><a href="https://wa.me/6282197718876" target="_blank">Chat via WhatsApp</a></p>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 Kaimana Car Rental & Travel. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>


---

2. styles.css (Styling)

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    color: #333;
    background-color: #f8f8f8;
}

header.hero {
    background: url('hero-image.jpg') no-repeat center center/cover;
    color: white;
    text-align: center;
    padding: 100px 20px;
}

.hero .btn {
    background: #007BFF;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
}

nav {
    background: #007BFF;
    padding: 10px 0;
    text-align: center;
}

nav ul {
    list-style: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 15px;
}

nav ul li a {
    color: white;
    text-decoration: none;
}

.section {
    padding: 50px 20px;
    text-align: center;
}

form input, form select, form textarea {
    display: block;
    width: 80%;
    margin: 10px auto;
    padding: 10px;
}

button {
    background: #007BFF;
    color: white;
    padding: 10px;
    border: none;
    cursor: pointer;
}


---

3. script.js (Form Submission)

document.getElementById("bookingForm").addEventListener("submit", function(event) {
    event.preventDefault();

    let name = document.getElementById("name").value;
    let phone = document.getElementById("phone").value;
    let service = document.getElementById("service").value;
    let date = document.getElementById("date").value;

    let whatsappMessage = `Hello, I would like to book: 
    Name: ${name}
    Phone: ${phone}
    Service: ${service}
    Date: ${date}`;

    window.open(https://wa.me/6282197718876?text=${encodeURIComponent(whatsappMessage)}, "_blank");
});


---

Instructions to Use

1. Upload these files to GitHub.


2. Enable GitHub Pages in the repository settings.


3. Your website will be live on https://your-github-username.github.io/kaimana-car-rental/.




---

Now, all booking requests will be sent directly to your WhatsApp!
Let me know if you need help deploying it!
