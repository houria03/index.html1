<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Projet PFE Drone</title>

<style>
body {
    margin: 0;
    font-family: Arial;
    background: #f5f6fa;
}

/* ===== HEADER ===== */
header {
    background: linear-gradient(135deg, #1a2a6c, #2a4099);
    color: white;
    text-align: center;
    padding: 40px;
}

/* ===== SLIDER ===== */
.slider {
    position: relative;
    width: 90%;
    max-width: 1000px;
    margin: 20px auto;
    overflow: hidden;
    border-radius: 12px;
}

.slides {
    display: flex;
    transition: transform 0.5s ease-in-out;
}

.slide {
    min-width: 100%;
}

.slide img {
    width: 100%;
    height: 400px;
    object-fit: cover;
}

/* Buttons */
.prev, .next {
    position: absolute;
    top: 50%;
    transform: translateY(-50%);
    background: rgba(0,0,0,0.5);
    color: white;
    border: none;
    padding: 10px 15px;
    cursor: pointer;
    font-size: 22px;
}

.prev { left: 10px; }
.next { right: 10px; }

.prev:hover, .next:hover {
    background: rgba(0,0,0,0.8);
}

/* ===== CONTENT ===== */
.container {
    width: 90%;
    max-width: 1000px;
    margin: auto;
    background: white;
    padding: 20px;
    border-radius: 10px;
}
</style>
</head>

<body>

<header>
    <h1>Projet Drone Intelligent</h1>
</header>

<!-- ⭐ SLIDER -->
<div class="slider">

    <div class="slides" id="slides">

        <div class="slide">
            <img src="images/photo1.jpg" alt="">
        </div>

        <div class="slide">
            <img src="images/photo2.jpg" alt="">
        </div>

        <div class="slide">
            <img src="images/photo3.jpg" alt="">
        </div>

    </div>

    <button class="prev" onclick="prevSlide()">❮</button>
    <button class="next" onclick="nextSlide()">❯</button>

</div>

<!-- CONTENT -->
<div class="container">
    <h2>Description du projet</h2>
    <p>Projet drone intelligent pour détection des incidents.</p>
</div>

<script>
let index = 0;
const slides = document.getElementById("slides");
const total = slides.children.length;

function showSlide() {
    slides.style.transform = "translateX(" + (-index * 100) + "%)";
}

function nextSlide() {
    index++;
    if (index >= total) index = 0;
    showSlide();
}

function prevSlide() {
    index--;
    if (index < 0) index = total - 1;
    showSlide();
}

/* Auto slide */
setInterval(() => {
    nextSlide();
}, 3000);
</script>

</body>
</html>
