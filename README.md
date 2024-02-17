<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Sign-In</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        form {
            width: 300px;
            padding: 20px;
            border: 1px solid #ccc;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            background-color: white;
        }
        label {
            display: block;
            margin-top: 10px;
        }
        input[type="email"],
        input[type="password"] {
            width: 100%;
            padding: 8px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 4px;
            box-sizing: border-box;
        }
        input[type="submit"] {
            width: 100%;
            padding: 8px;
            margin-top: 10px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        input[type="submit"]:hover {
            background-color: #45a049;
        }
        .options {
            margin-top: 10px;
        }
        .options label {
            display: inline-block;
            margin-right: 10px;
        }
        .options input[type="radio"] {
            margin-top: 2px;
        }
    </style>
</head>
<body>
    



<div class="options">
    <label for="poor">Be poor</label>
    <input type="radio" id="poor" name="status" value="poor">

    <label for="rich">Be rich</label>
    <input type="radio" id="rich" name="status" value="rich">
</div>

<script>
    const radioButtons = document.querySelectorAll('input[name="status"]');

    radioButtons.forEach((button) => {
        button.addEventListener("change", (event) => {
            if (event.target.value === "rich") {
                window.open("https://www.tesla.com/", "_blank");
            } else if (event.target.value === "poor") {
                window.open("https://www.roblox.com/", "_blank");
            }
        });
    });
</script>
</body>
</html>
