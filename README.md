# landing-page
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Landing Page</title>
  <style>
    /* Reset */
    * { margin: 0; padding: 0; box-sizing: border-box; }

    body {
      font-family: Arial, sans-serif;
      line-height: 1.6;
      background: #f4f4f4;
      color: #333;
    }

    header {
      background: #4CAF50;
      color: white;
      padding: 40px 20px;
      text-align: center;
    }

    header h1 { font-size: 2.5rem; }
    header p { font-size: 1.2rem; margin: 10px 0; }

    .btn {
      display: inline-block;
      margin-top: 15px;
      padding: 10px 20px;
      background: #fff;
      color: #4CAF50;
      border-radius: 5px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s;
    }
    .btn:hover { background: #ddd; }

    section {
      padding: 40px 20px;
      text-align: center;
    }

    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to My Landing Page</h1>
    <p>Build your online presence with a simple, clean design.</p>
    <a href="#signup" class="btn">Get Started</a>
  </header>

  <section>
    <h2>Why Choose Us?</h2>
    <p>We create beautiful, responsive websites that help you grow.</p>
  </section>

  <section id="signup">
    <h2>Sign Up Now</h2>
    <form onsubmit="return showMessage(event)">
      <input type="email" placeholder="Enter your email" required>
      <button type="submit" class="btn">Join</button>
    </form>
    <p id="message" style="margin-top:15px; color: green; font-weight:bold;"></p>
  </section>

  <footer>
    <p>&copy; 2025 My Landing Page. All rights reserved.</p>
  </footer>

  <script>
    function showMessage(e) {
      e.preventDefault();
      document.getElementById("message").textContent = "✅ Thank you for signing up!";
    }
  </script>
</body>
</html>
