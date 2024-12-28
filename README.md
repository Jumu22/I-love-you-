<!DOCTYPE html>
<html>
<head>
    <title>Jumman's Question</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background: radial-gradient(circle, black, green);
            color: white;
            overflow: hidden;
            position: relative;
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
        .dna {
            position: absolute;
            width: 10px;
            height: 10px;
            background: #00ff00;
            border-radius: 50%;
            animation: move 5s linear infinite;
        }
        @keyframes move {
            0% {
                transform: translate3d(0, 0, 0);
            }
            100% {
                transform: translate3d(100vw, 100vh, 0);
            }
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

        function createDNA() {
            for (let i = 0; i < 50; i++) {
                const dna = document.createElement('div');
                dna.classList.add('dna');
                dna.style.top = Math.random() * 100 + 'vh';
                dna.style.left = Math.random() * 100 + 'vw';
                dna.style.animationDelay = Math.random() * 5 + 's';
                document.body.appendChild(dna);
            }
        }

        createDNA();
    </script>
</body>
</html>