[index.html](https://github.com/user-attachments/files/24774075/index.html)
<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Te amo bb 💙</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: "Poppins", "Arial", sans-serif;
    }

    body {
      background: linear-gradient(135deg, #e6f0ff, #f7fbff);
      height: 100vh;
      overflow: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .container {
      background: #ffffff;
      padding: 30px 26px;
      border-radius: 26px;
      text-align: center;
      box-shadow: 0 12px 40px rgba(0, 82, 204, 0.25);
      width: 90%;
      max-width: 360px;
      animation: pop 0.9s ease;
      position: relative;
      border: 2px solid #dbe9ff;
    }

    @keyframes pop {
      0% {
        transform: scale(0.6);
        opacity: 0;
      }
      100% {
        transform: scale(1);
        opacity: 1;
      }
    }

    h1 {
      color: #1f4fd8;
      font-size: 1.7rem;
      margin-bottom: 12px;
      animation: float 2s ease-in-out infinite;
    }

    @keyframes float {
      0%, 100% {
        transform: translateY(0);
      }
      50% {
        transform: translateY(-6px);
      }
    }

    p {
      font-size: 1rem;
      margin-bottom: 20px;
      color: #4a5f91;
    }

    .buttons {
      position: relative;
      height: 120px;
      display: flex;
      justify-content: center;
      align-items: center;
      flex-wrap: wrap;
      gap: 14px;
    }

    button {
      padding: 12px 32px;
      font-size: 1rem;
      border: none;
      border-radius: 999px;
      cursor: pointer;
      transition: all 0.25s ease;
      font-weight: 600;
    }

    button:hover {
      transform: scale(1.08);
    }

    #yes {
      background: linear-gradient(135deg, #1f4fd8, #5fa8ff);
      color: white;
      animation: pulse 1.6s infinite;
    }

    @keyframes pulse {
      0% {
        transform: scale(1);
        box-shadow: 0 0 0 0 rgba(31, 79, 216, 0.6);
      }
      70% {
        transform: scale(1.08);
        box-shadow: 0 0 0 20px rgba(31, 79, 216, 0);
      }
      100% {
        transform: scale(1);
      }
    }

    #no {
      background-color: #e3edff;
      color: #1f4fd8;
      position: absolute;
    }

    .extra-yes {
      background: linear-gradient(135deg, #1f4fd8, #5fa8ff);
      color: white;
      animation: floatIn 0.4s ease;
    }

    @keyframes floatIn {
      from {
        opacity: 0;
        transform: translateY(14px);
      }
      to {
        opacity: 1;
        transform: translateY(0);
      }
    }

    .result {
      margin-top: 22px;
      font-size: 1.4rem;
      color: #1f4fd8;
      display: none;
      animation: fadeIn 1s ease forwards;
      font-weight: 600;
    }

    .roblox-message {
      margin-top: 14px;
      font-size: 1.1rem;
      color: #2d3f73;
      display: none;
      font-weight: 500;
      animation: fadeIn 1s ease forwards;
    }

    .roblox-image {
      width: 100%;
      max-width: 230px;
      border-radius: 18px;
      margin: 14px auto 0 auto;
      display: none;
      animation: imageFloatIn 1s ease forwards;
      border: 2px solid #dbe9ff;
    }

    @keyframes imageFloatIn {
      from {
        opacity: 0;
        transform: translateY(12px) scale(0.95);
      }
      to {
        opacity: 1;
        transform: translateY(0) scale(1);
      }
    }

    @keyframes fadeIn {
      from {
        opacity: 0;
      }
      to {
        opacity: 1;
      }
    }

    .heart {
      position: absolute;
      bottom: -20px;
      font-size: 20px;
      animation: floatUp 6s linear infinite;
      opacity: 0.9;
      pointer-events: none;
      color: #5fa8ff;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(0) scale(1);
        opacity: 0;
      }
      10% {
        opacity: 1;
      }
      100% {
        transform: translateY(-110vh) scale(1.5);
        opacity: 0;
      }
    }

    .tap-hint {
      position: absolute;
      bottom: 10px;
      width: 100%;
      text-align: center;
      font-size: 0.75rem;
      color: #5fa8ff;
      opacity: 0.6;
    }

    /* 🎵 Botão de música */
    .music-control {
      position: fixed;
      bottom: 20px;
      right: 20px;
      width: 52px;
      height: 52px;
      border-radius: 50%;
      border: none;
      background: linear-gradient(135deg, #1f4fd8, #5fa8ff);
      color: white;
      font-size: 22px;
      cursor: pointer;
      box-shadow: 0 8px 20px rgba(31, 79, 216, 0.4);
      display: flex;
      align-items: center;
      justify-content: center;
      transition: transform 0.2s ease;
      z-index: 999;
    }

    .music-control:hover {
      transform: scale(1.1);
    }
  </style>
</head>
<body>
  <div class="container" onclick="startMusic()">
    <h1>Você me ama de verdade?? 💙</h1>
    <p>Pois eu te amo muito!!!!!!</p>

    <div class="buttons" id="buttonsArea">
      <button id="yes">Sim 💙</button>
      <button id="no">Não</button>
    </div>

    <div class="result" id="result">
      AAAAA 😍💍  
      <br />
      Eu te amo, Rychard! 💙
      <p><small> finge que não foi forçado, rs</small></p>
    </div>

    <div class="roblox-message" id="robloxMessage">
      agora vamos jogar roblox.
    </div>

    <img src="baixados (18).jpg" alt="Roblox" class="roblox-image" id="robloxImage" />

    <div class="tap-hint">Toque na tela 💙</div>
  </div>

  <!-- 🎵 Botão de música -->
  <button class="music-control" id="musicBtn">▶</button>

  <audio id="bgMusic" loop>
    <source src="New_West_-_Those_Eyes_CeeNaija.com_.mp3" type="audio/mpeg" />
    Seu navegador não suporta áudio.
  </audio>

  <script>
    const noButton = document.getElementById("no");
    const yesButton = document.getElementById("yes");
    const result = document.getElementById("result");
    const buttonsArea = document.getElementById("buttonsArea");
    const music = document.getElementById("bgMusic");
    const robloxMessage = document.getElementById("robloxMessage");
    const robloxImage = document.getElementById("robloxImage");
    const musicBtn = document.getElementById("musicBtn");

    let heartsStarted = false;

    function startMusic() {
      if (!music.paused) return;
      music.volume = 0;
      music.play().then(() => {
        musicBtn.textContent = "⏸";
        const fade = setInterval(() => {
          if (music.volume < 1) {
            music.volume = Math.min(music.volume + 0.05, 1);
          } else {
            clearInterval(fade);
          }
        }, 200);
      }).catch(() => {});
    }

    function toggleMusic() {
      if (music.paused) {
        startMusic();
      } else {
        music.pause();
        musicBtn.textContent = "▶";
      }
    }

    musicBtn.addEventListener("click", toggleMusic);

    noButton.addEventListener("touchstart", moveNoButton);
    noButton.addEventListener("mouseover", moveNoButton);
    noButton.addEventListener("click", moveNoButton);

    function moveNoButton() {
      const areaWidth = buttonsArea.offsetWidth;
      const areaHeight = buttonsArea.offsetHeight;

      const randomX = Math.random() * (areaWidth - noButton.offsetWidth);
      const randomY = Math.random() * (areaHeight - noButton.offsetHeight);

      noButton.style.left = randomX + "px";
      noButton.style.top = randomY + "px";

      createExtraYes();
    }

    function createExtraYes() {
      const extraYes = document.createElement("button");
      extraYes.textContent = "Sim 💙";
      extraYes.classList.add("extra-yes");
      extraYes.addEventListener("click", showResult);
      buttonsArea.appendChild(extraYes);
    }

    yesButton.addEventListener("click", showResult);

    function showResult() {
      result.style.display = "block";
      buttonsArea.style.display = "none";
      robloxMessage.style.display = "block";
      robloxImage.style.display = "block";
      startMusic();
      if (!heartsStarted) startHearts();
    }

    function startHearts() {
      heartsStarted = true;
      setInterval(() => {
        const heart = document.createElement("div");
        heart.classList.add("heart");
        heart.textContent = "💙";
        heart.style.left = Math.random() * 100 + "vw";
        heart.style.animationDuration = 4 + Math.random() * 3 + "s";
        document.body.appendChild(heart);

        setTimeout(() => {
          heart.remove();
        }, 7000);
      }, 300);
    }

    // Começa os corações desde o início
    startHearts();
  </script>
</body>
</html>
[New_West_-_Those_Eyes_CeeNaija.com_.mp3](https://github.com/user-attachments/files/24774080/New_West_-_Those_Eyes_CeeNaija.com_.mp3)
![baixados (18)](https://github.com/user-attachments/assets/a8482b48-8361-49b2-a2ed-6ab204f26476)
