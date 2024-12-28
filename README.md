<html>
<head>
    <title>Jumman's Question</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
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
        .line {
            position: absolute;
            width: 2px;
            background: #00ff00;
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