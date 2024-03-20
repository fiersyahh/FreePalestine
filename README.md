<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Free Palestine</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f1f1f1;
            margin: 0;
            padding: 0;
        }
        .container {
            margin-top: 50px;
        }
        h1 {
            color: #333;
        }
        .icon {
            width: 100px;
            height: 100px;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Free Palestine</h1>
        <img class="icon" src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/d4/Flag_of_Palestine.svg/1280px-Flag_of_Palestine.svg.png" alt="Palestine Flag">
        <p>Together for justice and peace.</p>
    </div>

    <!-- README.md Content -->
    <div id="readmeContent" style="margin-top: 50px; text-align: left; padding: 20px;"></div>

    <script>
        // Fetching and displaying README content dynamically
        fetch('README.md')
            .then(response => response.text())
            .then(text => {
                document.getElementById('readmeContent').innerHTML = text;
            })
            .catch(error => {
                console.error('Error fetching README.md:', error);
            });
    </script>
</body>
</html>
