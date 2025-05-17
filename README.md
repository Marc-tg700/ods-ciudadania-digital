<!DOCTYPE html>
<html lang="es">
<head>
   <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ODS - Página Completa</title>

  <!-- Estilos -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick-theme.min.css">
  <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
  <style>
    body {
      background-color: #c3c3c3;
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    .imagen-con-texto {
      position: relative;
      text-align: center;
      color: white;
      margin-bottom: 30px;
    }

    .imagen-con-texto img {
      width: 100%;
      max-height: 400px;
      object-fit: cover;
      filter: brightness(60%);
    }

    .texto-superpuesto {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 48px;
      font-weight: bold;
      text-shadow: 2px 2px 8px #000;
      color: #fff;
    }
    /* Acordeón */
    .accordion-item {
      border: 1px solid #fffdfd;
      margin-bottom: 5px;
    }

    .accordion-header {
      background-color: #035ddb;
      color: white;
      padding: 25px;
      cursor: pointer;
    }

    .accordion-content {
      padding: 25px;
      display: none;
      background-color: #0187df;
    }

    /* Carrusel */
    .carousel img {
      width: 100%;
      max-height: 600px;
      object-fit: contain;
    }

    /* Mapa */
    #map {
      height: 400px;
      margin-top: 40px;
    }
  </style>
</head>
<body>

 <!-- Imagen principal con texto animado -->
  <div class="imagen-con-texto">
    <img src="https://ciec.edu.co/wp-content/uploads/2024/07/Academicos-buscan-replantear-los-ODS-de-la-ONU.jpg" alt="ODS ONU">
    <h1 id="titulo" class="texto-superpuesto">Objetivos de Desarrollo Sostenible</h1>
  </div>

  <!-- Carga la biblioteca GSAP -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.10.4/gsap.min.js"></script>

  <script>
    // Aplica animación al título
    gsap.to("#titulo", {
      duration: 2,
      repeat: -1,
      yoyo: true,
      ease: 'elastic.out(1.5, 0.5)',
      color: '#ff69b4',
      scale: 1.2
    });
  </script>

</body>

  <!-- Acordeón -->
  <h1>Preguntas Frecuentes sobre los ODS</h1>
  <div class="accordion">
    <div class="accordion-item">
      <div class="accordion-header">¿Qué son los ODS?</div>
      <div class="accordion-content">Los Objetivos de Desarrollo Sostenible son un plan de la ONU para lograr un futuro mejor.</div>
    </div>
    <div class="accordion-item">
      <div class="accordion-header">¿Qué busca la ODS 9?</div>
      <div class="accordion-content">Promover infraestructuras resilientes, industrialización sostenible e innovación.</div>
    </div>
    <div class="accordion-item">
      <div class="accordion-header">¿Cuántos ODS hay?</div>
      <div class="accordion-content">Hay 17 objetivos, que abordan temas como la pobreza, la educación y el medio ambiente.</div>
    </div>
    <div class="accordion-item">
      <div class="accordion-header">¿Porqué es importante la infraestructura?</div>
      <div class="accordion-content">Porque impulsa el crecimiento económico y conecta regiones.</div>
    </div>
    <div class="accordion-item">
      <div class="accordion-header">¿Qué sectores apoya este ODS?</div>
      <div class="accordion-content">Manufactura, tecnología, transporte y telecomunicaciones.</div>
    </div>
    <div class="accordion-item">
      <div class="accordion-header">¿Qué reto enfrenta esta ODS?</div>
      <div class="accordion-content">Falta de inversión en tecnología e infraestructura en países en desarrollo.</div>
    </div>
  </div>
  
  <!-- Carrusel -->
  <h1>Proyectos Sostenibles</h1>
  <div class="carousel">
    <!-- Imágenes desde URL -->
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%209%20-%20sp_0.png" alt="ODS 9"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/S-WEB-Goal-16.png" alt="ODS 16"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%202%20-%20sp.png" alt="ODS 2"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%203%20-%20sp_1.png" alt="ODS 3"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%204%20-%20sp.png" alt="ODS 4"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%205%20-%20sp.png" alt="ODS 5"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%206%20-%20sp.png" alt="ODS 6"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%207%20-%20sp.png" alt="ODS 7"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%208%20-%20sp.png" alt="ODS 8"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2010%20-%20sp.png" alt="ODS 10"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2011%20-sp.png" alt="ODS 11"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2012%20-%20sp.png" alt="ODS 12"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2013%20-%20sp.png" alt="ODS 13"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2014%20-%20sp.png" alt="ODS 14"></div>
    <div><img src="https://sdgs.un.org/sites/default/files/2020-11/Goal%2015%20-%20sp.png" alt="ODS 15"></div>
    <!-- Imágenes subidas por ti -->
    <div><img src="/mnt/data/57f50295-71ac-4804-9eb2-f4069dd189ec.png" alt="Infografía ODS 9"></div>
    <div><img src="/mnt/data/f987c31c-d6ba-4891-a685-3b586011a4de.png" alt="ODS 16 Logo"></div>
  </div>

  <!-- Mapa -->
  <h1>Proyectos en el Mundo</h1>
  <div id="map"></div>

  <!-- Scripts -->
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
  <script src="https://cdnjs.cloudflare.com/ajax/libs/slick-carousel/1.8.1/slick.min.js"></script>
  <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
  <script>
    $(document).ready(function () {
      // Acordeón
      $(".accordion-header").click(function () {
        $(this).next(".accordion-content").slideToggle();
      });

      // Carrusel
      $('.carousel').slick({
        autoplay: true,
        dots: true,
        arrows: false,
        slidesToShow: 1,
        adaptiveHeight: true
      });
    });

    // Mapa
    const map = L.map('map').setView([20, 0], 2);
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
      maxZoom: 18,
    }).addTo(map);

    L.marker([40.7128, -74.0060]).addTo(map)
      .bindPopup('Nueva York: Proyecto de energía limpia.');
  </script>
</body>
</html>
