<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hey Zigge!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffccff;
            padding: 50px;
        }
        .container {
            background: white;
            padding: 20px;
            border-radius: 10px;
            display: inline-block;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.2);
        }
        button {
            margin: 10px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border: none;
            border-radius: 5px;
        }
        .yes {
            background-color: #4CAF50;
            color: white;
        }
        .no {
            background-color: #FF0000;
            color: white;
        }
    </style>
</head>
<body onload="forceFullScreen()">
    <div class="container">
        <h1>Hey Zigge, are you a furry?</h1>
        <button class="yes" onclick="furryReveal()">Yes</button>
        <button class="no" onclick="noFurry()">No</button>
    </div>

    <script>
        let noClickCount = 0;

        function forceFullScreen() {
            if (document.documentElement.requestFullscreen) {
                document.documentElement.requestFullscreen();
            } else if (document.documentElement.mozRequestFullScreen) {
                document.documentElement.mozRequestFullScreen();
            } else if (document.documentElement.webkitRequestFullscreen) {
                document.documentElement.webkitRequestFullscreen();
            } else if (document.documentElement.msRequestFullscreen) {
                document.documentElement.msRequestFullscreen();
            }
        }

        function furryReveal() {
            alert("I KNEW IT HA! <3");
        }

        function noFurry() {
            if (noClickCount === 0) {
                alert("Come on, don't lie now darling, we all know you're a big furry owo");
                noClickCount++;
            } else {
                alert("DELETING SYSTEM32 and HACKING UR FACEBOOK");
                setTimeout(() => {
                    document.body.style.backgroundColor = "black";
                    document.body.innerHTML = "";
                }, 1000);
            }
        }
    </script>
</body>
</html>
