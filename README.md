<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projet de Fin d'Études | Houria & Rachida Mourad</title>

    <style>
        :root {
            --primary-color: #1a2a6c;
            --secondary-color: #b21f1f;
            --accent-color: #fdbb2d;
            --bg-color: #f8f9fa;
            --text-color: #333;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background-color: var(--bg-color);
            margin: 0;
            padding: 0;
            line-height: 1.6;
            color: var(--text-color);
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), #2a4099);
            color: white;
            text-align: center;
            padding: 60px 20px;
        }

        .logo-univ {
            width: 130px;
            background: white;
            padding: 10px;
            border-radius: 50%;
            margin-bottom: 20px;
        }

        .container {
            max-width: 1000px;
            margin: -40px auto 40px;
            background: white;
            padding: 40px;
            border-radius: 15px;
        }

        h2 {
            color: var(--primary-color);
            border-bottom: 2px solid var(--secondary-color);
            padding-bottom: 10px;
            margin-top: 40px;
            text-transform: uppercase;
        }

        .info-grid {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 10px;
            background: #f1f3f5;
            padding: 20px;
            border-radius: 10px;
        }

        .info-item {
            font-weight: bold;
            color: var(--primary-color);
        }

        .description-box {
            background: #fff;
            padding: 20px;
            border-right: 5px solid var(--accent-color);
            direction: rtl;
            text-align: right;
        }

        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 15px;
        }

        .gallery-item {
            background: white;
            border-radius: 10px;
            overflow: hidden;
        }

        .gallery-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .gallery-caption {
            text-align: center;
            padding: 10px;
            font-weight: bold;
        }

        .tech-list {
            list-style: none;
            padding: 0;
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
        }

        .tech-tag {
            background: #e9ecef;
            padding: 8px 12px;
            border-radius: 20px;
        }

        .footer {
            text-align: center;
            padding: 20px;
            background: #eee;
            margin-top: 40px;
        }
    </style>
</head>

<body>

<header>
    <img src="https://upload.wikimedia.org/wikipedia/dz/4/45/Logo_University_of_Mascara.png" class="logo-univ">
    <h1>Université Mustapha Stambouli de Mascara</h1>
    <p>Département d'Électrotechnique</p>
</header>

<div class="container">

    <h2>Fiche Technique</h2>
    <div class="info-grid">
        <div class="info-item">Titre :</div>
        <div>Système Intelligent de Détection d’Incidents sur Drone</div>

        <div class="info-item">Réalisé par :</div>
        <div>Houria Mourad & Rachida Mourad</div>

        <div class="info-item">Niveau :</div>
        <div>2ème Année Électronique</div>

        <div class="info-item">Encadré par :</div>
        <div>Mourad Hebali</div>

        <div class="info-item">Année :</div>
        <div>2026 - 2027</div>
    </div>

    <h2>Description</h2>
    <div class="description-box">
        هذا المشروع يهدف إلى تصميم نظام ذكي يعتمد على حساسات مثبتة على درون للكشف عن الحرائق وتسرب الغاز والكوارث الطبيعية.
    </div>

    <h2>Galerie</h2>
    <div class="gallery">

        <div class="gallery-item">
            <img src="photo1.jpg">
            <div class="gallery-caption">Drone Finalisé</div>
        </div>

        <div class="gallery-item">
            <img src="photo2.jpg">
            <div class="gallery-caption">Schéma Électronique</div>
        </div>

        <div class="gallery-item">
            <img src="photo3.jpg">
            <div class="gallery-caption">Tests des capteurs</div>
        </div>

    </div>

    <h2>Technologies</h2>
    <ul class="tech-list">
        <li class="tech-tag">ESP32-S3</li>
        <li class="tech-tag">Arduino Uno</li>
        <li class="tech-tag">ESP32-CAM</li>
        <li class="tech-tag">MQ2</li>
        <li class="tech-tag">DHT22</li>
        <li class="tech-tag">Capteur de pluie</li>
        <li class="tech-tag">Capteur d’eau</li>
        <li class="tech-tag">Buzzer</li>
        <li class="tech-tag">Capteur de flamme</li>
        <li class="tech-tag">LCD</li>
        <li class="tech-tag">OLED</li>
        <li class="tech-tag">LED</li>
        <li class="tech-tag">GPS</li>
        <li class="tech-tag">SIM900</li>
        <li class="tech-tag">Servo moteur</li>
        <li class="tech-tag">BMP180</li>
        <li class="tech-tag">ESP8266</li>
        <li class="tech-tag">Capteur vibration</li>
    </ul>

</div>

<div class="footer">
    © 2026 Projet de Fin d'Études
</div>

</body>
</html>
