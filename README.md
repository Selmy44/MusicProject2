# MusicProject2
This a music project 2
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Music Platform</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
        }

        .music-player {
            text-align: center;
        }

        #play-btn,
        #pause-btn {
            display: none;
        }
    </style>
</head>

<body>
    <div class="music-player">
        <h1>Music Platform</h1>
        <audio id="audio" controls>
            <source src="your-music-file.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <br>
        <button id="play-btn">Play</button>
        <button id="pause-btn">Pause</button>
    </div>

    <script>
        const audio = document.getElementById("audio");
        const playBtn = document.getElementById("play-btn");
        const pauseBtn = document.getElementById("pause-btn");

        playBtn.addEventListener("click", () => {
            audio.play();
            playBtn.style.display = "none";
            pauseBtn.style
