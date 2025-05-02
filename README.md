<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Trust Me</title>
  <style>
    body {
      margin: 0;
      background: black;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      font-family: sans-serif;
    }
    #trust-btn {
      padding: 16px 32px;
      font-size: 24px;
      border: none;
      border-radius: 12px;
      background: #bb66ff;
      color: black;
      cursor: pointer;
    }
    #animation-container {
      display: none;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }
    #pixel-art {
      width: 200px;
      height: 200px;
      background-image: url('https://i.imgur.com/8QfO7iH.gif'); /* Dans eden gif */
      background-size: contain;
      background-repeat: no-repeat;
    }
  </style>
</head>
<body>
  <button id="trust-btn">Trust me</button>

  <div id="animation-container">
    <div id="pixel-art"></div>
    <audio id="music" autoplay loop>
      <source src="https://www.soundhelix.com/examples/mp3/SoundHelix-Song-1.mp3" type="audio/mpeg">
    </audio>
  </div>

  <script>
    const btn = document.getElementById('trust-btn');
    const container = document.getElementById('animation-container');
    const music = document.getElementById('music');

    btn.addEventListener('click', () => {
      btn.style.display = 'none';
      container.style.display = 'flex';
      music.play();
    });
  </script>
</body>
</html>
