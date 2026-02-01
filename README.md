# Valentine-for-shuttumani-
Valentine for shuttumani 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Valentine 💖</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: pink;
      font-family: Arial, sans-serif;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      overflow: hidden;
    }

    h1 {
      text-align: center;
      margin-bottom: 40px;
    }

    button {
      font-size: 22px;
      padding: 12px 30px;
      border: none;
      border-radius: 10px;
      cursor: pointer;
    }

    #yes {
      background-color: #ff4d6d;
      color: white;
    }

    #no {
      position: absolute;
      background-color: #444;
      color: white;
    }
  </style>
</head>
<body>

  <h1>💖 Shuttumani, will you be my Valentine? 💖</h1>

  <button id="yes" onclick="yesClicked()">YES 💘</button>
  <button id="no">NO 😅</button>

  <script>
    const noBtn = document.getElementById("no");

    function moveNoButton() {
      const x = Math.random() * (window.innerWidth - noBtn.offsetWidth);
      const y = Math.random() * (window.innerHeight - noBtn.offsetHeight);
      noBtn.style.left = x + "px";
      noBtn.style.top = y + "px";
    }

    // Move continuously
    setInterval(moveNoButton, 600);

    function yesClicked() {
      document.body.innerHTML = `
        <h1>🎉 YAY SHUTTUMANI!!! 🎉</h1>
        <p>I knew you'd say YES ❤️</p>
      `;
    }
  </script>

</body>
</html>

