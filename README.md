<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>رسالة حب</title>
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f0f0f0;
            margin: 0;
            font-family: Arial, sans-serif;
        }
        #message {
            font-size: 2em;
            font-weight: bold;
            color: #ff0000;
            direction: rtl;
        }
    </style>
</head>
<body>
    <div id="message"></div>

    <script>
        const message = "اميمة رشيد كيبغيك ❤️";
        const messageContainer = document.getElementById('message');
        let index = 0;

        function typeMessage() {
            if (index < message.length) {
                messageContainer.innerHTML += message.charAt(index);
                index++;
                setTimeout(typeMessage, 200); // Adjust the delay to control the typing speed
            }
        }

        // Start typing the message when the page loads
        window.onload = typeMessage;
    </script>
</body>
</html>
