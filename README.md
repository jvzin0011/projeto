<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Relógio Digital - João Vitor Gonçalves</title>
  <style>
    body {
      background-color: #121212;
      color: #fff;
      font-family: Arial, sans-serif;
      text-align: center;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #1f1f1f;
      padding: 20px;
    }

    h1 {
      margin: 0;
      color: #0f0;
    }

    .clock {
      font-size: 5rem;
      color: #0f0;
      background-color: #000;
      border: 2px solid #0f0;
      border-radius: 10px;
      padding: 20px 50px;
      display: inline-block;
      margin-top: 40px;
      box-shadow: 0 0 20px #0f0;
    }

    footer {
      margin-top: 60px;
      padding: 20px;
      background-color: #1f1f1f;
      font-size: 0.9rem;
      color: #aaa;
    }

    a {
      color: #0f0;
      text-decoration: none;
    }

    a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>

  <header>
    <h1>Relógio Digital</h1>
    <p>Feito por João Vitor Gonçalves - Ciência da Computação</p>
  </header>

  <div class="clock" id="clock">00:00:00</div>

  <footer>
    <p>Email: <a href="mailto:joaovitornascimentop3534@gmail.com">joaovitornascimentop3534@gmail.com</a></p>
    <p>GitHub: <a href="https://github.com/jvzinn0011" target="_blank">github.com/jvzinn0011</a></p>
  </footer>

  <script>
    function updateClock() {
      const now = new Date();
      const h = String(now.getHours()).padStart(2, '0');
      const m = String(now.getMinutes()).padStart(2, '0');
      const s = String(now.getSeconds()).padStart(2, '0');
      document.getElementById('clock').textContent = `${h}:${m}:${s}`;
    }

    setInterval(updateClock, 1000);
    updateClock();
  </script>

</body>
</html>
