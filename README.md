<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>¿Quieres ser mi San Valentín? 💖</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe6f2;
        }
        h1 {
            margin-top: 50px;
        }
        .container {
            margin-top: 50px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            margin: 10px;
            transition: 0.3s;
        }
        .yes {
            background-color: #ff4da6;
            color: white;
        }
        .no {
            background-color: #ccc;
            color: black;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>¿Quieres ser mi San Valentín? 💘</h1>
    <div class="container">
        <button class="yes" onclick="showLove()">Sí 💖</button>
        <button class="no" id="noButton" onmouseover="moveNo()">No 😭</button>
    </div>
    <script>
        function showLove() {
            document.body.innerHTML = '<h1>¡Sabía que dirías que sí! 😍💘</h1>';
        }
        function moveNo() {
            let button = document.getElementById("noButton");
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.left = x + "px";
            button.style.top = y + "px";
        }
    </script>
</body>
</html>
