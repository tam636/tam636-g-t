<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Tặng ebe của anh</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      overflow: hidden;
      font-family: 'Segoe UI', sans-serif;
      background-color: #ffe6f0;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      position: relative;
    }

    .heart {
      width: 100px;
      height: 90px;
      background: red;
      position: relative;
      transform: rotate(-45deg);
      animation: beat 1s infinite;
      z-index: 2;
    }

    .heart::before,
    .heart::after {
      content: "";
      width: 100px;
      height: 90px;
      background: red;
      border-radius: 50%;
      position: absolute;
    }

    .heart::before {
      top: -50px;
      left: 0;
    }

    .heart::after {
      left: 50px;
      top: 0;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1) rotate(-45deg); }
      50% { transform: scale(1.2) rotate(-45deg); }
    }

    .text {
      margin-top: 30px;
      font-size: 24px;
      color: #d63384;
      font-weight: bold;
      z-index: 2;
    }

    .floating-huong {
      position: absolute;
      bottom: -50px;
      font-size: 30px;
      color: rgba(255, 105, 180, 0.2);
      animation: floatUp linear infinite;
      z-index: 0;
      pointer-events: none;
      white-space: nowrap;
    }

    @keyframes floatUp {
      0% {
        transform: translateY(100vh);
        opacity: 0;
      }
      30% {
        opacity: 1;
      }
      100% {
        transform: translateY(-150vh);
        opacity: 0;
      }
    }
  </style>
</head>
<body>
  <!-- Trái tim và chữ chính -->
  <div class="heart"></div>
  <div class="text">Tặng ebe của anh 💝</div>

  <!-- Tạo nhiều chữ Hương bay khắp nền -->
  <script>
    const colors = ['rgba(255,105,180,0.2)', 'rgba(255,105,180,0.3)', 'rgba(255,182,193,0.25)'];
    for (let i = 0; i < 40; i++) {
      const span = document.createElement('div');
      span.className = 'floating-huong';
      span.innerText = 'Hương 💗 Hương 💗';
      span.style.left = Math.random() * 100 + 'vw';
      span.style.animationDuration = (5 + Math.random() * 10) + 's';
      span.style.animationDelay = (Math.random() * 10) + 's';
      span.style.fontSize = (20 + Math.random() * 20) + 'px';
      span.style.color = colors[Math.floor(Math.random() * colors.length)];
      document.body.appendChild(span);
    }
  </script>
</body>
</html>
