<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Welcome</title>
  <style>
    body {
      width: 100%;
      height: 100%;
      margin: 0;
      font-family: arial;
      background: linear-gradient(to right, green, white);
    }

    .container {
      display: flex;
      justify-content: center;
      padding: 20px;
    }

    .title {
      width: 100%;
      margin-top: 50px;
      text-align: center;
    }

    .title h1 {
      font-size: 3rem;
      font-family: arial;
      margin: 0;
    }

    .title p {
      margin: 0;
      font-size: 1rem;
    }

    button {
      width: 30%;
      padding: 10px;
      background-color: green;
      color: black;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin-top: 10px;
      transition: background-color 0.3s, transform 0.2s;
    }

    button:hover {
      background-color: yellow;
      border: 1px solid black;
      transform: translateY(-2px);
    }

    .user {
      width: 100%;
      margin-top: 70px;
      text-align: center;
    }

    /* Media Queries */
    @media (max-width: 768px) {
      .title h1 {
        font-size: 2rem;
      }
      
      button {
        width: 60%;
      }
      
      .user {
        margin-top: 40px;
      }
    }

    @media (max-width: 480px) {
      .title h1 {
        font-size: 1.5rem;
      }
      
      button {
        width: 80%;
        padding: 12px;
      }
      
      .title {
        margin-top: 30px;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="title">
      <p><b>Welcome to</b></p>
      <h1>Bulacan Polytechnic College</h1>
      <p>Online Environment</p><br>

      <div class="user">
        <h3>Login as:</h3>
        <button onclick="student()">Student</button><br>
        <button onclick="instructor()">Instructor</button><br>
        <button onclick="admin()">Admin</button>
      </div>
    </div>
  </div>

  <script>
    function student() {
      alert("Proceed to Login");
      window.location.href = "studentlogin.html";
    }

    function instructor() {
     alert("Proceed to Login");;
      window.location.href = "instuctorlogin.html";
    }

    function admin() {
      alert("Proceed to Login");
      window.location.href = "adminlogin.html";
    }
  </script>
</body>
</html>
