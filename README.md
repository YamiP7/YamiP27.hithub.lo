<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>COLO VAPER</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Header con nombre y logo -->
    <header class="header">
        <div class="logo-container">
            <h1 class="rainbow-text">COLO VAPER</h1>
            <img src="logo.jpeg" alt="Logo COLO VAPER" class="logo-img">
        </div>
    </header>

    <!-- Menú de navegación para las secciones -->
    <nav class="nav-bar">
        <a href="#kits-de-inicio">KITS DE INICIO</a>
        <a href="#pods-recargables">PODS RECARGABLES</a>
        <a href="#baterias">BATERÍAS</a>
        <a href="#cargadores">CARGADORES</a>
        <a href="#atomizadores">ATOMIZADORES</a>
        <a href="#accesorios">ACCESORIOS</a>
    </nav>

    <!-- Formulario de administración de productos -->
    <section class="admin-section">
        <h2>Agregar Producto</h2>
        <form id="product-form">
            <input type="text" id="product-name" placeholder="Nombre del producto" required>
            <input type="number" id="product-price" placeholder="Precio" required>
            <input type="number" id="product-stock" placeholder="Stock" required>
            <input type="file" id="product-image" accept="image/*" required>
            <select id="product-category" required>
                <option value="kits-de-inicio">KITS DE INICIO</option>
                <option value="pods-recargables">PODS RECARGABLES</option>
                <option value="baterias">BATERÍAS</option>
                <option value="cargadores">CARGADORES</option>
                <option value="atomizadores">ATOMIZADORES</option>
                <option value="accesorios">ACCESORIOS</option>
            </select>
            <button type="submit">Agregar Producto</button>
        </form>
    </section>

    <!-- Contenedor de productos para cada categoría -->
    <div class="products-section">
        <section id="kits-de-inicio">
            <h2>KITS DE INICIO</h2>
            <div class="product-grid" id="kits-de-inicio-grid"></div>
        </section>
        <section id="pods-recargables">
            <h2>PODS RECARGABLES</h2>
            <div class="product-grid" id="pods-recargables-grid"></div>
        </section>
        <section id="baterias">
            <h2>BATERÍAS</h2>
            <div class="product-grid" id="baterias-grid"></div>
        </section>
        <section id="cargadores">
            <h2>CARGADORES</h2>
            <div class="product-grid" id="cargadores-grid"></div>
        </section>
        <section id="atomizadores">
            <h2>ATOMIZADORES</h2>
            <div class="product-grid" id="atomizadores-grid"></div>
        </section>
        <section id="accesorios">
            <h2>ACCESORIOS</h2>
            <div class="product-grid" id="accesorios-grid"></div>
        </section>
    </div>

    <!-- Script para manejar la lógica de productos -->
    <script src="script.js"></script>
</body>
</html>
