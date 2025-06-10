<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>K_ory - Turismo en Riohacha</title>
<!-- Bootstrap CSS -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
<style>
    body {
        font-family: Arial, sans-serif;
        background: #f0f8ff;
        color: #333;
    }
    header {
        background-image: url('Como-Llegar-a-Riohacha-La-Guajira-Hotel-Chip-Viajero-13.jpg');
        background-size: cover;
        background-position: center;
        height: 450px;
        display: flex;
        align-items: center;
        justify-content: center;
        position: relative;
    }
    header::before {
        content: "";
        position: absolute;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.4);
    }
    header h1 {
        position: relative;
        font-size: 3rem;
        color: #fff;
        background-color: rgba(255, 255, 255, 0.2);
        padding: 20px;
        border-radius: 10px;
    }
    .cart-btn {
        background: #ff4500;
        color: #fff;
        border: none;
        border-radius: 50px;
        padding: 8px 15px;
        cursor: pointer;
        font-size: 1rem;
        box-shadow: 0 4px 6px rgba(0,0,0,0.2);
        transition: background 0.3s;
    }
    .cart-btn:hover {
        background: #e63e00;
    }
    .cart-count {
        font-weight: bold;
        margin-left: 5px;
    }
    .product {
        background: #fff;
        border-radius: 15px;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        padding: 20px;
        margin-bottom: 20px;
        transition: transform 0.3s;
    }
    .product:hover {
        transform: translateY(-5px);
    }
    .product h3 {
        color: #ff4500;
        margin-bottom: 10px;
    }
    .product button {
        background: #ff4500;
        color: #fff;
        border: none;
        border-radius: 20px;
        padding: 10px 20px;
        transition: background 0.3s;
    }
    .product button:hover {
        background: #e63e00;
    }
    footer {
        background: #ff4500;
        color: #fff;
        text-align: center;
        padding: 20px;
    }
</style>
</head>
<body>

<!-- Navbar -->
<nav class="navbar navbar-expand-lg navbar-dark" style="background-color:#ff4500;">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">K_ory</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav" 
      aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item"><a class="nav-link active" href="#">Inicio</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Tours</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Contacto</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Acerca de</a></li>
      </ul>
      <button class="cart-btn">
          <i class="fas fa-shopping-cart"></i> Carrito 
          <span class="cart-count">0</span>
      </button>
    </div>
  </div>
</nav>

<!-- Header -->
<header>
    <h1>Descubre Riohacha</h1>
</header>

<!-- Sección de Tours -->
<div class="container mt-5">
    <h2 class="text-center mb-4" style="color:#ff4500;">Tours y Aventuras</h2>
    <div class="row">
        <div class="col-md-4">
            <div class="product">
                <h3>Tour Playa Blanca</h3>
                <p>Relájate en las aguas turquesas de Playa Blanca.</p>
                <button class="add-to-cart">Agregar al carrito</button>
            </div>
        </div>
        <div class="col-md-4">
            <div class="product">
                <h3>Tour Cultura Wayuu</h3>
                <p>Descubre las tradiciones y la cultura Wayuu.</p>
                <button class="add-to-cart">Agregar al carrito</button>
            </div>
        </div>
        <div class="col-md-4">
            <div class="product">
                <h3>Tour Malecón</h3>
                <p>Disfruta de un paseo inolvidable en el malecón de Riohacha.</p>
                <button class="add-to-cart">Agregar al carrito</button>
            </div>
        </div>
    </div>
</div>

<!-- Footer -->
<footer>
    <p>&copy; 2025 K_ory - Turismo en Riohacha, La Guajira. Todos los derechos reservados.</p>
</footer>

<!-- JS de Bootstrap y funciones de carrito -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
<script>
    let cartCount = 0;
    const cartCountEl = document.querySelector('.cart-count');
    const addToCartButtons = document.querySelectorAll('.add-to-cart');

    addToCartButtons.forEach(button => {
        button.addEventListener('click', () => {
            cartCount++;
            cartCountEl.textContent = cartCount;
            alert('Producto agregado al carrito');
        });
    });
</script>
</body>
</html>
