<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Hello Lama</title>
  <style>
    body {
      margin: 0;
      background-color: pink;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      font-family: Arial, sans-serif;
    }

    #helloButton {
      background-color: white;
      color: black;
      border: none;
      padding: 20px 40px;
      font-size: 24px;
      border-radius: 12px;
      cursor: pointer;
      transition: transform 0.2s;
    }

    #helloButton:hover {
      transform: scale(1.05);
    }

    #animation {
      display: none;
      font-size: 36px;
      color: white;
      text-align: center;
      animation: fadeIn 2s ease-in-out;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>
  <div id="container">
    <button id="helloButton">Hello Lama</button>
    <div id="animation">أنا أحب قلبك ♥️</div>
  </div>

  <script>
    const button = document.getElementById('helloButton');
    const animation = document.getElementById('animation');

    button.addEventListener('click', () => {
      button.style.display = 'none';
      animation.style.display = 'block';
    });
  </script>
</body>
</html>
