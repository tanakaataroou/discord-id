
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Discord ID - imamuraryouta</title>
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      min-height: 100vh;
      display: flex;
      align-items: center;
      justify-content: center;
      background: #232428;
      color: #ffffff;
      font-family: Arial, sans-serif;
    }

    main {
      text-align: center;
      padding: 24px;
    }

    .logo {
      font-size: 64px;
      margin-bottom: 24px;
    }

    .label {
      color: #aeb4c5;
      font-size: 20px;
      margin-bottom: 16px;
    }

    .username {
      font-size: clamp(28px, 7vw, 64px);
      font-weight: 800;
      letter-spacing: -1px;
      cursor: pointer;
      overflow-wrap: anywhere;
      transition: color 0.2s;
    }

    .username:hover {
      color: #7289ff;
    }

    .hint {
      margin-top: 20px;
      color: #9296a3;
      font-size: 14px;
    }

    #message {
      margin-top: 12px;
      color: #8ea1ff;
      font-size: 14px;
    }
  </style>
</head>
<body>
  <main>
    <div class="logo">💬</div>
    <div class="label">Discord ID</div>

    <div class="username" id="username">
      imamuraryouta
    </div>

    <div class="hint">クリックしてIDをコピー</div>
    <div id="message"></div>
  </main>

  <script>
    const username = document.getElementById("username");
    const message = document.getElementById("message");

    username.addEventListener("click", async () => {
      try {
        await navigator.clipboard.writeText("imamuraryouta");
        message.textContent = "コピーしました！";
      } catch {
        message.textContent = "ID：imamuraryouta";
      }
    });
  </script>
</body>
</html>
