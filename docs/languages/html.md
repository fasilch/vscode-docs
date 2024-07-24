<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smiley Face Sticker</title>
    <style>
        .smiley {
            position: relative;
            width: 200px;
            height: 200px;
            background: yellow;
            border-radius: 50%;
            border: 5px solid black;
        }
        .smiley::before,
        .smiley::after {
            content: '';
            position: absolute;
            width: 30px;
            height: 30px;
            background: black;
            border-radius: 50%;
            top: 60px;
        }
        .smiley::before {
            left: 50px;
        }
        .smiley::after {
            right: 50px;
        }
        .smiley .mouth {
            position: absolute;
            bottom: 40px;
            left: 50%;
            width: 100px;
            height: 50px;
            border-bottom: 5px solid black;
            border-radius: 0 0 50px 50px;
            transform: translateX(-50%);
        }
    </style>
</head>
<body>
    <div class="smiley">
        <div class="mouth"></div>
    </div>
</body>
</html>
