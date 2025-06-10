<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Turismo en Riohacha - La Guajira</title>

  <!-- Bootstrap CSS -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">

  <style>
    body {
      font-family: 'Roboto', sans-serif;
      background: #f4f4f4;
      color: #333;
    }
    header {
      position: relative;
      height: 60vh;
      background: url('file-P3ji6kfg4MWWTku656bYeP') center/cover no-repeat;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
    }
    header h1 {
      font-size: 3em;
      background: rgba(0,0,0,0.4);
      padding: 20px;
      border-radius: 10px;
    }
    .section-title {
      color: #ff7e5f;
      margin-bottom: 20px;
      text-align: center;
    }
    .card-img-top {
      height: 200px;
      object-fit: cover;
    }
    footer {
      background: #333;
      color: #fff;
      padding: 20px 0;
      text-align: center;
    }
  </style>
</head>
<body>

  <!-- Banner con 1 imagen -->
  <header>
    <h1>Descubre Riohacha - La Guajira</h1>
  </header>

  <main class="container my-5">
    <h2 class="section-title">Lugares y Actividades</h2>
    <div class="row g-4">
      <div class="col-md-4">
        <div class="card shadow-sm">
          <img src="file-TEicLJ8ujoLsNBHa6TUGtw" class="card-img-top" alt="Atardecer en Riohacha">
          <div class="card-body">
            <h5 class="card-title">Atardecer en Riohacha</h5>
            <p class="card-text">Disfruta de un mágico atardecer a la orilla del mar Caribe, con un ambiente único y acogedor.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card shadow-sm">
          <img src="file-572av2bMJ7m2SDKmdJcErw" class="card-img-top" alt="Playas de Palomino">
          <div class="card-body">
            <h5 class="card-title">Playas de Palomino</h5>
            <p class="card-text">Arena blanca y palmeras infinitas para disfrutar del sol y la brisa caribeña.</p>
          </div>
        </div>
      </div>

      <div class="col-md-4">
        <div class="card shadow-sm">
          <img src="file-8K9nMbFKtYfjUoPkz4Nxgs" class="card-img-top" alt="I Love Riohacha">
          <div class="card-body">
            <h5 class="card-title">I Love Riohacha</h5>
            <p class="card-text">Un símbolo icónico de la ciudad, perfecto para tus fotos y recuerdos inolvidables.</p>
          </div>
        </div>
      </div>
    </div>
  </main>

  <footer>
    <p>&copy; 2025 Turismo Riohacha - Todos los derechos reservados</p>
  </footer>

  <!-- Bootstrap Bundle JS (con Popper) -->
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"></script>

  <!-- Animación de aparición suave -->
  <script>
    document.addEventListener("DOMContentLoaded", () => {
      const cards = document.querySelectorAll(".card");
      cards.forEach((card, index) => {
        setTimeout(() => {
          card.classList.add("shadow-lg");
        }, index * 300);
      });
    });
  </script>

</body>
</html>

