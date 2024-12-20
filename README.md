<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Legion Motorcycle Club</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #000000;
            color: #ff0000;
        }
        header {
            background-color: #2b2b2b;
            padding: 20px;
            text-align: center;
        }
        header h1 {
            margin: 0;
        }
        nav {
            background-color: #333;
            overflow: hidden;
        }
        nav a {
            float: left;
            display: block;
            color: #fff;
            text-align: center;
            padding: 14px 16px;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #575757;
        }
        .container {
            padding: 20px;
        }
        footer {
            background-color: #2b2b2b;
            text-align: center;
            padding: 10px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>

<header>
    <h1>Legion Motorcycle Club</h1>
    <p>Ride with Honor, Live with Pride</p>
</header>

<nav>
    <a href="#about">About Us</a>
    <a href="#events">Events</a>
    <a href="#gallery">Gallery</a>
    <a href="#contact">Contact</a>
</nav>

<div class="container" id="about">
    <h2>About Us</h2>
    <p>Welcome to the Legion Motorcycle Club. We are a group of passionate motorcycle enthusiasts who share a love for the open road, camaraderie, and living life to the fullest. Our club is built on principles of honor, respect, and loyalty.</p>
</div>

<div class="container" id="events">
    <h2>Events</h2>
    <p>Join us for our upcoming events and rides. Whether it's a charity ride, a road trip, or a social gathering, our events are always filled with excitement and brotherhood.</p>
    <ul>
        <li>Annual Charity Ride - January 15, 2025</li>
        <li>Spring Road Trip - April 10, 2025</li>
        <li>Summer BBQ & Ride - July 25, 2025</li>
    </ul>
</div>

<div class="container" id="gallery">
    <h2>Gallery</h2>
    <p>Check out some of the photos from our recent rides and events.</p>
    <div id="photoGallery">
        <!-- Images can be added here -->
    </div>
</div>

<div class="container" id="contact">
    <h2>Contact Us</h2>
    <p>Have any questions or want to join our club? Reach out to us!</p>
    <form id="contactForm">
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name"><br><br>
        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email"><br><br>
        <label for="message">Message:</label><br>
        <textarea id="message" name="message"></textarea><br><br>
        <button type="button" onclick="submitForm()">Submit</button>
    </form>
</div>

<footer>
    <p>&copy; 2025 Legion Motorcycle Club. All rights reserved.</p>
</footer>

<script>
    function submitForm() {
        const name = document.getElementById('name').value;
        const email = document.getElementById('email').value;
        const message = document.getElementById('message').value;
        
        if (name && email && message) {
            alert('Thank you for contacting us, ' + name + '! We will get back to you shortly.');
            document.getElementById('contactForm').reset();
        } else {
            alert('Please fill in all fields before submitting.');
        }
    }
</script>

</body>
</html>
