<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nutrients You Need (N&N) | Productos FitLine Completos</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css">
    <style>
        :root {
            --primary: #0056b3;
            --secondary: #ff6b00;
            --accent: #00a651;
            --light: #f8f9fa;
            --dark: #212529;
            --gray: #6c757d;
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
            overflow-x: hidden;
            background-color: #f5f7fa;
        }

        h1, h2, h3, h4, h5, h6 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            line-height: 1.2;
            margin-bottom: 1rem;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
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
            border: none;
            cursor: pointer;
            font-family: 'Montserrat', sans-serif;
            font-size: 14px;
        }

        .btn-primary {
            background: linear-gradient(135deg, var(--primary), #003d82);
            color: white;
            box-shadow: 0 4px 15px rgba(0, 86, 179, 0.3);
        }

        .btn-primary:hover {
            background: linear-gradient(135deg, #004494, #002e63);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 86, 179, 0.4);
        }

        .btn-secondary {
            background: linear-gradient(135deg, var(--secondary), #e05a00);
            color: white;
            box-shadow: 0 4px 15px rgba(255, 107, 0, 0.3);
        }

        .btn-secondary:hover {
            background: linear-gradient(135deg, #e05a00, #c94e00);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(255, 107, 0, 0.4);
        }

        .btn-accent {
            background: linear-gradient(135deg, var(--accent), #008a43);
            color: white;
            box-shadow: 0 4px 15px rgba(0, 166, 81, 0.3);
        }

        .btn-accent:hover {
            background: linear-gradient(135deg, #008a43, #007036);
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(0, 166, 81, 0.4);
        }

        /* Header */
        header {
            position: fixed;
            top: 0;
            width: 100%;
            z-index: 1000;
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            padding: 15px 0;
            transition: var(--transition);
        }

        header.scrolled {
            padding: 10px 0;
            background-color: rgba(255, 255, 255, 0.98);
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
            font-size: 24px;
            margin-bottom: 0;
            color: var(--primary);
        }

        .logo span {
            color: var(--secondary);
        }

        .nav-menu {
            display: flex;
            list-style: none;
        }

        .nav-menu li {
            margin-left: 30px;
        }

        .nav-menu a {
            text-decoration: none;
            color: var(--dark);
            font-weight: 600;
            font-size: 16px;
            position: relative;
            padding: 5px 0;
            transition: var(--transition);
        }

        .nav-menu a:hover {
            color: var(--primary);
        }

        .nav-menu a:after {
            content: '';
            position: absolute;
            width: 0;
            height: 2px;
            background: var(--primary);
            bottom: 0;
            left: 0;
            transition: var(--transition);
        }

        .nav-menu a:hover:after {
            width: 100%;
        }

        .mobile-toggle {
            display: none;
            font-size: 24px;
            cursor: pointer;
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            min-height: 700px;
            background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)), url('https://www.pm-international.com/es/es/images/default-source/default-album/hero-bg.jpg?sfvrsn=0') center/cover no-repeat;
            display: flex;
            align-items: center;
            color: white;
            padding-top: 80px;
        }

        .hero-content {
            max-width: 700px;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 20px;
            line-height: 1.2;
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 30px;
            max-width: 600px;
        }

        .hero-buttons {
            display: flex;
            gap: 20px;
            margin-top: 30px;
        }

        /* Features */
        .features {
            padding: 100px 0;
            background-color: white;
        }

        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-title h2 {
            font-size: 2.5rem;
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

        .features-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .feature-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }

        .feature-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 40px rgba(0, 0, 0, 0.15);
        }

        .feature-img {
            height: 200px;
            overflow: hidden;
        }

        .feature-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .feature-card:hover .feature-img img {
            transform: scale(1.05);
        }

        .feature-content {
            padding: 25px;
        }

        .feature-content h3 {
            font-size: 1.5rem;
            color: var(--primary);
            margin-bottom: 15px;
        }

        /* Products */
        .products {
            padding: 100px 0;
            background-color: var(--light);
        }

        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 30px;
        }

        .product-card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
            display: flex;
            flex-direction: column;
            height: 100%;
        }

        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.1);
        }

        .product-img {
            height: 220px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background: #f9f9f9;
        }

        .product-img img {
            max-height: 180px;
            max-width: 100%;
            transition: var(--transition);
        }

        .product-card:hover .product-img img {
            transform: scale(1.05);
        }

        .product-content {
            padding: 20px;
            text-align: center;
            flex-grow: 1;
            display: flex;
            flex-direction: column;
        }

        .product-content h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
        }

        .product-content .price {
            color: var(--primary);
            font-weight: 700;
            font-size: 1.3rem;
            margin: 10px 0;
        }

        .product-content .btn {
            width: 100%;
            margin-top: auto;
            padding: 10px 15px;
        }

        .category-title {
            text-align: center;
            margin: 60px 0 30px;
            padding-bottom: 15px;
            border-bottom: 3px solid var(--secondary);
            font-size: 1.8rem;
            color: var(--primary);
        }

        /* Networking */
        .networking {
            padding: 100px 0;
            background: linear-gradient(135deg, #1a3a6c, #0e2446);
            color: white;
        }

        .networking-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .networking-text h2 {
            color: white;
            font-size: 2.5rem;
        }

        .networking-text p {
            margin-bottom: 20px;
        }

        .levels {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }

        .level-card {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: var(--transition);
        }

        .level-card:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateY(-5px);
        }

        .level-card h4 {
            color: var(--secondary);
            margin-bottom: 10px;
        }

        .networking-image {
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.3);
        }

        .networking-image img {
            width: 100%;
            height: auto;
            display: block;
        }

        /* Testimonials */
        .testimonials {
            padding: 100px 0;
            background-color: white;
        }

        .testimonials-container {
            max-width: 900px;
            margin: 0 auto;
        }

        .testimonial-slider {
            position: relative;
            overflow: hidden;
        }

        .testimonial-track {
            display: flex;
            transition: transform 0.5s ease;
        }

        .testimonial-card {
            min-width: 100%;
            padding: 40px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.05);
            text-align: center;
        }

        .testimonial-card img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            margin-bottom: 20px;
            border: 3px solid var(--primary);
        }

        .testimonial-card h4 {
            color: var(--primary);
            margin-bottom: 5px;
        }

        .testimonial-card .position {
            color: var(--gray);
            font-style: italic;
            margin-bottom: 20px;
        }

        .testimonial-text {
            font-style: italic;
            position: relative;
        }

        .testimonial-text:before,
        .testimonial-text:after {
            content: '"';
            font-size: 4rem;
            color: rgba(0, 86, 179, 0.1);
            position: absolute;
            line-height: 1;
        }

        .testimonial-text:before {
            top: -20px;
            left: -20px;
        }

        .testimonial-text:after {
            bottom: -50px;
            right: -20px;
        }

        .slider-nav {
            display: flex;
            justify-content: center;
            margin-top: 40px;
            gap: 10px;
        }

        .slider-dot {
            width: 12px;
            height: 12px;
            border-radius: 50%;
            background: #ddd;
            cursor: pointer;
            transition: var(--transition);
        }

        .slider-dot.active {
            background: var(--primary);
            transform: scale(1.2);
        }

        /* CTA */
        .cta {
            padding: 100px 0;
            background: linear-gradient(135deg, var(--primary), #003d82);
            color: white;
            text-align: center;
        }

        .cta h2 {
            font-size: 2.8rem;
            margin-bottom: 20px;
            color: white;
        }

        .cta p {
            max-width: 700px;
            margin: 0 auto 30px;
            font-size: 1.2rem;
        }

        /* Footer */
        footer {
            background: var(--dark);
            color: white;
            padding: 70px 0 0;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 50px;
        }

        .footer-col h4 {
            color: white;
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

        .footer-col p {
            margin-bottom: 20px;
            opacity: 0.8;
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
            padding: 20px 0;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }

        /* Animations */
        [data-aos] {
            transition: all 1s ease;
        }

        /* Responsive */
        @media (max-width: 992px) {
            .hero h1 {
                font-size: 2.8rem;
            }
            
            .networking-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            
            .levels {
                justify-content: center;
            }
        }

        @media (max-width: 768px) {
            .mobile-toggle {
                display: block;
            }
            
            .nav-menu {
                position: fixed;
                top: 80px;
                left: -100%;
                width: 100%;
                height: calc(100vh - 80px);
                background: white;
                flex-direction: column;
                align-items: center;
                justify-content: flex-start;
                padding-top: 50px;
                transition: var(--transition);
            }
            
            .nav-menu.active {
                left: 0;
            }
            
            .nav-menu li {
                margin: 15px 0;
            }
            
            .hero h1 {
                font-size: 2.3rem;
            }
            
            .hero-buttons {
                flex-direction: column;
                gap: 15px;
            }
            
            .btn {
                width: 100%;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header id="header">
        <div class="container header-container">
            <div class="logo">
                <h1>Nutrients <span>You Need</span></h1>
            </div>
            
            <div class="mobile-toggle" id="mobileToggle">
                <i class="fas fa-bars"></i>
            </div>
            
            <ul class="nav-menu" id="navMenu">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#productos">Productos</a></li>
                <li><a href="#nosotros">Quiénes Somos</a></li>
                <li><a href="#networking">Networking</a></li>
                <li><a href="#unete" class="btn btn-accent">Únete a Nosotros</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="container">
            <div class="hero-content">
                <h1 data-aos="fade-right">Todos los Productos FitLine en un Solo Lugar</h1>
                <p data-aos="fade-right" data-aos-delay="100">Descubre la gama completa de suplementos nutricionales de FitLine con los mejores precios y tu código de afiliado.</p>
                <div class="hero-buttons" data-aos="fade-right" data-aos-delay="200">
                    <a href="#productos" class="btn btn-primary">Ver Productos</a>
                    <a href="#unete" class="btn btn-secondary">Únete al Equipo</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Products -->
    <section class="products" id="productos">
        <div class="container">
            <div class="section-title" data-aos="fade-up">
                <h2>Catálogo Completo de Productos FitLine</h2>
                <p>Todos los productos disponibles con enlaces directos a la tienda oficial</p>
            </div>
            
            <!-- Suplementos Nutricionales -->
            <h3 class="category-title" data-aos="fade-right">Suplementos Nutricionales</h3>
            <div class="products-grid">
                <!-- Restorate -->
                <div class="product-card" data-aos="fade-up" data-aos-delay="100">
                    <div class="product-img">
                        <img src="https://www.pm-international.com/es/es/images/default-source/products/fitline/fitline-restorate/fitline_restorate_30st_250x250px.png?sfvrsn=2" alt="FitLine Restorate">
                    </div>
                    <div
