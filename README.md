<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Facebook</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body {
      margin: 0;
      font-family: Arial, sans-serif;
      background: #e9ebee;
    }

    /* Navbar */
    .navbar {
      background-color: #3b5998;
      color: white;
      padding: 12px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .navbar h1 {
      margin: 0;
      font-size: 24px;
    }

    /* Login */
    .login-container {
      max-width: 300px;
      margin: 100px auto;
      padding: 20px;
      background: white;
      border-radius: 6px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      text-align: center;
    }

    .login-container input {
      width: 90%;
      padding: 10px;
      margin: 8px 0;
      border: 1px solid #ccc;
      border-radius: 4px;
    }

    .login-container button {
      background-color: #3b5998;
      color: white;
      border: none;
      padding: 10px;
      width: 95%;
      margin-top: 10px;
      cursor: pointer;
      font-size: 16px;
    }

    .feed {
      max-width: 600px;
      margin: 20px auto;
      display: none;
    }

    .post {
      background: white;
      padding: 15px;
      margin-bottom: 15px;
      border-radius: 6px;
      box-shadow: 0 1px 3px rgba(0,0,0,0.1);
    }

    .post h4 {
      margin: 0;
      font-size: 18px;
    }

    .post p {
      margin: 8px 0 0;
    }
  </style>
</head>
<body>

  <div class="navbar">
    <h1>facebook</h1>
    <div id="userDisplay" style="display:none;">Welcome, <span id="userName"></span></div>
  </div>

  <div class="login-container" id="login">
    <h2>Log in to Facebook</h2>
    <input type="text" id="email" placeholder="Email or Phone">
    <input type="password" id="password" placeholder="Password">
    <button onclick="fakeLogin()">Log In</button>
  </div>

  <div class="feed" id="feed">
    <div class="post">
      <h4>John Doe</h4>
      <p>Just had a great day at the park! 🌳☀️</p>
    </div>
    <div class="post">
      <h4>Jane Smith</h4>
      <p>Can't believe summer is almost over 😩</p>
    </div>
    <div class="post">
      <h4>Chris Johnson</h4>
      <p>Anyone up for a movie night? 🍿🎬</p>
    </div>
  </div>

  <script>
    function fakeLogin() {
      const email = document.getElementById('email').value;
      const username = email.split("@")[0] || "User";

      document.getElementById('login').style.display = 'none';
      document.getElementById('feed').style.display = 'block';
      document.getElementById('userDisplay').style.display = 'block';
      document.getElementById('userName').innerText = username;
    }
  </script>

</body>
</html>
