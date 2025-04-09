<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Donate to 3ABN</title>
  <link rel="icon" type="image/png" href="https://3abn.org/sites/all/themes/zen3abn/logo.png">
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Open Sans', Arial, sans-serif;
      background-color: #ffffff;
      color: #222;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #0077C8;
      padding: 10px 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
    }

    .logo {
      display: flex;
      align-items: center;
    }

    .logo img {
      height: 60px;
      margin-right: 10px;
    }

    .nav-links {
      display: flex;
      gap: 20px;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      font-weight: bold;
    }

    .container {
      max-width: 600px;
      margin: 40px auto;
      padding: 20px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      border-radius: 10px;
      background-color: #f9f9f9;
    }

    h2 {
      text-align: center;
      color: #0077C8;
    }

    label {
      display: block;
      margin-top: 15px;
      font-weight: bold;
    }

    input, select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }

    .btn {
      background-color: #0077C8;
      color: white;
      padding: 12px;
      width: 100%;
      border: none;
      border-radius: 6px;
      margin-top: 20px;
      font-size: 16px;
      cursor: pointer;
    }

    .btn:hover {
      background-color: #005fa3;
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">
      <img src="https://3abn.org/sites/all/themes/zen3abn/logo.png" alt="3ABN Logo">
      <span style="color: white; font-size: 22px; font-weight: bold;">3ABN</span>
    </div>
    <nav class="nav-links">
      <a href="#">Home</a>
      <a href="#">Watch</a>
      <a href="#">Donate</a>
      <a href="#">Schedule</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <div class="container">
    <h2>Donate to 3ABN</h2>
    <form id="donationForm">
      <label for="name">Full Name:</label>
      <input type="text" id="name" required>

      <label for="email">Email Address:</label>
      <input type="email" id="email" required>

      <label for="phone">Phone Number:</label>
      <input type="tel" id="phone" required>

      <label for="area">Donation Area:</label>
      <select id="area" required>
        <option value="">-- Select --</option>
        <option value="Child Welfare">Child Welfare</option>
        <option value="TV Ministry">TV Ministry</option>
        <option value="Global Outreach">Global Outreach</option>
      </select>

      <label for="amount">Donation Amount (USD):</label>
      <input type="number" id="amount" min="1" required>

      <button type="submit" class="btn">Proceed to Payment</button>
    </form>
  </div>

  <script>
    document.getElementById("donationForm").addEventListener("submit", function(e) {
      e.preventDefault();
      
      // You could log details or store here

      // Redirect to PayPal
      window.location.href = "https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=UYJVUZRSBUCYY&source=url&ssrt=1744192747654";
    });
  </script>
</body>
</html>
