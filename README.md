<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heart Redirect</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #ffe6e6;
            font-family: Arial, sans-serif;
        }
        .heart {
            position: relative;
            width: 100px;
            height: 100px;
            background-color: red;
            transform: rotate(-45deg);
        }
        .heart:before,
        .heart:after {
            content: '';
            position: absolute;
            width: 100px;
            height: 100px;
            background-color: red;
            border-radius: 50%;
        }
        .heart:before {
            top: -50px;
            left: 0;
        }
        .heart:after {
            top: 0;
            left: 50px;
        }
        p {
            margin-top: 20px;
            text-align: center;
            color: #333;
        }
    </style>
    <script>
        // Chuyển hướng sau 5 giây
        setTimeout(function() {
            window.location.href = "https://example.com"; // Thay link bạn muốn chuyển đến
        }, 5000);
    </script>
</head>
<body>
    <div>
        <div class="heart"></div>
        <p>Chờ một chút... bạn sẽ được chuyển hướng sau 5 giây!</p>
    </div>
</body>
</html>
