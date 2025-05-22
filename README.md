<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Love of my life</title>
  <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Open+Sans&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Open Sans', sans-serif;
      background: url('background.jpg.jpg') no-repeat center center fixed;
      background-size: cover;
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      color: #fff;
    }

    .card {
      background: rgba(0, 0, 0, 0.6);
      padding: 40px;
      border-radius: 20px;
      text-align: center;
      max-width: 600px;
      width: 90%;
      box-shadow: 0 8px 24px rgba(0,0,0,0.3);
    }

    h1 {
      font-family: 'Great Vibes', cursive;
      font-size: 40px;
      color: #ffc0cb;
      margin-bottom: 10px;
    }

    input {
      padding: 10px 15px;
      font-size: 18px;
      border: none;
      border-radius: 10px;
      outline: none;
      margin-top: 15px;
    }

    button {
      margin-top: 10px;
      padding: 10px 20px;
      font-size: 18px;
      background-color: #ff69b4;
      color: white;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }

    #message {
      margin-top: 30px;
      font-size: 20px;
      line-height: 1.5;
      color: #ffebf0;
    }
  </style>
</head>
<body>
  <div class="card">
    <h1>Love of my life</h1>
    <p>Type "Hi" and click the button</p>
    <input type="text" id="inputText" placeholder="Type here..." />
    <br>
    <button onclick="showMessage()">Enter Hi</button>
    <div id="message"></div>
  </div>

  <script>
    const loveLines = [
      "You’re my today and all of my tomorrows.",
      "You are my heart’s most peaceful place.",
      "Loving you is my favorite habit.",
      "I didn’t believe in soulmates until you.",
      "You are my once-in-a-lifetime.",
      "My world begins and ends with you.",
      "Life makes perfect sense with you.",
      "With you, every day is worth waking up for.",
      "You’re not my option — you’re my everything.",
      "You light up my darkest days.",
      "I’m better because of you.",
      "You are my person. Always.",
      "Even forever feels short with you.",
      "You’re my smile in every moment.",
      "You're the reason I believe in magic.",
      "Home is wherever you're with me.",
      "You're the melody to my silent heart.",
      "You’re the calm in all my storms.",
      "Your love is my favorite story.",
      "My love for you only grows stronger.",
      "I fall for you more every day.",
      "You’re the peace I prayed for."
    ];

    function showMessage() {
      const input = document.getElementById("inputText").value.trim().toLowerCase();
      const messageDiv = document.getElementById("message");
      if (input === "hi") {
        const randomLine = loveLines[Math.floor(Math.random() * loveLines.length)];
        messageDiv.innerHTML = `
          Swetha, En Pondatti, I'm one ring/message away from you!<br><br>
          ❤️ ${randomLine}
        `;
      } else {
        messageDiv.textContent = "Just say Hi, my love ❤️";
      }
    }
  </script>
</body>
</html>
