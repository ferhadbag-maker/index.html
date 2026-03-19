<!DOCTYPE html>
<html lang="az">
<head>
    <meta charset="UTF-8">
    <title>Ad günü mübarək</title>

    <!-- Google font -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">

    <!-- Confetti library -->
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.6.0/dist/confetti.browser.min.js"></script>

    <style>
        body {
            margin: 0;
            padding: 0;
            text-align: center;
            font-family: 'Pacifico', cursive;
            background: linear-gradient(270deg, #ff9a9e, #fad0c4, #fad0c4, #ffdde1);
            background-size: 800% 800%;
            animation: gradient 10s ease infinite;
        }

        @keyframes gradient {
            0% {background-position: 0%}
            50% {background-position: 100%}
            100% {background-position: 0%}
        }

        h1 {
            margin-top: 120px;
            font-size: 50px;
            color: white;
            animation: glow 2s infinite alternate;
        }

        @keyframes glow {
            from {text-shadow: 0 0 10px white;}
            to {text-shadow: 0 0 30px #ff4da6;}
        }

        p {
            font-size: 26px;
            color: white;
            margin-top: 20px;
        }

        button {
            margin-top: 40px;
            padding: 15px 30px;
            font-size: 20px;
            border: none;
            border-radius: 30px;
            background: #ff4da6;
            color: white;
            cursor: pointer;
            transition: 0.3s;
        }

        button:hover {
            transform: scale(1.1);
            background: #ff1a8c;
        }

        .heart {
            position: fixed;
            bottom: -10px;
            font-size: 20px;
            animation: floatUp 5s linear infinite;
            color: red;
        }

        @keyframes floatUp {
            0% {transform: translateY(0);}
            100% {transform: translateY(-100vh);}
        }
    </style>
</head>

<body>

    <h1>🎉 Ad günün mübarək 🎉</h1>
    <p>Allah xeyirli, bərəkətli ömür versin əziz Bacım ❤️</p>

    <button onclick="startCelebration()">🎁 Bas buraya</button>

    <!-- Music -->
    <audio id="music" src="https://www.bensound.com/bensound-music/bensound-happyrock.mp3"></audio>

    <script>
        function startCelebration() {
            // Confetti
            confetti({
                particleCount: 200,
                spread: 100
            });

            // Music
            document.getElementById("music").play();

            // Hearts
            for (let i = 0; i < 20; i++) {
                let heart = document.createElement("div");
                heart.className = "heart";
                heart.innerHTML = "❤️";
                heart.style.left = Math.random() * 100 + "vw";
                heart.style.animationDuration = (3 + Math.random() * 2) + "s";
                document.body.appendChild(heart);

                setTimeout(() => heart.remove(), 5000);
            }
        }
    </script>

</body>
</html>
