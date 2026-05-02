<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Happy Birthday, My Love!</title>
    <script src="https://cdn.jsdelivr.net/npm/canvas-confetti@1.5.1/dist/confetti.browser.min.js"></script>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #fce4ec 0%, #f8bbd0 100%);
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            text-align: center;
            color: #880e4f;
        }
        .container {
            background: rgba(255, 255, 255, 0.8);
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            max-width: 90%;
            width: 400px;
        }
        h1 { font-size: 2.5rem; margin-bottom: 10px; }
        p { font-size: 1.2rem; line-height: 1.6; }
        .heart { color: #e91e63; font-size: 3rem; margin: 20px 0; }
        button {
            background-color: #e91e63;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1rem;
            border-radius: 50px;
            cursor: pointer;
            transition: transform 0.2s;
            font-weight: bold;
        }
        button:hover { transform: scale(1.05); background-color: #c2185b; }
    </style>
</head>
<body>

<div class="container">
    <div class="heart">❤️</div>
    <h1>Happy Birthday!</h1>
    <p>To my wonderful wife,</p>
    <p>You make every day brighter just by being in it. Here's to another year of adventures together!</p>
    <br>
    <button onclick="celebrate()">Click for a Surprise!</button>
</div>

<script>
    function celebrate() {
        confetti({
            particleCount: 150,
            spread: 70,
            origin: { y: 0.6 },
            colors: ['#ff4081', '#ff80ab', '#ffffff']
        });
    }
</script>

</body>
</html>
