<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-widthб, initial-scale=1.0">
    <title>My Bio</title>
    <style>
         body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
            background: #17212b;
            color: white;
            text-align: center;
            padding: 20px;
            margin: 0;
        }
        button {
            background: #2b5278;
            color: white;
            border: none;
            padding: 12px 24px;
            border-radius: 12px;
            font-size: 16px;
            cursor: pointer;
            margin: 10px;
        }
        .card {
            background: #242f3d;
            border-radius: 16px;
            padding: 20px;
            margin: 20px auto;
            max-width: 400px;
        }
    </style>
    <link rel="stylesheet" href="/css/main.css">
</head>
<body>
<div class="card">
<h1> Hello</h1>
<p>Это мое био!</p>
</div>
<script src="https://telegram.org/js/telegram-web-app.js"></script>
</script>
const tg = window.Telegtam.WebApp;
tg.expand();

const user = tg.initDataUnsafe?.user;
if (user) {
    console.log('Пользователь:', user.first_name);
}
document.getElementById('btn').onclick = () => {
            tg.showAlert('Привет из приложения! 🎉');
        };
    
</body>
</html>
