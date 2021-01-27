# Ride-On-Motion-
#index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ride On</title>
    <link rel="stylesheet" href="style.css">
    <script src="script.js"></script>
</head>
<body>
    <div class = "container">
        <div class = "sky">
            <div class = "trees">
                <div class = "track">
                    <div class = "car">
                        <div class = "wheel1">
                            <img src="PinClipart.com_sports-car-clip-art_5622429 (2).png" alt="">  
                        </div>
                        <div class = "wheel2">
                            <img src="PinClipart.com_sports-car-clip-art_5622429 (1).png" alt="">
                        </div>

                    </div>
                </div>
            </div>

        </div>
    </div>

</body>
</html>

#style.css
*{
    margin:0;
    padding:0;
}
body{
    overflow: hidden;
}
.sky{
    height: 100vh;
    width: 100%;
    background-image: url(3NIEQB3SFVCMNHH6MHZ42FO6PA.jpg);
    background-repeat: no-repeat;
    position: absolute;
}

.trees{
    height: 100vh;
    width: 100%;
    background-image: url(forest-scene-with-trees-field-background_1308-29719.jpg);
    background-size: cover;
    position: absolute;

}

.track{
    height: 60vh;
    width: 800vw;
    background-image: url(start-finish-line-racing-track-marking-car-karting-road-race-rally-vector-background-123249599.jpg);
    background-repeat: repeat-x;
    position: absolute;
    top: 71vh;
    animation: carMove linear 6s infinite;

}

.car{
    height: 100px;
    width: 337px;
    background-image: url(PinClipart.com_sports-car-clip-art_5622429.png);
    background-size: cover;
    background-repeat: repeat-x;
    position: absolute;
    left: 456px;
    bottom: 333px;

}

.wheel1 img{
    width: 79px;
    position: relative;
    top: 32px;
    left: 26px;
    animation: wheelrotation linear .6s infinite;
}

.wheel2 img{
    width: 80px;
    position: relative;
    top: -42px;
    left: 239px;
    animation: wheelrotation linear .6s infinite;
}

@keyframes wheelrotation
{
    100%{
        transform : rotate(360deg);
    }
}

@keyframes carMove
{
    100%{
        transform : translateX(-500vw);
    }
}

#script.js
var audio = document.createElement('audio');
audio.setAttribute('src', 'sound.mp3');
audio.loop = true;
audio.play();
