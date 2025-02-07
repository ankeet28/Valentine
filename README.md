# Valentine
Puntuuu
index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Be My Valentine?</title>
    <style>
        body {
            text-align: center;
            background-color: pink;
            font-family: Arial, sans-serif;
            margin: 50px;
        }
        h1 {
            color: red;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
        }
        .yes {
            background-color: red;
            color: white;
        }
        .no {
            background-color: white;
            color: red;
            position: absolute;
        }
    </style>
    <script>
        function moveNoButton() {
            let x = Math.random() * window.innerWidth;
            let y = Math.random() * window.innerHeight;
            document.getElementById("noButton").style.left = x + "px";
            document.getElementById("noButton").style.top = y + "px";
        }
    </script>
</head>
<body>
    <h1>Will You Be My Valentine? ❤️</h1>
    <div class="buttons">
        <button class="yes" onclick="alert('Yay! I can’t wait! ❤️')">Yes</button>
        <button class="no" id="noButton" onmouseover="moveNoButton()">No</button>
    </div>
</body>
</html>
