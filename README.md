# index.html1
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Projet de Fin d'Études | Houria & Rachida Mourad</title> 
    <style> 
        :root {
            --primary-color: #1a2a6c; /* أزرق داكن أكاديمي */
            --secondary-color: #b21f1f; /* أحمر للتنبيهات والعناوين */
            --accent-color: #fdbb2d; /* ذهبي كلمسة فنية */
            --bg-color: #f8f9fa; /* خلفية رمادية فاتحة جداً */
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
            box-shadow: 0 4px 12px rgba(0,0,0,0.15);
        }

        .logo-univ {
            width: 130px;
            background: white;
            padding: 10px;
            border-radius: 50%;
            margin-bottom: 20px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.2);
        }

        .container {
            max-width: 1000px;
            margin: -40px auto 40px;
            background: white;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
        }

        h1 { font-size: 28px; margin-bottom: 10px; }
        p.department { font-size: 18px; opacity: 0.9; margin-top: 0; }
/* Slider */
.slider {
    position: relative;
    max-width: 100%;
    height: 300px;
    overflow: hidden;
    border-radius: 12px;
    margin-top: 20px;
}

.slides {
    display: flex;
    width: 300%;
    animation: slide 12s infinite;
}

.slides img {
    width: 100%;
    height: 300px;
    object-fit: cover;
}

@keyframes slide {
    0% { transform: translateX(0); }
    33% { transform: translateX(0); }
    38% { transform: translateX(-100%); }
    66% { transform: translateX(-100%); }
    71% { transform: translateX(-200%); }
    100% { transform: translateX(-200%); }
}
        h2 { 
            color: var(--primary-color); 
            border-bottom: 2px solid var(--secondary-color); 
            padding-bottom: 10px; 
            margin-top: 40px; 
            font-size: 24px; 
            text-transform: uppercase; 
            letter-spacing: 1px;
        }

        /* معرض الصور المنظم | Photo Gallery */
        .gallery {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .gallery-item {
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 6px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            background: white;
            display: flex;
            flex-direction: column;
        }

        .gallery-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        .gallery-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-bottom: 4px solid var(--accent-color);
        }

        .gallery-caption {
            padding: 15px;
            text-align: center;
            font-size: 15px;
            font-weight: bold;
            color: var(--primary-color);
            background: #fff;
            flex-grow: 1;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        /* تنسيق البيانات الفنية | Fiche Technique */
        .info-grid {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 15px;
            margin-top: 20px;
            background: #f1f3f5;
            padding: 25px;
            border-radius: 10px;
            border-right: 5px solid var(--primary-color);
        }

        .info-item { font-weight: bold; color: var(--primary-color); }
        
        .description-box {
            background: #fff;
            border-right: 5px solid var(--accent-color);
            padding: 25px;
            margin-top: 20px;
            text-align: right; /* للنص العربي */
            direction: rtl;
            border-radius: 8px;
            box-shadow: inset 0 2px 5px rgba(0,0,0,0.05);
        } /* تنسيق التقنيات | Technologies */
        .tech-list {
            list-style-type: none;
            padding: 0;
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin-top: 15px;
        }

        .tech-tag {
            background: #e9ecef;
            color: var(--primary-color);
            padding: 8px 18px;
            border-radius: 25px;
            font-size: 14px;
            font-weight: bold;
            box-shadow: 0 2px 4px rgba(0,0,0,0.05);
        }

        .footer {
            text-align: center;
            padding: 25px;
            font-size: 14px;
            color: #666;
            background: #eee;
            margin-top: 50px;
            border-top: 1px solid #ddd;
        }

        /* Responsive Design */
        @media (max-width: 600px) {
            .info-grid { grid-template-columns: 1fr; padding: 15px; }
            .container { width: 92%; margin-top: -20px; padding: 20px; }
            h1 { font-size: 22px; }
            h2 { font-size: 20px; }
            .gallery { grid-template-columns: 1fr; }
        }
    </style>
</head>
<body>

<header>
    <img src="https://upload.wikimedia.org/wikipedia/dz/4/45/Logo_University_of_Mascara.png" alt="Université de Mascara" class="logo-univ">
    <h1>Université Mustapha Stambouli de Mascara</h1>
    <p class="department">Faculté de Technologie / Département d'Électrotechnique</p>
</header>

<div class="container">
    <h2>Fiche Technique du Projet</h2>
    <div class="info-grid">
        <div class="info-item">Titre du Projet:</div>
        <div>Conception et Réalisation d’un Système Intelligent de Détection d’Incidents Dangereux Monté sur un Drone</div>
        
        <div class="info-item">Réalisé par:</div>
           <div>Houria Mourad  </div>
        <div class="info-item">Réalisé par:</div>
           <div>Rachida Mourad  </div>
        
        <div class="info-item">Niveau:</div>
           <div>2ème Année Électronique</div>
        
        <div class="info-item">Encadré par:</div>
           <div>Mourad Hebali</div>
        
        <div class="info-item">Année Universitaire:</div>
              <div>2026 - 2027</div>
</div>

    <h2>Description du Projet (Résumé)</h2>
    <div class="description-box">
        هذا المشروع يهدف إلى تصميم نظام مدمج يعتمد على حساسات  محمول على درون للكشف عن المخاطر مثل الحرائق وتسرب الغازو كوارث الطبيعية  بشكل آلي وسريع، باستخدام تقنيات ESP32S3 وArduino uno  .
    </div>

    <h2>Galerie Photos du Projet</h2>
     <div class="gallery">

    <div class="gallery-item">
        <img src="" alt="Drone Intelligent Finalisé">
        <div class="gallery-caption">Drone Finalisé (Vue d'ensemble)</div>
    </div>

    <div class="gallery-item">
        <img src="" alt="Schéma Électronique Du Projet"> 
        <div class="gallery-caption">Schéma Électronique (Circuit)</div>
    </div>

    <div class="gallery-item">
        <img src="photo_2026-04-19_10-30-19.jpg" alt="Test les capteurs">
          <img src="photo_2026-04-09_00-22-54.jpg" alt="Test les capteurs">
           <img src="photo_2026-04-08_23-26-45.jpg" alt="Test les capteurs">
        <div class="gallery-caption">Test des capteurs</div>
    </div>

</div>
        

    <h2>Technologies Clés Utilisées</h2>
    <ul class="tech-list">
        <li class="tech-tag">ESP32-S3</li>     <li class="tech-tag">Arduino Uno</li>         <li class="tech-tag">ESP32-CAM</li>                 <li class="tech-tag">Capteur MQ2</li
        <li class="tech-tag">DHT22</li>        <li class="tech-tag">Capteur de pluie</li>    <li class="tech-tag"> Capteur Niveau de l'eau</li>   <li class="tech-tag">Buzzer</li>
        <li class="tech-tag">Capteur de Flamme</li>  <li class="tech-tag"> L'écran lcd</li>   <li class="tech-tag">L'écran oled</li>             <li class="tech-tag">led Rouge et vert </li>
        <li class="tech-tag">GPS </li>              <li class="tech-tag">Sim900 </li>         <li class="tech-tag">Servo Moteur </li>
        <li class="tech-tag">Capteur Bmp180</li>     <li class="tech-tag">Capteur Esp8266/li   <li class="tech-tag">Capteur vebrasion </li>
     </ul>
</div>

<div class="footer">
    &copy; 2026 Houria Mourad & Rachida Mourad - Faculté de Technologie - Mascara
</div>

</body>
</html>
