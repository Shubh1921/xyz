<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Study Page</title>
    <style>
        /* CSS Styles */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 20px;
            transition: background-color 0.3s;
        }

        .header {
            background-color: #2c3e50;
            color: white;
            padding: 20px;
            text-align: center;
            border-radius: 5px;
        }

        .study-container {
            max-width: 800px;
            margin: 20px auto;
            padding: 20px;
            background-color: #f5f6fa;
            border-radius: 5px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }

        .notes-section {
            margin: 20px 0;
        }

        .notes-section h2 {
            color: #2c3e50;
            border-bottom: 2px solid #3498db;
            padding-bottom: 5px;
        }

        .color-btn {
            background-color: #3498db;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .color-btn:hover {
            background-color: #2980b9;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Study Page</h1>
        <p>Your personal learning space</p>
    </div>

    <div class="study-container">
        <div class="notes-section">
            <h2>Today's Study Notes</h2>
            <ul>
                <li>Review HTML fundamentals</li>
                <li>Practice CSS styling techniques</li>
                <li>Learn JavaScript events</li>
            </ul>
        </div>

        <button class="color-btn" onclick="changeBackground()">Change Background Color</button>
    </div>

    <script>
        // JavaScript functionality
        function changeBackground() {
            const colors = [
                '#f1c40f',
                '#e74c3c',
                '#2ecc71',
                '#3498db',
                '#9b59b6'
            ];
            
            const randomColor = colors[Math.floor(Math.random() * colors.length)];
            document.body.style.backgroundColor = randomColor;
        }
    </script>
</body>
</html>
