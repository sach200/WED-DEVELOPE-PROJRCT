# WED-DEVELOPE-PROJRCT
CREATING AND DEPLOYING A LANDING PAGE FOR WEBSITE
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Landing Page</title>
    <style>
        /* CSS Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
        }

        .container {
            width: 80%;
            margin: 0 auto;
            text-align: center;
        }

        header {
            background-color: #4CAF50;
            color: white;
            padding: 60px 0;
        }

        header h1 {
            font-size: 48px;
        }

        header p {
            font-size: 20px;
            margin-top: 20px;
        }

        .cta-button {
            display: inline-block;
            background-color: #ff6347;
            color: white;
            padding: 15px 30px;
            text-decoration: none;
            font-size: 18px;
            border-radius: 5px;
            margin-top: 20px;
        }

        .cta-button:hover {
            background-color: #ff4500;
        }

        .cta-section {
            padding: 40px 0;
            background-color: #ffffff;
        }

        .cta-section h2 {
            font-size: 36px;
        }

        .cta-section p {
            font-size: 18px;
            margin: 20px 0;
        }

        form {
            display: flex;
            justify-content: center;
            gap: 10px;
        }

        input[type="email"] {
            padding: 10px;
            font-size: 16px;
            width: 300px;
            border: 1px solid #ddd;
            border-radius: 5px;
        }

        button {
            padding: 10px 20px;
            font-size: 16px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #45a049;
        }

        footer {
            background-color: #333;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
    </style>
</head>

<body>

    <!-- Landing Page Content -->
    <header>
        <div class="container">
            <h1>Welcome to My Landing Page</h1>
            <p>Your journey begins here!</p>
            <a href="#cta" class="cta-button">Get Started</a>
        </div>
    </header>

    <section id="cta" class="cta-section">
        <div class="container">
            <h2>Ready to Get Started?</h2>
            <p>Sign up now to unlock exclusive content!</p>
            <form id="signupForm" action="#">
                <input type="email" id="emailInput" placeholder="Enter your email" required>
                <button type="submit">Sign Up</button>
            </form>
        </div>
    </section>

    <footer>
        <p>&copy; 2025 My Landing Page. All rights reserved.</p>
    </footer>

    <!-- JavaScript to handle form submission -->
    <script>
        // JavaScript to handle form submission and show a thank-you message
        document.getElementById('signupForm').addEventListener('submit', function (e) {
            e.preventDefault(); // Prevent page reload

            const email = document.getElementById('emailInput').value;
            alert(`Thank you for subscribing with: ${email}`);
        });
    </script>

</body>

</html>

