<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>18 Maret 2025</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        body {
            background: linear-gradient(135deg, #ff9a9e, #fad0c4);
            font-family: 'Calibri', cursive, sans-serif;
            display: flex;
            align-items: center;
            justify-content: center;
            min-height: 100vh;
            overflow: hidden;
        }
        .card {
            background: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(10px);
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            padding: 30px;
            max-width: 400px;
            text-align: center;
            position: relative;
            animation: float 4s infinite ease-in-out;
        }
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        .button {
            background: linear-gradient(to right, #ff416c, #ff4b2b);
            color: white;
            padding: 7px 30px;
            border-radius: 30px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            transition: transform 0.3s, box-shadow 0.3s;
            display: inline-block;
        }
        .button:hover {
            transform: scale(1.1) rotate(-2deg);
            box-shadow: 0 8px 20px rgba(255, 71, 126, 0.4);
        }
        .countdown {
            position: absolute;
            top: 10px;
            right: 10px;
            background: #ff416c;
            color: white;
            padding: 8px 14px;
            border-radius: 12px;
            font-size: 16px;
            font-weight: bold;
        }
        .emoji {
            position: absolute;
            font-size: 2em;
            top: -50px;
            animation: fall linear infinite;
        }
        @keyframes fall {
            from { transform: translateY(-50px); opacity: 1; }
            to { transform: translateY(100vh); opacity: 0; }
        }
        .image-container {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }
        .image-container img {
            width: 80%;
            max-width: 180px;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        #notification {
            position: fixed;
            bottom: -100px;
            left: 50%;
            transform: translateX(-50%);
            background: rgba(255, 255, 255, 0.5); /* Warna hitam dengan transparansi 50% */
            color: #ff416c;
            padding: 12px 20px;
            border-radius: 20px;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
            font-weight: bold;
            text-align: center;
            transition: bottom 0.5s ease-in-out;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="countdown">H-1</div>
        <h1 class="text-3xl font-bold text-pink-600">18 Maret 2025!</h1>
        <p class="mt-4 text-gray-700 leading-relaxed">Semangat buat yang mengikuti SNBP! besok adalah hari yang ditunggu-tunggu! Apapun hasilnya stay cool. Semoga kalian semua bisa lulus, dan jika belum, jangan menyerah, masih banyak jalan lain untuk meraihnya. Jangan lupa berdo'a sebelum membuka hasilnya dan tetap semangat para pejuang UTBK! 💪🔥❤️</p>
        <p class="mt-4 text-gray-400 font-medium">by Fathir</p>
        <div class="image-container">
            <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEghSkJGrqswngbHhxRgscmw1I_UJyHcgLEJ0FBPpyxJE7-dyXKOMl8p5iD51DLOaTjib60zfD-9x_Ou2pIT4ouiSbv8ZQseSHs1g77oD6LJ7z3asxMVvuVjDdcKbis46nUoy9o48FG1GTrq3571axCYbE_ONw8i5ialU9WVlYrt3KVca8Eiri6FaiO4wzI/s320/logo-snbp.png" alt="SNBP">
        </div>
        <button class="button mt-6">Keep the Spirit</button>
    </div>
    <div id="notification">🎊 أنتم جميعا رائعون 🎊</div>
    <script>
        function createEmoji() {
            const emojiArray = ['❤️', '🎉', '💖', '💪', '🌟', '🔥', '💕', '❤️‍🔥'];
            const emoji = document.createElement('div');
            emoji.classList.add('emoji');
            emoji.innerText = emojiArray[Math.floor(Math.random() * emojiArray.length)];
            emoji.style.left = Math.random() * window.innerWidth + 'px';
            emoji.style.animationDuration = (Math.random() * 3 + 2) + 's';
            document.body.appendChild(emoji);
            setTimeout(() => emoji.remove(), 5000);
        }
        setInterval(createEmoji, 700);
        document.querySelector('.button').addEventListener('click', () => {
            const notification = document.getElementById('notification');
            notification.style.bottom = '20px';
            setTimeout(() => {
                notification.style.bottom = '-100px';
            }, 3000);
        });
    </script>
</body>
</html>
