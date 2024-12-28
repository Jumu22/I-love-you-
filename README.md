
<html><head>
    <title>Jumman's Question</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background: radial-gradient(circle, black, green);
            color: white;
        }
        h1 {
            color: #00ff00;
            text-shadow: 0 0 10px #00ff00;
        }
        .btn {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            border: none;
            border-radius: 5px;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
            cursor: pointer;
            position: absolute;
        }
        .yes {
            background-color: green;
            color: white;
            left: 50%;
            transform: translateX(-50%);
        }
        .no {
            background-color: gray;
            color: white;
            left: 50%;
            transform: translateX(-50%);
        }
    </style>
</head>
<body>
    <h1>Jumman Tomake Valobashe, Tumi Ki Raji?</h1>
    <button class="btn yes" onclick="alert('Thanks for accept')">Yes</button>
    <button class="btn no" onclick="moveButton()">No</button>

    <script>
        function moveButton() {
            const noButton = document.querySelector('.no');
            const randomX = Math.floor(Math.random() * (window.innerWidth - noButton.clientWidth));
            const randomY = Math.floor(Math.random() * (window.innerHeight - noButton.clientHeight));
            noButton.style.left = randomX + 'px';
            noButton.style.top = randomY + 'px';
        }
    </script>
</body>
</html>