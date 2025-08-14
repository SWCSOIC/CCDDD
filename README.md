<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hello Buggu ji</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f9f9f9;
            margin: 0;
            padding: 50px;
        }
        h1 {
            color: #333;
            margin-bottom: 40px;
        }
        .phone-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
        }
        .call-button {
            background-color: #28a745;
            color: white;
            border: none;
            border-radius: 50%;
            width: 120px;
            height: 120px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 50px;
            cursor: pointer;
            text-decoration: none;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
            transition: background-color 0.2s, transform 0.1s;
        }
        .call-button:hover {
            background-color: #218838;
            transform: scale(1.05);
        }
        p {
            font-size: 18px;
            color: #555;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <h1>Hello Buggu ji</h1>
    <div class="phone-container">
        <a href="tel:+911234567890" class="call-button">📞</a>
        <p>Tap to call me</p>
    </div>
</body>
</html>
