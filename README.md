<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>3ABN Donation Form</title>
  <style>
    body { font-family: Arial, sans-serif; padding: 40px; background: #f7f7f7; }
    form { background: #fff; padding: 20px; border-radius: 10px; max-width: 500px; margin: auto; box-shadow: 0 0 10px rgba(0,0,0,0.1); }
    label { display: block; margin-top: 15px; font-weight: bold; }
    input, select, button { width: 100%; padding: 10px; margin-top: 5px; border-radius: 5px; border: 1px solid #ccc; }
    button { background-color: #0070ba; color: white; border: none; cursor: pointer; }
    button:hover { background-color: #005ea6; }
  </style>
</head>
<body>

  <h2 style="text-align:center;">Donate to 3ABN</h2>

  <form id="donationForm">
    <label for="name">Full Name:</label>
    <input type="text" name="name" required>

    <label for="email">Email Address:</label>
    <input type="email" name="email" required>

    <label for="phone">Phone Number:</label>
    <input type="text" name="phone">

    <label for="donationArea">Donation Area:</label>
    <select name="donationArea">
      <option value="Child Welfare">Child Welfare</option>
      <option value="Women Support">Women Support</option>
      <option value="Elderly Aid">Elderly Aid</option>
      <option value="War Relief">War Relief</option>
    </select>

    <label for="amount">Donation Amount (USD):</label>
    <input type="number" name="amount" required>

    <button type="submit">Proceed to Payment</button>
  </form>

  <script>
    document.getElementById('donationForm').addEventListener('submit', function(e) {
      e.preventDefault();

      // Later: You can add a POST to a NetSuite RESTlet here.

      // Redirect to PayPal donation page
      window.location.href = "https://www.paypal.com/donate/?cmd=_s-xclick&hosted_button_id=UYJVUZRSBUCYY&source=url&ssrt=1744178200616";
    });
  </script>

</body>
</html>
