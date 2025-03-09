# VR
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VR TechCon 2025</title>
    <style>
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #1a1a2e;
            color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        }
        nav {
            background-color: #222831;
            text-align: center;
            padding: 12px;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 20px;
            font-weight: 600;
            font-size: 1.2rem;
        }
        nav a:hover {
            color: #ff6347;
            text-decoration: underline;
        }
        section {
            padding: 20px;
            margin: 20px auto;
            max-width: 900px;
            background-color: #16213e;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
        }
        section h2 {
            color: #4CAF50;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 15px;
            background: white;
            color: black;
        }
        table th, table td {
            border: 1px solid #ddd;
            padding: 12px;
            text-align: left;
        }
        table th {
            background-color: #4CAF50;
            color: white;
        }
        table tr:nth-child(even) {
            background-color: #f9f9f9;
        }
        #countdown {
            font-size: 1.5rem;
            text-align: center;
            font-weight: bold;
            color: #ff6347;
        }
        form {
            max-width: 600px;
            margin: auto;
        }
        form label {
            display: block;
            margin: 8px 0;
            font-weight: 600;
        }
        form input, form textarea, form select, form button {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
        }
        form input, form textarea {
            background-color: #222;
            color: white;
        }
        form select {
            background-color: #4CAF50;
            color: white;
        }
        form button {
            background-color: #ff6347;
            color: white;
            font-weight: 700;
            cursor: pointer;
        }
        form button:hover {
            background-color: #e04e3f;
        }
        footer {
            background-color: #222831;
            padding: 20px;
            text-align: center;
        }
        footer a {
            color: #4CAF50;
            text-decoration: none;
            margin: 0 10px;
        }
        footer a:hover {
            color: #ff6347;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to VR TechCon 2025</h1> 
        <p>The Ultimate Technology and Programming Conference</p>
        <div id="countdown">Event starts in: <span id="timer"></span></div>
    </header>
    <nav>
        <a href="#about">About</a> |
        <a href="#schedule">Schedule</a> |
        <a href="#events">Upcoming Events</a> |
        <a href="#rsvp">RSVP</a> |
        <a href="#contact">Contact</a>
    </nav>

    <section id="about">
        <h2>About the Event</h2>
        <p>VR TechCon 2025 brings together leading minds in programming, 
            tech, and innovation. Join us for insightful talks, hands-on workshops,
            and an opportunity to network with professionals worldwide.</p>
    </section>

    <section id="schedule">
        <h2>Event Schedule</h2>
        <table>
            <thead>
                <tr>
                    <th>Time</th>
                    <th>Session</th>
                    <th>Speaker</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>9:00 AM</td>
                    <td>Opening Keynote</td>
                    <td>VRPlatform</td> 
                </tr>
                <tr>
                    <td>10:30 AM</td>
                    <td>Understanding AI and Machine Learning</td>
                    <td>Mr. Arvind Kumar</td>
                </tr>
                <tr>
                    <td>1:00 PM</td>
                    <td>Lunch Break</td>
                    <td>-</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section id="events">
        <h2>Upcoming Events</h2>
        <ul>
            <li><strong>March 15:</strong> AI & VR in Gaming</li>
            <li><strong>April 10:</strong> Blockchain for Secure Transactions</li>
            <li><strong>May 5:</strong> Future of Quantum Computing</li>
        </ul>
    </section>

    <section id="rsvp">
        <h2>RSVP for the Event</h2>
        <form id="rsvp-form">
            <label for="rsvp-name">Name:</label>
            <input type="text" id="rsvp-name" name="rsvp-name" placeholder="Enter your name" required>

            <label for="rsvp-email">Email:</label>
            <input type="email" id="rsvp-email" name="rsvp-email" placeholder="Enter your email" required>

            <button type="submit">RSVP Now</button>
        </form>
    </section>

    <footer>
        <h3>Follow Us</h3>
        <p>
            <a href="https://www.facebook.com/YOUR_FACEBOOK_ID" target="_blank">Facebook</a> | 
            <a href="https://www.instagram.com/YOUR_INSTAGRAM_ID" target="_blank">Instagram</a> | 
            <a href="https://twitter.com/YOUR_TWITTER_ID" target="_blank">Twitter</a> | 
            <a href="https://www.linkedin.com/in/YOUR_LINKEDIN_ID" target="_blank">LinkedIn</a>
        </p>
    </footer>

    <script>
        // Countdown Timer
        function updateCountdown() {
            const eventDate = new Date("2025-06-15T09:00:00").getTime();
            const now = new Date().getTime();
            const timeLeft = eventDate - now;
            
            const days = Math.floor(timeLeft / (1000 * 60 * 60 * 24));
            const hours = Math.floor((timeLeft % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
            const minutes = Math.floor((timeLeft % (1000 * 60 * 60)) / (1000 * 60));
            const seconds = Math.floor((timeLeft % (1000 * 60)) / 1000);

            document.getElementById("timer").innerHTML = `${days}d ${hours}h ${minutes}m ${seconds}s`;
        }
        setInterval(updateCountdown, 1000);

        // RSVP Form Alert
        document.getElementById("rsvp-form").addEventListener("submit", function(event) {
            event.preventDefault();
            alert("Thank you for RSVPing! We’ll send event updates to your email.");
        });
    </script>
</body>
</html>
    <section id="payment">
        <h2>Ticket Payment</h2>
        <form>
            <label for="ticket-type">Select Ticket Type:</label>
            <select id="ticket-type" name="ticket-type">
                <option value="general">General Admission - $20</option>
                <option value="vip">VIP Pass - $50</option>
            </select>

            <label for="payment-method">Choose Payment Method:</label>
            <select id="payment-method" name="payment-method">
                <option value="credit">Credit Card</option>
                <option value="paypal">PayPal</option>
                <option value="crypto">Cryptocurrency</option>
            </select>

            <button type="submit">Proceed to Payment</button>
        </form>
    </section>
