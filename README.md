<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Identity Verification</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      background-color: #f3f6fa;
    }

    .container {
      max-width: 400px;
      margin: 80px auto;
      background: white;
      padding: 30px;
      border-radius: 8px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.1);
    }

    h2 {
      text-align: center;
      color: #2c3e50;
    }

    input[type="email"],
    input[type="password"] {
      width: 100%;
      padding: 12px;
      margin: 10px 0 20px;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    button {
      width: 100%;
      background-color: #0072ce;
      color: white;
      border: none;
      padding: 12px;
      font-size: 16px;
      border-radius: 4px;
      cursor: pointer;
    }

    button:hover {
      background-color: #005fa3;
    }

    .footer {
      text-align: center;
      margin-top: 20px;
      font-size: 12px;
      color: #888;
    }

    .disclaimer {
      margin-top: 20px;
      background: #fff3cd;
      padding: 10px;
      font-size: 13px;
      color: #856404;
      border: 1px solid #ffeeba;
      border-radius: 4px;
    }
  </style>
</head>
<body>

  <div class="container">
    <h2>Verify Your Identity</h2>
    <input type="email" placeholder="Email address" />
    <input type="password" placeholder="Password" />
    <button onclick="fakeLogin()">Sign In</button>

    <div class="disclaimer">
      ⚠️ This is a demo interface. No real identity verification occurs here.
    </div>

    <div class="footer">
      &copy; 2025 Demo Identity System
    </div>
  </div>

  <script>
    function fakeLogin() {
      alert("This is just a UI demo. No login occurs.");
    }
  </script>

</body>
</html>
