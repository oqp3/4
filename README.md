    <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>discord.gg/201</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            background: url('https://i.pinimg.com/originals/51/ae/a3/51aea3393b8234a1e69d8713a0a58bc3.gif') no-repeat center center fixed;
            background-size: cover;
            font-family: 'Courier New', Courier, monospace;
            color: #ff0000;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            flex-direction: column;
            text-align: center;
        }
        .image-container img {
            width: 750px; 
            height: auto;
            border: 2px solid #ff0000; 
            border-radius: 15px;
            box-shadow: 0 0 15px rgba(0, 0, 255, 0.7); 
        }
        .info {
            margin-top: 20px;
            font-size: 1.5em;
            color: #ff0000; 
            text-shadow: 0px 0px 8px #ff0000, 0px 0px 15px #ff0000, 0px 0px 25px #ff0000; 
            letter-spacing: 4.5px; 
            white-space: pre-wrap;
        }
        .text {
            margin-top: 20px;
            font-size: 3em; 
            color: #ff1d1d; 
            text-shadow: 0px 0px 8px #ff1212, 0px 0px 15px #fb1111, 0px 0px 25px #ff1111; 
            letter-spacing: 4.5px; 
        }
    </style>
</head>
<body>
    <div class="image-container">
        <img src="https://cdn.discordapp.com/attachments/1429112313935564811/1431735853662605434/copy_C2BC1C60-0F3B-4CC1-A533-7A6F7329306B.gif?ex=68fe7f6b&is=68fd2deb&hm=3bbb3a50cdd823d9779e57ed35e69dd65ec9ad119f444650dfe60d6d83859061&" alt="Discord Image">
    </div>
    <audio autoplay loop>
        <source src="aa.mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>
     <div class="text">تست تست ربو ادارتكم تمم؟</div>
    <div class="info" id="ip-info">
        <strong>IP: <span id="ip"></span></strong><br>
        <span><strong>City:</strong> <span id="city"></span></span><br>
        <span><strong>Region:</strong> <span id="region"></span></span><br>
        <span><strong>Country:</strong> <span id="country"></span></span><br>
        <span><strong>Location:</strong> <span id="loc"></span></span><br>
        <span><strong>Organization:</strong> <span id="org"></span></span><br>
        <span><strong>Timezone:</strong> <span id="timezone"></span></span>
    </div>
    <div class="text">GG : 201 on top  : discord.gg/201</div>

    <script>
         fetch('https://ipinfo.io/json')
        .then(response => response.json())
        .then(data => {
            delete data.readme;
            const infoDiv = document.getElementById('ip-info');
            infoDiv.textContent = JSON.stringify(data, null, 2);
        });
    </script>
</body>
</html>
