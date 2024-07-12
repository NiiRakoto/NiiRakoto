<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Page de GitHub Customisée</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background: linear-gradient(135deg, #71b7e6, #9b59b6);
            overflow: hidden;
        }
        h1 {
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
            font-size: 3em;
            position: relative;
            animation: textAnimation 5s infinite;
        }
        @keyframes textAnimation {
            0% { transform: scale(1); }
            50% { transform: scale(1.2); }
            100% { transform: scale(1); }
        }
        .circle {
            position: absolute;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.2);
            animation: circleAnimation 10s infinite;
        }
        @keyframes circleAnimation {
            0% {
                transform: scale(0);
                opacity: 1;
            }
            50% {
                opacity: 0.5;
            }
            100% {
                transform: scale(1);
                opacity: 0;
            }
        }
    </style>
</head>
<body>
    <h1>Bienvenue sur mon GitHub!</h1>

    <script>
        const createCircle = () => {
            const circle = document.createElement('div');
            circle.classList.add('circle');
            const size = Math.random() * 50 + 50;
            circle.style.width = `${size}px`;
            circle.style.height = `${size}px`;
            circle.style.left = `${Math.random() * 100}vw`;
            circle.style.top = `${Math.random() * 100}vh`;
            circle.style.animationDuration = `${Math.random() * 5 + 5}s`;
            document.body.appendChild(circle);
            setTimeout(() => {
                circle.remove();
            }, 10000);
        };

        setInterval(createCircle, 500);
    </script>
</body>
</html>

<!--
**NiiRakoto/NiiRakoto** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
