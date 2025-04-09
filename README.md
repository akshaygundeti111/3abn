<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Donate to 3ABN</title>
  <link rel="icon" href="3abn-logo.png" />
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Open Sans', Arial, sans-serif;
      background-color: #f2f7fc;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #ffffff;
      padding: 15px 20px;
      display: flex;
      align-items: center;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    header img {
      height: 60px;
      margin-right: 15px;
    }

    header span {
      color: #0077C8;
      font-size: 24px;
      font-weight: bold;
    }

    .container {
      max-width: 500px;
      margin: 50px auto;
      padding: 30px;
      background: #fff;
      border-radius: 10px;
      box-shadow: 0 0 20px rgba(0,0,0,0.1);
    }

    h2 {
      text-align: center;
      color: #0077C8;
      margin-bottom: 20px;
    }

    label {
      font-weight: bold;
      display: block;
      margin-top: 15px;
    }

    input, select {
      width: 100%;
      padding: 10px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 6px;
      font-size: 14px;
    }

    .btn {
      margin-top: 20px;
      background-color: #0077C8;
      color: white;
      border: none;
      padding: 12px;
      font-size: 16px;
      width: 100%;
      border-radius: 6px;
      cursor: pointer;
      font-weight: bold;
    }

    .btn:hover {
      background-color: #005fa3;
    }
  </style>
</head>
<body>

  <header>
    <img src="3abn-logo.png" alt="3ABN Logo">
    <span>3ABN</span>
  </header>

  <div class="container">
    <h2>Make a Donation</h2>
    <form id="donationForm">
      <label for="name">Full Name</label>
      <input type="text" id="name" required>

      <label for="email">Email Address</label>
      <input type="email" id="email" required>

      <label for="phone">Phone Number</label>
      <input type="tel" id="phone" required>

      <label for="area">Select Donation Area</label>
      <select id="area" required>
        <option value="">-- Select Donation Area --</option>
        <option value="TV Ministry">TV Ministry</option>
        <option value="Evangelism">Evangelism</option>
        <option value="Children's Ministry">Children's Ministry</option>
      </select>

      <label for="amount">Donation Amount (USD)</label>
      <input type="number" id="amount" required>

      <button type="submit" class="btn">Proceed to Payment</button>
    </form>
  </div>

  <script>
    document.getElementById("donationForm").addEventListener("submit", function(e) {
      e.preventDefault();

      // Redirect to PayPal or payment gateway
      window.location.href = "https://www.paypal.com/donate/?hosted_button_id=UYJVUZRSBUCYY";
    });
  </script>
</body>
</html>
