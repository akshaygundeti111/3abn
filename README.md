<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Donate to 3ABN</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f9f9f9;
      text-align: center;
    }
    .container {
      max-width: 400px;
      margin: 50px auto;
      padding: 30px;
      background-color: #fff;
      border-radius: 10px;
      box-shadow: 0px 0px 10px rgba(0,0,0,0.1);
    }
    h2 {
      margin-bottom: 20px;
    }
    input, select, button {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      font-size: 16px;
    }
    button {
      background-color: #2574db;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #1a5bbf;
    }
    .logo {
      font-size: 26px;
      color: #2574db;
      font-weight: bold;
    }
  </style>
</head>
<body>
  <div class="logo">3ABN</div>
  <div class="container">
    <h2>Donate to 3ABN</h2>
    <form id="donationForm">
      <input type="text" id="name" placeholder="Full Name" required />
      <input type="email" id="email" placeholder="Email Address" required />
      <input type="tel" id="phone" placeholder="Phone Number" required />
      <select id="area" required>
        <option value="">Select Donation Area</option>
        <option>Child Welfare</option>
        <option>Education</option>
        <option>Medical Help</option>
      </select>
      <input type="number" id="amount" placeholder="Donation Amount (USD)" required />
      <button type="submit">Proceed to Payment</button>
    </form>
  </div>

  <script>
    document.getElementById("donationForm").addEventListener("submit", function(event) {
      event.preventDefault();

      // Collect form values if needed (optional)
      const name = document.getElementById("name").value;
      alert("Thank you, " + name + "! Redirecting to PayPal...");

      // Redirect to PayPal donation page
      window.location.href = "https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=UYJVUZRSBUCYY&source=url&ssrt=1744192747654";
    });
  </script>
</body>
</html>
