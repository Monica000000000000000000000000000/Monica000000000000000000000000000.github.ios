<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Documents</title>

    <style>
body {
    height: 100%;
    margin: 1px;
    padding: 0;
    box-sizing: border-box;
}


.ShipPhoto {
    background: linear-gradient(rgba(0, 0, 0, 0.856), rgba(0, 0, 0, 0.856)), url(https://preview.redd.it/4k-wallpaper-steampunk-pirate-ship-v0-8nq76z9pm0sa1.jpg?width=3840&format=pjpg&auto=webp&s=176b4467e66e11c0ec07bc8d6e00c24c43b1447d);
    background-size: cover;
    background-attachment: fixed;
    background-position: center;
    height: 2000px;
    width: auto;
}

:root {
    --purple: #8e44ad;
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    font-size: 62.5%;
}

.container .heading {
    font-size: 3rem;
    margin: 2px 0;
    text-transform: capitalize;
    color: var(--purple);
    font-family: Verdana, Geneva, Tahoma, sans-serif;
    letter-spacing: .2rem;
    text-align: center;
    text-shadow: 0 .3rem .5rem rgba(0, 0, 0, 0.5);
}

.video-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}

.video-container .video {
    height: 400px;
    width: 600px;
    margin: 2rem;
    box-sizing: 0 .5rem 1rem rgba(0, 0, 0, 0.5);
    box-shadow: 0 0.5rem 1rem rgba(0, 0, 0, 0.5);
    overflow: hidden;
    border-radius: 1rem;
}

.video-container .video video {
    height: 407px;
    width: 610px;
    object-fit: cover;
    outline: none;
    border: none;
    cursor: pointer;
    border: 3px solid rgb(231, 231, 231); /* Add a white border around the paragraph */
    background-color: rgb(231, 231, 231); /* Set the background color to white */
}

.video-container .video video:hover {
    transition: .2s linear;
    transform: scale(1.3);
}

.video-container .video .active {
    position: fixed;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    height: 80%;
    width: 80%;
    box-shadow: 0 0 0 100vh rgba(0, 0, 0, .7);
    z-index: 1;
}

.video-container .video .active:hover {
    transition: none;
    transform: translate(-50%, -50%) scale(1);
}

hr {
    border-color: black; /* Set the color of the horizontal rule (hr) to black */
}

.wrapper {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center; /* Center vertically */
    height: 10vh; /* Make the container full height of the viewport */
}

.img-eye {
    width: 272px;
    height: 372px;
    margin: 10px;
    border-radius: 20px;
    border: 1px solid rgb(231, 231, 231); /* Add a white border around the paragraph */
    background-color: rgb(231, 231, 231); /* Set the background color to white */
}
.ai{
    width: 343px;
    height: 400px;
    margin: 10px;
    border-radius: 20px;
    border: 1px solid rgb(231, 231, 231); /* Add a white border around the paragraph */
    background-color: rgb(231, 231, 231); /* Set the background color to white */
    transition: transform 0.3s ease-in-out;
}

.img-eyee {
    width: 311px;
    height: 240px;
    margin: 10px;
    border-radius: 20px;
    border: 1px solid rgb(231, 231, 231); /* Add a white border around the paragraph */
    background-color: rgb(231, 231, 231); /* Set the background color to white */
}

.img-eye{
    width: 343px;
    height: 386px;
    margin: 10px;
    border-radius: 20px;
    transition: transform 0.3s ease-in-out;
}
.img-eyee {
    width: 380px;
    height: 310px;
    margin: 9px;
    border-radius: 20px;
    transition: transform 0.3s ease-in-out;
}

/* Apply the scale transform on hover */
.img-eye:hover,
.img-eyee:hover {
    transform: scale(1.5); /* Adjust the scale factor as needed */
    cursor: pointer;
    position: relative;
}
.ai:hover {
    transform: scale(1.5); /* Adjust the scale factor as needed */
    cursor: pointer;
    position: relative;
}
    </style>

</head>
<body>
    <div class="ShipPhoto">
        <div class="container">
            <div class="heading">Videos</div>
            <div class="video-container">
                <div class="video">
                    <video controls src="f:\0\0 ALA\0926.mp4"></video>
                </div>
                <div class="video">
                    <video controls src="f:\0\0 ALA\VideoEditing.mp4"></video>
                </div>
            </div>
        </div>

<hr>
<br>
<hr>
    <br>
    <hr>
    <br>
    <hr>
<br>
<hr>
    <br>
    <hr>
    <br>

    <div class="wrapper">
        <img class="ai" src="f:\0\0 ALA\20231003_021258.jpg" onclick="toggleImageSize(this)">
        <img class="ai" src="f:\0\0 ALA\20231003_021403.jpg" onclick="toggleImageSize(this)">
        <img class="ai" src="f:\0\0 ALA\20231003_021437.jpg" onclick="toggleImageSize(this)">
        <img class="img-eye" src="f:\0\0 ALA\Monica_Gypsum_shapes_to_color_for_children.jpg" onclick="toggleImageSize(this)">
        <img class="img-eyee" src="f:\0\0 ALA\Monica Karate.JPG" onclick="toggleImageSize(this)">
        <img class="img-eyee" src="f:\0\0 ALA\Monica Scouts.JPG" onclick="toggleImageSize(this)">
        <img class="img-eyee" src="f:\0\0 ALA\Monica Scouts2.JPG" onclick="toggleImageSize(this)">
        <img class="img-eyee" src="f:\0\0 ALA\Monica Scouts3.JPG" onclick="toggleImageSize(this)">
    </div>

    <div id="enlarged-image" class="enlarged-image-container">
        <img id="enlarged-img" class="enlarged-img" src="">
        <span class="close-button" onclick="closeImage()">&times;</span>
    </div>

<script>
    document.addEventListener('DOMContentLoaded', function () {
        var images = document.querySelectorAll('.img-eye, .img-eyee');

        function toggleImageSize(image) {
            images.forEach(function (otherImage) {
                if (otherImage !== image) {
                    otherImage.style.opacity = '0.5';
                    otherImage.style.pointerEvents = 'none';
                }
            });

            image.classList.toggle('img-enlarged');

            image.addEventListener('click', function () {
                images.forEach(function (otherImage) {
                    otherImage.style.opacity = '1';
                    otherImage.style.pointerEvents = 'auto';
                });
            });
        }


        images.forEach(function (image) {
            image.addEventListener('click', function () {
                toggleImageSize(image);
            });
        });
    });
</script>

<script>    function toggleImageSizeOnHover(image) {
    image.addEventListener('mouseover', function() {
        image.classList.add('img-enlarged');
    });

    image.addEventListener('mouseout', function() {
        image.classList.remove('img-enlarged');
    });
}
</script>

</div>
</body>
</html>
