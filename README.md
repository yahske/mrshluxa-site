# mrshluxa-site
<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>@mrshluxa — Профиль</title>
  <style>
    @keyframes fadeInUp {
      0% { opacity: 0; transform: translateY(20px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes diagonalGlow {
      0% {
        transform: translate(-100%, -100%) rotate(45deg);
        opacity: 0;
      }
      50% {
        opacity: 1;
      }
      100% {
        transform: translate(200%, 200%) rotate(45deg);
        opacity: 0;
      }
    }

    @keyframes glowPulse {
      0% { filter: brightness(1); }
      50% { filter: brightness(1.15); }
      100% { filter: brightness(1); }
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background: #0f0f0f;
      color: #f5f5f5;
      display: flex;
      justify-content: center;
      align-items: center;
      min-height: 100vh;
      overflow: hidden;
    }

    .background-line {
      position: absolute;
      top: 0;
      left: 0;
      width: 200%;
      height: 4px;
      background: linear-gradient(90deg, transparent, #a64fff, transparent);
      transform: rotate(45deg);
      animation: diagonalGlow 5s linear infinite;
      z-index: 0;
    }

    .card {
      position: relative;
      z-index: 1;
      background: #1a1a1a;
      border-radius: 20px;
      padding: 2rem;
      max-width: 420px;
      text-align: center;
      box-shadow: 0 0 20px rgba(0,0,0,0.5);
      animation: fadeInUp 1.5s ease-out;
    }

    .avatar {
      width: 120px;
      height: 120px;
      border-radius: 50%;
      object-fit: cover;
      border: 3px solid #00aaff;
      margin-bottom: 1rem;
      animation: fadeInUp 1.8s ease-out;
    }

    h1 {
      margin-bottom: 0.5rem;
      font-size: 1.8rem;
    }

    p {
      margin: 0.5rem 0;
      line-height: 1.5;
    }

    .skills {
      margin: 1rem 0;
    }

    .skills span {
      display: inline-block;
      background: #333;
      padding: 0.3rem 0.6rem;
      border-radius: 8px;
      margin: 0.2rem;
      font-size: 0.9rem;
    }

    .buttons {
      margin-top: 2rem;
    }

    .buttons a {
      display: inline-block;
      margin: 0.5rem;
      padding: 0.6rem 1.2rem;
      background: #00aaff;
      color: #fff;
      border-radius: 10px;
      text-decoration: none;
      font-weight: bold;
      transition: background 0.3s, filter 0.2s;
    }

    .buttons a:hover {
      background: #0077cc;
    }

    .buttons a:active {
      filter: brightness(1.2);
    }

    .price-buttons {
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      margin-top: 2rem;
      gap: 0.5rem;
    }

    .price-button {
      flex: 1 1 45%;
      background: #222;
      color: #fff;
      padding: 1rem;
      border-radius: 12px;
      animation: glowPulse 2.5s ease-in-out infinite;
      font-weight: bold;
    }

    .price-button sub {
      display: block;
      font-weight: normal;
      font-size: 0.75rem;
      margin-top: 4px;
      color: #ccc;
    }

    audio {
      display: none;
    }
  </style>
</head>
<body>
  <div class="background-line"></div>
  <div class="card">
    <img class="avatar" src="https://via.placeholder.com/120" alt="Аватар">
    <h1>@mrshluxa</h1>
    <p>📲 Продаю номера на любой вкус | fish |</p>
    <div class="skills">
      <span>Python</span>
      <span>C++</span>
      <span>Rust</span>
    </div>
    <div class="buttons">
      <a href="https://t.me/mrshluxa" target="_blank">Telegram</a>
    </div>
    <div class="price-buttons">
      <div class="price-button">
        Вся Европа
        <sub>есть исключения • от 100₽</sub>
      </div>
      <div class="price-button">
        Вся Азия
        <sub>от 50₽</sub>
      </div>
      <div class="price-button">
        Америка
        <sub>100₽</sub>
      </div>
      <div class="price-button">
        Россия
        <sub>150₽</sub>
      </div>
    </div>
  </div>
  <audio autoplay loop>
    <source src="https://files.catbox.moe/1s2bbm.mp3" type="audio/mpeg">
  </audio>
</body>
</html>


Готово! Теперь:

На фоне играет Home – Resonance.

Внизу четыре кнопки с прайсом, каждая с лёгким анимированным свечением.

Мелкий текст (в скобках) отображается как подпись под основной надписью.


Хочешь добавить переключатель громкости, или чтобы музыка включалась только по клику?

