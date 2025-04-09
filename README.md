<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Donate to 3ABN</title>
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
    }
    body {
      font-family: 'Open Sans', sans-serif;
      margin: 0;
      background-color: #f1f5f9;
      color: #333;
    }
    header {
      background-color: #ffffff;
      padding: 20px 40px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.05);
      display: flex;
      align-items: center;
      justify-content: center;
    }
    .logo {
      font-size: 28px;
      font-weight: 600;
      color: #005da4;
    }
    main {
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: calc(100vh - 100px);
      padding: 40px 20px;
    }
    .form-container {
      background: #ffffff;
      padding: 30px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
      max-width: 450px;
      width: 100%;
    }
    h2 {
      text-align: center;
      margin-bottom: 25px;
      color: #005da4;
    }
    input, select, button {
      width: 100%;
      padding: 12px;
      margin: 10px 0;
      font-size: 16px;
      border: 1px solid #ccc;
      border-radius: 6px;
    }
    button {
      background-color: #005da4;
      color: white;
      border: none;
      font-weight: 600;
      cursor: pointer;
      transition: background 0.3s;
    }
    button:hover {
      background-color: #004b87;
    }
    footer {
      text-align: center;
      padding: 20px;
      font-size: 14px;
      color: #888;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">3ABN</div>
  </header>

  <main>
    <div class="form-container">
      <h2>Make a Donation</h2>
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
        <button type="submit">Proceed to PayPal</button>
      </form>
    </div>
  </main>

  <footer>
    &copy; 2025 3ABN. All Rights Reserved.
  </footer>

  <script>
    document.getElementById("donationForm").addEventListener("submit", function(event) {
      event.preventDefault();

      const name = document.getElementById("name").value;
      alert("Thank you, " + name + "! Redirecting to PayPal...");

      window.location.href = "https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=UYJVUZRSBUCYY&source=url&ssrt=1744192747654";
    });
  </script>
</body>
</html>
