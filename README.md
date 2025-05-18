<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Happy Birthday Stuti! 🎉❤️</title>
  <link href="https://fonts.googleapis.com/css2?family=Dancing+Script:wght@700&family=Poppins:wght@300;600&display=swap" rel="stylesheet" />
  <style>
    /* Reset */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
    }
    html, body {
      height: 100%;
      background: linear-gradient(135deg, #fceabb, #f8b500);
      font-family: 'Poppins', sans-serif;
      overflow-x: hidden;
      display: flex;
      justify-content: center;
      align-items: center;
      padding: 20px;
      user-select: none;
      position: relative;
    }
    /* Container */
    .container {
      background: rgba(255,255,255,0.95);
      border-radius: 30px;
      box-shadow: 0 15px 40px rgba(0,0,0,0.15);
      max-width: 600px;
      width: 100%;
      padding: 40px 30px 30px;
      text-align: center;
      position: relative;
      z-index: 20;
      overflow: hidden;
    }

    /* Attractive Rainbow Animated Heading with Emojis */
    h1.rainbow-heading {
      font-family: 'Dancing Script', cursive;
      font-weight: 900;
      font-size: 3.8rem;
      text-align: center;
      user-select: none;
      margin-bottom: 0.8em;
      color: #d94f70;
      text-shadow:
        0 0 8px #ff6b81,
        0 0 15px #ff6b81,
        0 0 25px #d94f70;
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 12px;
    }

    h1.rainbow-heading .rainbow-text {
      background: linear-gradient(270deg, #ff6b6b, #f48fb1, #d94f70, #ff6b6b, #f48fb1, #d94f70);
      background-size: 1200% 1200%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: rainbowShift 7s ease infinite;
      display: inline-block;
      padding: 0 6px;
    }

    h1.rainbow-heading .love-name {
      font-size: 4.2rem;
      background: linear-gradient(90deg, #ffb347, #ff6b81, #a18cd1, #fbc2eb, #fad0c4);
      background-size: 200% 200%;
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
      animation: rainbowShift 6s linear infinite;
      padding: 0 6px;
      display: inline-block;
      text-shadow:
        0 0 12px #ffb6c1,
        0 0 22px #f48fb1,
        0 0 32px #d94f70;
    }

    /* Animate emojis with gentle bounce */
    h1.rainbow-heading > :not(.rainbow-text):not(.love-name) {
      font-size: 3.8rem;
      animation: emojiBounce 3s ease-in-out infinite;
      user-select: none;
    }

    h1.rainbow-heading > :not(.rainbow-text):not(.love-name):nth-child(odd) {
      animation-delay: 0s;
    }
    h1.rainbow-heading > :not(.rainbow-text):not(.love-name):nth-child(even) {
      animation-delay: 1.5s;
    }

    @keyframes rainbowShift {
      0% {background-position: 0% 50%;}
      50% {background-position: 100% 50%;}
      100% {background-position: 0% 50%;}
    }

    @keyframes emojiBounce {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    /* Bouncing hearts around heading */
    .heart-bounce {
      position: absolute;
      width: 30px;
      height: 30px;
      background: #d94f70;
      transform: rotate(45deg);
      border-radius: 5px 5px 0 0;
      animation: bounce 2s infinite ease-in-out;
      filter: drop-shadow(0 0 4px #d94f70);
      opacity: 0.85;
      z-index: 21;
    }
    .heart-bounce::before,
    .heart-bounce::after {
      content: "";
      position: absolute;
      width: 30px;
      height: 30px;
      background: #d94f70;
      border-radius: 50%;
      top: 0;
      left: 0;
      filter: drop-shadow(0 0 4px #d94f70);
    }
    .heart-bounce::before {
      top: -15px;
      left: 0;
    }
    .heart-bounce::after {
      top: 0;
      left: 15px;
    }
    @keyframes bounce {
      0%, 100% { transform: translateY(0) rotate(45deg); }
      50% { transform: translateY(-15px) rotate(45deg); }
    }
    /* Position hearts around heading */
    .heart1 { top: -20px; left: -40px; animation-delay: 0s; }
    .heart2 { top: -10px; right: -40px; animation-delay: 0.5s; }
    .heart3 { bottom: -20px; left: 10px; animation-delay: 1s; }
    .heart4 { bottom: -20px; right: 10px; animation-delay: 1.5s; }

    /* Unique carousel section */
    #loveCarousel {
      margin: 24px 0 20px;
      min-height: 60px;
      font-size: 1.25rem;
      color: #d94f70;
      font-weight: 600;
      background: #fff0f6;
      border-radius: 18px;
      box-shadow: 0 0 15px rgba(217,79,112,0.13);
      padding: 18px 30px;
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 12px;
      transition: background 0.3s;
      user-select: text;
      min-width: 220px;
      max-width: 90vw;
      margin-left: auto;
      margin-right: auto;
      letter-spacing: 0.02em;
      position: relative;
      z-index: 2;
    }
    .carousel-emoji {
      font-size: 2rem;
      margin-right: 10px;
      animation: emojiPop 0.6s cubic-bezier(.6,1.6,.6,1) both;
    }
    @keyframes emojiPop {
      0% { transform: scale(0.4) rotate(-30deg); opacity: 0; }
      50% { transform: scale(1.2) rotate(10deg); opacity: 1; }
      100% { transform: scale(1) rotate(0); }
    }

    /* Typing message */
    #typingMessage {
      font-size: 1.15rem;
      color: #6a2c70;
      min-height: 180px;
      margin: 30px 0 20px;
      font-weight: 600;
      white-space: pre-line;
      border-right: 3px solid #d94f70;
      width: 100%;
      margin-left: auto;
      margin-right: auto;
      text-align: left;
      display: none;
      padding: 20px 25px;
      border-radius: 12px;
      background: #fff0f6;
      box-shadow: 0 0 20px rgba(217,79,112,0.4);
      user-select: text;
      line-height: 1.6;
      letter-spacing: 0.02em;
    }

    /* Reveal wishes */
    #wishes {
      font-size: 1.15rem;
      color: #4a2c2a;
      margin-top: 20px;
      white-space: pre-wrap;
      line-height: 1.7;
      display: none;
      text-align: left;
      padding: 25px 30px;
      background: #fff0f6;
      border-radius: 15px;
      box-shadow: 0 10px 40px rgba(217,79,112,0.35);
      user-select: text;
      font-weight: 600;
    }

    /* Button */
    button {
      background: #d94f70;
      color: white;
      border: none;
      border-radius: 50px;
      padding: 15px 40px;
      font-size: 1.2rem;
      font-weight: 600;
      box-shadow: 0 8px 15px rgba(217,79,112,0.4);
      cursor: pointer;
      transition: background 0.3s ease, box-shadow 0.3s ease, transform 0.3s ease;
      margin-top: 1.5em;
      user-select: none;
    }
    button:hover {
      background: #b03a56;
      box-shadow: 0 12px 20px rgba(176,58,86,0.6);
      transform: scale(1.05);
    }

    /* Responsive */
    @media (max-width: 600px) {
      h1.rainbow-heading { font-size: 2.8rem; }
      h1.rainbow-heading .love-name { font-size: 3.2rem; }
      #loveCarousel { font-size: 1.05rem; padding: 14px 12px; }
      #typingMessage { font-size: 1rem; min-height: 160px; }
      #wishes { font-size: 1rem; }
      button { padding: 12px 30px; font-size: 1rem; }
    }
  </style>
</head>
<body>

  <canvas id="confettiCanvas"></canvas>

  <div class="container" role="main" aria-label="Birthday greeting for Stuti">

    <h1 class="rainbow-heading" aria-label="Happy Birthday My Love Stuti! Celebration">
      🎉 <span class="rainbow-text">Happy Birthday</span> 🎂 <span class="love-name">My Love Stuti! ❤️</span> 🎈
      <div class="heart-bounce heart1"></div>
      <div class="heart-bounce heart2"></div>
      <div class="heart-bounce heart3"></div>
      <div class="heart-bounce heart4"></div>
    </h1>

    <!-- Unique carousel section -->
    <div id="loveCarousel" aria-live="polite" aria-atomic="true"></div>

    <div id="typingMessage" aria-live="polite" aria-atomic="true"></div>

    <button id="showWishesBtn" aria-haspopup="true" aria-controls="wishes" aria-expanded="false" style="display:none">Show Your Birthday Wishes 💌</button>

    <div id="wishes" tabindex="0" aria-live="polite" role="region" aria-label="Birthday wishes message"></div>

    <div class="signature">Always your Shwet ❤️</div>
  </div>

  <!-- The rest of your existing scripts remain unchanged -->

  <!-- Carousel Script -->
  <script>
    const carouselItems = [
      {emoji: "🌟", text: "You light up my world every single day."},
      {emoji: "😂", text: "Your laughter is my favorite sound."},
      {emoji: "💖", text: "Your love makes me the happiest person alive."},
      {emoji: "👸", text: "You are my queen, my princess, my everything."},
      {emoji: "🍰", text: "With you, every day is as sweet as cake."},
      {emoji: "🎶", text: "Your voice is the melody to my heart."},
      {emoji: "🦄", text: "You make life magical and full of wonder."},
      {emoji: "🫂", text: "Your hugs are my safe place."},
      {emoji: "✨", text: "You bring sparkle to every moment."},
      {emoji: "💋", text: "Your kisses are my favorite thing in the universe."},
      {emoji: "🥰", text: "You are adorable beyond words."},
      {emoji: "🌈", text: "With you, life is always colorful."},
      {emoji: "🌹", text: "You are as beautiful as a rose."},
      {emoji: "💌", text: "You are my greatest love letter."},
      {emoji: "🧸", text: "Cuddling with you is the best feeling ever."}
    ];
    let carouselIndex = 0;
    const carouselEl = document.getElementById('loveCarousel');
    function showCarouselItem() {
      const item = carouselItems[carouselIndex];
      carouselEl.innerHTML = `<span class="carousel-emoji">${item.emoji}</span> ${item.text}`;
      carouselIndex = (carouselIndex + 1) % carouselItems.length;
    }
    showCarouselItem();
    setInterval(showCarouselItem, 2200);
  </script>

  <!-- Typing animation and other scripts remain unchanged -->

</body>
</html>
