<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Catálogo Completo FitLine | Nutrients You Need</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;500;600;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #0056b3;
            --secondary: #ff6b00;
            --accent: #00a651;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
            --light-gray: #e9ecef;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Open Sans', sans-serif;
            line-height: 1.6;
            color: var(--dark);
            background-color: #f5f7fa;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary), #003d82);
            color: white;
            padding: 20px 0;
            position: sticky;
            top: 0;
            z-index: 100;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
        }
        
        .logo h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.8rem;
            font-weight: 700;
        }
        
        .logo span {
            color: var(--secondary);
        }
        
        .nav-menu {
            display: flex;
            list-style: none;
        }
        
        .nav-menu li {
            margin-left: 20px;
        }
        
        .nav-menu a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: var(--transition);
        }
        
        .nav-menu a:hover {
            color: var(--secondary);
        }
        
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://www.pm-international.com/es/es/images/default-source/default-album/hero-bg.jpg?sfvrsn=0') center/cover no-repeat;
            padding: 100px 0;
            color: white;
            text-align: center;
        }
        
        .hero h1 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.8rem;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 30px;
        }
        
        .btn {
            display: inline-block;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: var(--transition);
            font-size: 14px;
            margin: 5px;
        }
        
        .btn-primary {
            background: white;
            color: var(--primary);
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
        }
        
        .btn-primary:hover {
            background: var(--light-gray);
            transform: translateY(-3px);
        }
        
        .btn-secondary {
            background: var(--secondary);
            color: white;
            box-shadow: 0 4px 15px rgba(255, 107, 0, 0.3);
        }
        
        .btn-secondary:hover {
            background: #e05a00;
            transform: translateY(-3px);
        }
        
        .section-title {
            text-align: center;
            margin: 60px 0 40px;
        }
        
        .section-title h2 {
            font-family: 'Montserrat', sans-serif;
            font-size: 2.2rem;
            position: relative;
            display: inline-block;
            padding-bottom: 15px;
        }
        
        .section-title h2:after {
            content: '';
            position: absolute;
            width: 80px;
            height: 4px;
            background: var(--secondary);
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }
        
        .category-title {
            text-align: center;
            margin: 50px 0 30px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--secondary);
            font-family: 'Montserrat', sans-serif;
            font-size: 1.8rem;
            color: var(--primary);
        }
        
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 60px;
        }
        
        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.08);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
            height: 100%;
        }
        
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.12);
        }
        
        .product-img {
            height: 250px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background: #f9f9f9;
        }
        
        .product-img img {
            max-height: 210px;
            max-width: 100%;
            transition: var(--transition);
        }
        
        .product-card:hover .product-img img {
            transform: scale(1.05);
        }
        
        .product-content {
            padding: 20px;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }
        
        .product-content h3 {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--primary);
        }
        
        .product-content .flavor {
            display: inline-block;
            background: var(--light-gray);
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 0.85rem;
            margin-bottom: 10px;
        }
        
        .product-content .price {
            color: var(--primary);
            font-weight: 700;
            font-size: 1.4rem;
            margin: 10px 0;
        }
        
        .product-content .btn {
            width: 100%;
            margin-top: auto;
            padding: 10px 15px;
            font-size: 0.9rem;
        }
        
        .flavors-container {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 10px 0;
        }
        
        .flavor-badge {
            background: var(--light-gray);
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            transition: var(--transition);
            cursor: pointer;
        }
        
        .flavor-badge:hover {
            background: var(--secondary);
            color: white;
        }
        
        .flavor-badge.active {
            background: var(--primary);
            color: white;
        }
        
        .featured-products {
            background: var(--light);
            padding: 60px 0;
        }
        
        .testimonials {
            padding: 80px 0;
            background: linear-gradient(135deg, #1a3a6c, #0e2446);
            color: white;
        }
        
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .testimonial-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 30px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .testimonial-card img {
            width: 70px;
            height: 70px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 20px;
            border: 3px solid var(--secondary);
        }
        
        .testimonial-card h4 {
            color: var(--secondary);
            margin-bottom: 5px;
        }
        
        .position {
            font-style: italic;
            margin-bottom: 15px;
            opacity: 0.8;
        }
        
        .testimonial-text {
            font-style: italic;
        }
        
        .cta {
            padding: 80px 0;
            text-align: center;
            background: linear-gradient(135deg, var(--accent), #008a43);
            color: white;
        }
        
        .cta h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
        }
        
        .benefits {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }
        
        .benefit {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
        }
        
        .benefit i {
            font-size: 2.5rem;
            margin-bottom: 15px;
            color: white;
        }
        
        footer {
            background: var(--dark);
            color: white;
            padding: 60px 0 20px;
        }
        
        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-col h4 {
            font-family: 'Montserrat', sans-serif;
            font-size: 1.3rem;
            margin-bottom: 20px;
            position: relative;
            padding-bottom: 10px;
        }
        
        .footer-col h4:after {
            content: '';
            position: absolute;
            width: 50px;
            height: 3px;
            background: var(--secondary);
            bottom: 0;
            left: 0;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 10px;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: var(--transition);
        }
        
        .footer-links a:hover {
            color: var(--secondary);
            padding-left: 5px;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-links a {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 18px;
            transition: var(--transition);
        }
        
        .social-links a:hover {
            background: var(--secondary);
            transform: translateY(-5px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }
        
        @media (max-width: 768px) {
            .header-container {
                flex-direction: column;
                text-align: center;
            }
            
            .nav-menu {
                margin-top: 20px;
                justify-content: center;
            }
            
            .nav-menu li {
                margin: 0 10px;
            }
            
            .hero h1 {
                font-size: 2.2rem;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <h1>Nutrients <span>You Need</span></h1>
            </div>
            <ul class="nav-menu">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#productos">Productos</a></li>
                <li><a href="#networking">Networking</a></li>
                <li><a href="#unete">Únete</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="container">
            <h1>Catálogo Completo de Productos FitLine</h1>
            <p>Descubre todos los productos de nutrición avanzada con tecnología NTC®. Suplementos, vitaminas y productos para el cuidado personal de máxima calidad.</p>
            <a href="#productos" class="btn btn-primary">Ver Productos</a>
            <a href="#unete" class="btn btn-secondary">Únete al Equipo</a>
        </div>
    </section>

    <!-- Product Categories -->
    <section class="featured-products" id="productos">
        <div class="container">
            <div class="section-title">
                <h2>Todas las Categorías de Productos</h2>
                <p>Explora la gama completa de FitLine organizada por categorías</p>
            </div>

            <!-- Nutrición Deportiva -->
            <h3 class="category-title">Nutrición Deportiva</h3>
            <div class="products-grid">
                <!-- Restorate -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-restorate/fitline_restorate_30st_250x250px.png?sfvrsn=2" alt="FitLine Restorate">
                    </div>
                    <div class="product-content">
                        <h3>FitLine Restorate</h3>
                        <p>Suplemento para la regeneración muscular durante la noche</p>
                        <div class="flavors-container">
                            <span class="flavor-badge active">Original</span>
                        </div>
                        <div class="price">39,90 €</div>
                        <a href="https://www.pm-international.com/es/es/acerca-de-nuestros-productos/restorate/?TP=21075705" class="btn btn-primary">Comprar Ahora</a>
                    </div>
                </div>
                
                <!-- PowerCocktail -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-powercocktail/fitline_powercocktail_250x250px.png?sfvrsn=2" alt="FitLine PowerCocktail">
                    </div>
                    <div class="product-content">
                        <h3>FitLine PowerCocktail</h3>
                        <p>Bebida isotónica para un rendimiento óptimo</p>
                        <div class="flavors-container">
                            <span class="flavor-badge active">Frutas del Bosque</span>
                            <span class="flavor-badge">Tropical</span>
                            <span class="flavor-badge">Naranja-Mango</span>
                        </div>
                        <div class="price">29,90 €</div>
                        <a href="https://www.pm-international.com/es/es/acerca-de-nuestros-productos/powercocktail/?TP=21075705" class="btn btn-primary">Comprar Ahora</a>
                    </div>
                </div>
                
                <!-- Endurance -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-endurance/fitline_endurance_250x250px.png?sfvrsn=2" alt="FitLine Endurance">
                    </div>
                    <div class="product-content">
                        <h3>FitLine Endurance</h3>
                        <p>Mejora la resistencia y reduce la fatiga</p>
                        <div class="flavors-container">
                            <span class="flavor-badge active">Frutas del Bosque</span>
                        </div>
                        <div class="price">39,90 €</div>
                        <a href="https://www.pm-international.com/es/es/acerca-de-nuestros-productos/endurance/?TP=21075705" class="btn btn-primary">Comprar Ahora</a>
                    </div>
                </div>
            </div>

            <!-- Control de Peso -->
            <h3 class="category-title">Control de Peso</h3>
            <div class="products-grid">
                <!-- ProShape -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-proshape/fitline_proshape_250x250px.png?sfvrsn=2" alt="FitLine ProShape">
                    </div>
                    <div class="product-content">
                        <h3>FitLine ProShape</h3>
                        <p>Batido proteico para el control del peso</p>
                        <div class="flavors-container">
                            <span class="flavor-badge active">Vainilla</span>
                            <span class="flavor-badge">Chocolate</span>
                            <span class="flavor-badge">Fresa</span>
                        </div>
                        <div class="price">42,90 €</div>
                        <a href="https://www.pm-international.com/es/es/acerca-de-nuestros-productos/proshape/?TP=21075705" class="btn btn-primary">Comprar Ahora</a>
                    </div>
                </div>
                
                <!-- Metabolic Pack -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-metabolic-pack/fitline_metabolic-pack_250x250px.png?sfvrsn=2" alt="FitLine Metabolic Pack">
                    </div>
                    <div class="product-content">
                        <h3>FitLine Metabolic Pack</h3>
                        <p>Pack completo para activar el metabolismo</p>
                        <div class="price">119,90 €</div>
                        <a href="https://www.pm-international.com/es/es/acerca-de-nuestros-productos/metabolic-pack/?TP=21075705" class="btn btn-primary">Comprar Ahora</a>
                    </div>
                </div>
            </div>

            <!-- Salud y Bienestar -->
            <h3 class="category-title">Salud y Bienestar</h3>
            <div class="products-grid">
                <!-- Basics -->
                <div class="product-card">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-basics/fitline_basics_250x250px.png?sfvrsn=2" alt="FitLine Basics">
                    </div>
                    <div class="product-content">
                        <h3>FitLine Basics</h3>
                        <p>Complejo vitamínico-mineral para el bienestar diario</p>
                        <div class="flavors-container">
                            <span class="flavor-badge active">Original</span>
                        </div>
                        <div class="price">34,90 €</div>
                        <a href="ht


