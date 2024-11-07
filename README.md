# Joel_Laboratorio222
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carrusel Simple</title>
    <link rel="stylesheet" href="Carrusel.css">
</head>
<body>

    <div class="carousel">
        <div class="slides">
            <div class="slide">
                <img src="IMG_5087-1-600x900.jpg" alt="Imagen 1">
            </div>
            <div class="slide">
                <img src="IMG_5087-1-600x900.jpg" alt="Imagen 2">
            </div>
            <div class="slide">
                <img src="IMG_5087-1-600x900.jpg" alt="Imagen 3">
            </div>
        </div>
    </div>

    * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-color: #f3f3f3;
}

.carousel {
    width: 80%;
    max-width: 600px;
    overflow: hidden;
    border-radius: 10px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.slides {
    display: flex;
    width: 300%;
    animation: slide 12s infinite;
}

.slide {
    width: 100%;
    flex-shrink: 0;
}

.slide img {
    width: 50%;        
    height: auto;       
    object-fit: cover; 
    border-radius: 10px;
}

@keyframes slide {
    0%, 33% { transform: translateX(0); }
    34%, 66% { transform: translateX(-100%); }
    67%, 100% { transform: translateX(-200%); }
}


</body>
</html>
