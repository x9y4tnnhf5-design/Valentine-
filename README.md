# Valentine-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Verification Required</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(135deg, #ff9a9e, #fad0c4);
      height: 100vh;
      margin: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #333;
    }
    .card {
      background: white;
      padding: 30px;
      border-radius: 12px;
      text-align: center;
      width: 320px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
    }
    button {
      padding: 10px 20px;
      margin: 10px;
      border: none;
      border-radius: 8px;
      font-size: 16px;
      cursor: pointer;
    }
    .yes {
      background-color: #ff4d6d;
      color: white;
    }
    .no {
      background-color: #ddd;
      color: #333;
    }
    .hidden {
      display: none;
    }
  </style>
</head>
<body>

  <div class="card" id="question">
    <h2>Elizabeth 💕</h2>
    <p>Will you be my Valentine?</p>
    <button class="yes" onclick="showYes()">YES ❤️</button>
    <button class="no" onclick="showNo()">NO ❌</button>
  </div>

  <div class="card hidden" id="yes">
    <h2>🎉 SUCCESS 🎉</h2>
    <p>
      Congratulations Elizabeth 💖<br><br>
      You are officially my Valentine 🥰<br><br>
      Benefits include unlimited hugs, snacks,
      and lifetime love 💘
    </p>
  </div>

  <div class="card hidden" id="no">
    <h2>❌ ERROR 404 ❌</h2>
    <p>
      Choice Not Found<br><br>
      The option “No” does not exist 😌<br><br>
      Please go back and select YES ❤️
    </p>
  </div>

  <script>
    function showYes() {
      document.getElementById('question').classList.add('hidden');
      document.getElementById('yes').classList.remove('hidden');
    }
    function showNo() {
      document.getElementById('question').classList.add('hidden');
      document.getElementById('no').classList.remove('hidden');
    }
  </script>

</body>
</html>