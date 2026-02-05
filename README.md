<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sanitas | Clínicas Dentales - Tu Clínica Dental de Confianza</title>
    <meta name="description" content="Sanitas Clínicas dentales con más de 15 años de experiencia. Implantes, ortodoncia invisible, estética dental y urgencias 24/7. Primera consulta gratuita.">
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600;700&family=DM+Sans:wght@400;500;600;700&family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

    <style>
        :root {
            --color-primary: #0A4D68;
            --color-primary-light: #088395;
            --color-accent: #05BFDB;
            --color-neutral-100: #FAFBFC;
            --color-neutral-200: #F0F4F8;
            --color-neutral-300: #D9E2EC;
            --color-neutral-700: #334E68;
            --color-neutral-900: #102A43;
            --color-success: #47B881;
            --color-warning: #FFB84D;
            --color-urgent: #F76C6C;
            
            --font-display: 'Cormorant Garamond', serif;
            --font-body: 'DM Sans', sans-serif;
            --font-heading: 'Poppins', sans-serif;
            
            --spacing-xs: 0.5rem;
            --spacing-sm: 1rem;
            --spacing-md: 1.5rem;
            --spacing-lg: 2.5rem;
            --spacing-xl: 4rem;
            --spacing-2xl: 6rem;
            
            --radius-sm: 8px;
            --radius-md: 16px;
            --radius-lg: 24px;
            
            --shadow-sm: 0 2px 8px rgba(16, 42, 67, 0.06);
            --shadow-md: 0 4px 16px rgba(16, 42, 67, 0.08);
            --shadow-lg: 0 8px 32px rgba(16, 42, 67, 0.12);
            --shadow-xl: 0 16px 48px rgba(16, 42, 67, 0.16);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        body {
            font-family: var(--font-body);
            color: var(--color-neutral-700);
            line-height: 1.6;
            background-color: var(--color-neutral-100);
            overflow-x: hidden;
        }
        
        /* Typography */
        h1, h2, h3, h4 {
            font-family: var(--font-display);
            color: var(--color-neutral-900);
            line-height: 1.2;
            font-weight: 700;
        }
        
        h1 {
            font-size: clamp(2.5rem, 5vw, 4rem);
            letter-spacing: -0.02em;
        }
        
        h2 {
            font-size: clamp(2rem, 4vw, 3rem);
            letter-spacing: -0.01em;
        }
        
        h3 {
            font-size: clamp(1.5rem, 3vw, 2rem);
        }
        
        p {
            font-size: 1.0625rem;
            margin-bottom: 1rem;
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        /* ========== HEADER CORREGIDO ========== */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.253);
            backdrop-filter: blur(12px);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
        }
        
        .header.scrolled {
            background: rgba(255, 255, 255, 0);
            backdrop-filter: blur(18px);
            box-shadow: var(--shadow-md);
        }
        
        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        /* Logo container CORREGIDO */
        .logo-wrapper {
            display: flex;
            align-items: center;
            gap: 1rem;
        }
        
        .logo {
            display: flex;
            align-items: center;
            animation: logoEntrance 1s ease-out;
        }
        
        .logo img {
            height: auto;
            max-width: 100%;
            object-fit: contain;
            transition: transform 0.3s ease;
        }
        
        .logo:hover img {
            transform: scale(1.05);
        }
        
        @keyframes logoEntrance {
            0% {
                opacity: 0;
                transform: translateY(-20px);
            }
            100% {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        /* Título clínica CORREGIDO */
        .titulo-clinica {
            color: #00a2ff;
            font-family: var(--font-heading);
            font-size: clamp(1.1rem, 1.5vw, 1.5rem);
            font-weight: 600;
            white-space: nowrap;
            margin: 0;
        }
        
        /* Navegación CORREGIDA */
        .nav-menu {
            display: flex;
            flex-direction: row;
            list-style: none;
            gap: 0.6rem;
            align-items: center;
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .nav-menu li {
            transition: all 0.3s ease;
        }
        
        .nav-menu a {
            font-weight: 500;
            color: var(--color-neutral-700);
            transition: all 0.3s ease;
            padding: 0.6rem 1.2rem;
            border-radius: var(--radius-sm);
            background: linear-gradient(135deg, rgba(10, 77, 104, 0.08), rgba(5, 191, 219, 0.08));
            border: 1px solid rgba(10, 77, 104, 0.15);
            display: inline-block;
            backdrop-filter: blur(4px);
            box-shadow: 0 2px 8px rgba(10, 77, 104, 0.08);
            font-size: 0.9rem;
        }
        
        .nav-menu a:hover {
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(10, 77, 104, 0.2);
            border-color: transparent;
        }
        
        /* Botones */
        .btn {
            padding: 0.875rem 2rem;
            border-radius: var(--radius-sm);
            font-weight: 600;
            cursor: pointer;
            border: none;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            font-family: var(--font-body);
            display: inline-flex;
            align-items: center;
            gap: 0.5rem;
            font-size: 1rem;
        }
        
        .btn-primary {
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            color: white;
            box-shadow: var(--shadow-sm);
        }
        
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: var(--shadow-lg);
        }
        
        .btn-secondary {
            background: transparent;
            color: var(--color-primary);
            border: 2px solid var(--color-primary);
        }
        
        .btn-secondary:hover {
            background: var(--color-primary);
            color: white;
        }
        
        /* Mobile Menu Toggle */
        .mobile-toggle {
            display: none;
            flex-direction: column;
            gap: 5px;
            cursor: pointer;
            padding: 8px;
            z-index: 1001;
        }
        
        .mobile-toggle span {
            width: 25px;
            height: 3px;
            background: var(--color-primary);
            border-radius: 2px;
            transition: all 0.3s ease;
        }
        
        .mobile-toggle:hover span {
            background: var(--color-accent);
        }
        
        .mobile-toggle.active span:nth-child(1) {
            transform: rotate(45deg) translate(5px, 5px);
        }
        
        .mobile-toggle.active span:nth-child(2) {
            opacity: 0;
        }
        
        .mobile-toggle.active span:nth-child(3) {
            transform: rotate(-45deg) translate(7px, -6px);
        }
        
        /* Mobile menu overlay */
        .menu-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.5);
            backdrop-filter: blur(4px);
            z-index: 998;
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        
        .menu-overlay.active {
            display: block;
            opacity: 1;
        }
        
        /* Hero Section */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
            padding-top: 100px;
            background: linear-gradient(135deg, #f9fafc 0%, #91c4f8 100%);
        }
        
        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -20%;
            width: 80%;
            height: 150%;
            background: radial-gradient(circle, rgba(5, 191, 219, 0.08) 0%, transparent 70%);
            border-radius: 50%;
            animation: float 20s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translate(0, 0) rotate(0deg); }
            33% { transform: translate(30px, -30px) rotate(5deg); }
            66% { transform: translate(-20px, 20px) rotate(-5deg); }
        }
        
        .hero-container {
            max-width: 1400px;
            margin: 0 auto;
            padding: 0 2rem;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
            position: relative;
            z-index: 1;
        }
        
        .hero-content {
            animation: slideInLeft 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        @keyframes slideInLeft {
            from {
                opacity: 0;
                transform: translateX(-30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .hero-subtitle {
            color: var(--color-accent);
            font-weight: 600;
            font-size: 1.125rem;
            margin-bottom: 1rem;
            letter-spacing: 0.05em;
            text-transform: uppercase;
        }
        
        .hero h1 {
            margin-bottom: 1.5rem;
            background: linear-gradient(135deg, var(--color-neutral-900), var(--color-primary));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
        }
        
        .hero-description {
            font-size: 1.25rem;
            color: var(--color-neutral-700);
            margin-bottom: 2rem;
            line-height: 1.7;
        }
        
        .hero-stats {
            display: flex;
            gap: 2rem;
            margin-top: 3rem;
            flex-wrap: wrap;
        }
        
        .stat-item {
            display: flex;
            align-items: center;
            gap: 0.75rem;
        }
        
        .stat-icon {
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, var(--color-accent), var(--color-primary-light));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.25rem;
        }
        
        .stat-text {
            font-size: 0.875rem;
            color: var(--color-neutral-700);
        }
        
        .stat-number {
            font-weight: 700;
            color: var(--color-neutral-900);
            display: block;
            font-size: 1.125rem;
        }
        
        .hero-buttons {
            display: flex;
            gap: 1rem;
            margin-top: 2.5rem;
            flex-wrap: wrap;
        }
        
        .hero-image {
            position: relative;
            animation: slideInRight 0.8s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        @keyframes slideInRight {
            from {
                opacity: 0;
                transform: translateX(30px);
            }
            to {
                opacity: 1;
                transform: translateX(0);
            }
        }
        
        .hero-image img {
            width: 100%;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-xl);
        }
        
        .floating-card {
            position: absolute;
            background: white;
            padding: 1.5rem;
            border-radius: var(--radius-md);
            box-shadow: var(--shadow-lg);
            animation: floatCard 3s ease-in-out infinite;
            z-index: 10;
        }
        
        @keyframes floatCard {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        
        .card-1 {
            top: 20%;
            left: 5%;
        }
        
        .card-2 {
            bottom: 20%;
            right: 5%;
        }
        
        .card-icon {
            width: 40px;
            height: 40px;
            background: linear-gradient(135deg, var(--color-success), #3AA76D);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            margin-bottom: 0.5rem;
            font-size: 1.25rem;
        }
        
        .card-title {
            font-weight: 600;
            color: var(--color-neutral-900);
            font-size: 0.875rem;
            margin-bottom: 0.25rem;
        }
        
        .card-value {
            color: var(--color-accent);
            font-weight: 700;
            font-size: 1.25rem;
        }
        
        /* Section Styles */
        section {
            padding: var(--spacing-2xl) 2rem;
        }
        
        .section-container {
            max-width: 1400px;
            margin: 0 auto;
        }
        
        .section-header {
            text-align: center;
            margin-bottom: 4rem;
        }
        
        .section-subtitle {
            color: var(--color-accent);
            font-weight: 600;
            font-size: 1rem;
            margin-bottom: 1rem;
            letter-spacing: 0.05em;
            text-transform: uppercase;
        }
        
        .section-title {
            margin-bottom: 1rem;
        }
        
        .section-description {
            font-size: 1.125rem;
            color: var(--color-neutral-700);
            max-width: 700px;
            margin: 0 auto;
        }
        
        /* About Section */
        .about {
            background: white;
        }
        
        .about-content {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
            align-items: center;
        }
        
        .about-text p {
            font-size: 1.125rem;
            margin-bottom: 1.5rem;
        }
        
        .about-features {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .feature-item {
            display: flex;
            align-items: flex-start;
            gap: 1rem;
        }
        
        .feature-icon {
            width: 48px;
            height: 48px;
            background: linear-gradient(135deg, var(--color-accent), var(--color-primary-light));
            border-radius: 12px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            flex-shrink: 0;
        }
        
        .feature-text h4 {
            font-size: 1.125rem;
            margin-bottom: 0.25rem;
            color: var(--color-neutral-900);
        }
        
        .feature-text p {
            font-size: 0.9375rem;
            color: var(--color-neutral-700);
            margin: 0;
        }
        
        .about-image {
            position: relative;
        }
        
        .about-image img {
            width: 100%;
            border-radius: var(--radius-lg);
            box-shadow: var(--shadow-lg);
        }
        
        /* Services Section */
        .services {
            background: var(--color-neutral-100);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 2rem;
        }
        
        .service-card {
            background: white;
            padding: 2.5rem;
            border-radius: var(--radius-md);
            box-shadow: var(--shadow-sm);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }
        
        .service-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 4px;
            background: linear-gradient(90deg, var(--color-accent), var(--color-primary));
            transform: scaleX(0);
            transition: transform 0.4s ease;
        }
        
        .service-card:hover {
            transform: translateY(-8px);
            box-shadow: var(--shadow-lg);
        }
        
        .service-card:hover::before {
            transform: scaleX(1);
        }
        
        .service-icon {
            width: 64px;
            height: 64px;
            background: linear-gradient(135deg, var(--color-accent), var(--color-primary-light));
            border-radius: 16px;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 2rem;
            margin-bottom: 1.5rem;
        }
        
        .service-card h3 {
            font-size: 1.5rem;
            margin-bottom: 1rem;
        }
        
        .service-card p {
            color: var(--color-neutral-700);
            margin-bottom: 1.5rem;
        }
        
        .service-features {
            list-style: none;
            margin-bottom: 1.5rem;
        }
        
        .service-features li {
            padding: 0.5rem 0;
            padding-left: 1.75rem;
            position: relative;
            color: var(--color-neutral-700);
            font-size: 0.9375rem;
        }
        
        .service-features li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--color-success);
            font-weight: 700;
        }
        
        .service-badge {
            display: inline-block;
            padding: 0.5rem 1rem;
            background: linear-gradient(135deg, #FFF4E6, #FFE8CC);
            color: #CC7A00;
            border-radius: var(--radius-sm);
            font-size: 0.875rem;
            font-weight: 600;
            margin-top: 1rem;
        }
        
        /* Utilities */
        .text-center { text-align: center; }
        .mb-1 { margin-bottom: 1rem; }
        .mb-2 { margin-bottom: 2rem; }
        .mt-2 { margin-top: 2rem; }
        
        /* Scroll reveal */
        .reveal {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease-out;
        }
        
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }
        
        /* ========== RESPONSIVE CORREGIDO ========== */
        @media (max-width: 1024px) {
            .titulo-clinica {
                font-size: 1.2rem;
            }
            
            .nav-menu {
                gap: 0.4rem;
            }
            
            .nav-menu a {
                padding: 0.5rem 0.9rem;
                font-size: 0.85rem;
            }
            
            .hero-container,
            .about-content {
                grid-template-columns: 1fr;
            }
            
            .hero-image {
                order: -1;
            }
            
            .floating-card {
                display: none;
            }
        }
        
        @media (max-width: 768px) {
            .nav-menu {
                position: fixed;
                top: 70px;
                right: -100%;
                width: 280px;
                height: calc(100vh - 70px);
                background: rgba(255, 255, 255, 0.98);
                backdrop-filter: blur(20px);
                padding: 2rem;
                flex-direction: column;
                align-items: flex-start;
                gap: 1rem;
                box-shadow: -4px 0 20px rgba(0, 0, 0, 0.1);
                transition: right 0.4s cubic-bezier(0.4, 0, 0.2, 1);
                z-index: 999;
            }
            
            .nav-menu.active {
                right: 0;
            }
            
            .nav-menu a {
                width: 100%;
                text-align: left;
                padding: 1rem 1.5rem;
                font-size: 1rem;
            }
            
            .mobile-toggle {
                display: flex;
            }
        
            .titulo-clinica {
                display: none;
            }
            
            .hero {
                padding-top: 80px;
                min-height: auto;
                padding-bottom: 4rem;
            }
            
            section {
                padding: 4rem 1.5rem;
            }
            
            .about-features,
            .hero-stats {
                grid-template-columns: 1fr;
            }
            
            .hero-buttons {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
        }
        
        @media (max-width: 480px) {
            .logo img {
                width: 140px;
            }
            
            .nav-container {
                padding: 0.75rem 1rem;
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="header" id="header">
        <nav class="nav-container">
            <div class="logo-wrapper">
                <a href="#inicio" class="logo">
                    <img src="gloria-logo.svg" alt="Sanitas Clínicas Dentales">
                </a>
                <p class="titulo-clinica">Clínica Dental</p>
            </div>
            
            <ul class="nav-menu">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#nosotros">Nosotros</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#equipo">Equipo</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
            
            <div class="mobile-toggle">
                <span></span>
                <span></span>
                <span></span>
            </div>
        </nav>
    </header>

    <!-- Mobile Menu Overlay -->
    <div class="menu-overlay"></div>

    <!-- Hero Section -->
    <section class="hero" id="inicio">
        <div class="hero-container">
            <div class="hero-content">
                <div class="hero-subtitle">Bienvenido a Sanitas</div>
                <h1>Cuida tu salud dental con confianza</h1>
                <p class="hero-description">
                    Tratamientos personalizados, tecnología de vanguardia y un equipo que te escucha. 
                    Tu sonrisa es nuestra prioridad.
                </p>
                
                <div class="hero-buttons">
                    <button class="btn btn-primary">📅 Reserva tu cita gratuita</button>
                    <button class="btn btn-secondary">📞 Llámanos ahora</button>
                </div>
                
                <div class="hero-stats">
                    <div class="stat-item">
                        <div class="stat-icon">⭐</div>
                        <div class="stat-text">
                            <span class="stat-number">15+ años</span>
                            de experiencia
                        </div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-icon">😊</div>
                        <div class="stat-text">
                            <span class="stat-number">5,000+</span>
                            pacientes felices
                        </div>
                    </div>
                    <div class="stat-item">
                        <div class="stat-icon">🚨</div>
                        <div class="stat-text">
                            <span class="stat-number">24/7</span>
                            urgencias
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="hero-image">
                <img src="data:image/svg+xml,%3Csvg width='600' height='500' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='600' height='500' fill='%23E8F4F8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' font-family='Arial' font-size='24' fill='%230A4D68' opacity='0.3'%3EEquipo médico profesional%3C/text%3E%3C/svg%3E" alt="Equipo dental profesional">
            </div>
        </div>
        
        <div class="floating-card card-1">
            <div class="card-icon">✓</div>
            <div class="card-title">Primera consulta</div>
            <div class="card-value">Gratis</div>
        </div>
        
        <div class="floating-card card-2">
            <div class="card-icon">⚡</div>
            <div class="card-title">Valoración</div>
            <div class="card-value">4.9/5</div>
        </div>
    </section>

    <!-- About Section -->
    <section class="about" id="nosotros">
        <div class="section-container">
            <div class="about-content">
                <div class="about-text reveal">
                    <div class="section-subtitle">Sobre Nosotros</div>
                    <h2>Conoce a tu nueva clínica dental de confianza</h2>
                    
                    <p>
                        En Sanitas, entendemos que ir al dentista puede generar nerviosismo. Por eso hemos creado 
                        un espacio donde la tecnología más avanzada se combina con un trato cercano y humano.
                    </p>
                    
                    <p>
                        Con más de 15 años cuidando la salud dental de familias como la tuya, nuestro equipo de 
                        especialistas está comprometido con tu bienestar.
                    </p>
                    
                    <div class="about-features">
                        <div class="feature-item">
                            <div class="feature-icon">🏆</div>
                            <div class="feature-text">
                                <h4>Clínica Certificada</h4>
                                <p>Autorizados y regulados</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">💳</div>
                            <div class="feature-text">
                                <h4>Financiación</h4>
                                <p>Hasta 36 meses sin intereses</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">⏰</div>
                            <div class="feature-text">
                                <h4>Horario Flexible</h4>
                                <p>Adaptado a ti</p>
                            </div>
                        </div>
                        <div class="feature-item">
                            <div class="feature-icon">🛡️</div>
                            <div class="feature-text">
                                <h4>Garantía Total</h4>
                                <p>En todos nuestros tratamientos</p>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="about-image reveal">
                    <img src="data:image/svg+xml,%3Csvg width='600' height='600' xmlns='http://www.w3.org/2000/svg'%3E%3Crect width='600' height='600' fill='%23F0F4F8'/%3E%3Ctext x='50%25' y='50%25' text-anchor='middle' dy='.3em' font-family='Arial' font-size='20' fill='%230A4D68' opacity='0.3'%3EClínica moderna y equipada%3C/text%3E%3C/svg%3E" alt="Instalaciones modernas">
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="servicios">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Nuestros Servicios</div>
                <h2>Soluciones completas para tu salud dental</h2>
                <p class="section-description">
                    Desde cuidado preventivo hasta tratamientos especializados, todo en un solo lugar
                </p>
            </div>
            
            <div class="services-grid">
                <div class="service-card reveal">
                    <div class="service-icon">🦷</div>
                    <h3>Odontología General</h3>
                    <p>Cuidado dental completo para toda la familia</p>
                    <ul class="service-features">
                        <li>Revisiones y diagnóstico</li>
                        <li>Limpiezas dentales profundas</li>
                        <li>Obturaciones (empastes)</li>
                        <li>Endodoncias</li>
                    </ul>
                </div>
                
                <div class="service-card reveal">
                    <div class="service-icon">🔧</div>
                    <h3>Implantes Dentales</h3>
                    <p>Recupera tu sonrisa de forma permanente</p>
                    <ul class="service-features">
                        <li>Implantes de titanio biocompatible</li>
                        <li>Cirugía guiada por ordenador</li>
                        <li>Coronas sobre implantes</li>
                        <li>Prótesis fijas completas</li>
                    </ul>
                    <span class="service-badge">Garantía de 10 años</span>
                </div>
                
                <div class="service-card reveal">
                    <div class="service-icon">😁</div>
                    <h3>Ortodoncia</h3>
                    <p>Alinea tu sonrisa con la técnica que prefieras</p>
                    <ul class="service-features">
                        <li>Ortodoncia invisible (Invisalign)</li>
                        <li>Brackets metálicos y estéticos</li>
                        <li>Ortodoncia lingual</li>
                        <li>Retenedores personalizados</li>
                    </ul>
                    <span class="service-badge">Primera consulta gratis</span>
                </div>
                
                <div class="service-card reveal">
                    <div class="service-icon">✨</div>
                    <h3>Estética Dental</h3>
                    <p>La sonrisa que siempre soñaste</p>
                    <ul class="service-features">
                        <li>Blanqueamiento profesional</li>
                        <li>Carillas de porcelana</li>
                        <li>Diseño digital de sonrisa (DSD)</li>
                        <li>Reconstrucciones estéticas</li>
                    </ul>
                </div>
                
                <div class="service-card reveal">
                    <div class="service-icon">💊</div>
                    <h3>Periodoncia</h3>
                    <p>Encías sanas, sonrisa duradera</p>
                    <ul class="service-features">
                        <li>Tratamiento de gingivitis</li>
                        <li>Curetajes y raspados</li>
                        <li>Cirugía periodontal</li>
                        <li>Mantenimiento preventivo</li>
                    </ul>
                </div>
                
                <div class="service-card reveal">
                    <div class="service-icon">🚨</div>
                    <h3>Urgencias Dentales</h3>
                    <p>Atención inmediata cuando más lo necesitas</p>
                    <ul class="service-features">
                        <li>Atención en 24 horas</li>
                        <li>Tratamiento del dolor</li>
                        <li>Reparación de fracturas</li>
                        <li>Infecciones dentales</li>
                    </ul>
                    <span class="service-badge">Disponible 24/7</span>
                </div>
            </div>
        </div>
    </section>

    <script>
        // Header scroll effect
        window.addEventListener('scroll', () => {
            const header = document.getElementById('header');
            if (window.scrollY > 50) {
                header.classList.add('scrolled');
            } else {
                header.classList.remove('scrolled');
            }
        });

        // Mobile menu toggle
        const mobileToggle = document.querySelector('.mobile-toggle');
        const navMenu = document.querySelector('.nav-menu');
        const menuOverlay = document.querySelector('.menu-overlay');
        
        mobileToggle.addEventListener('click', () => {
            mobileToggle.classList.toggle('active');
            navMenu.classList.toggle('active');
            menuOverlay.classList.toggle('active');
            document.body.style.overflow = navMenu.classList.contains('active') ? 'hidden' : '';
        });
        
        // Close menu when clicking on a link
        const navLinks = document.querySelectorAll('.nav-menu a');
        navLinks.forEach(link => {
            link.addEventListener('click', () => {
                mobileToggle.classList.remove('active');
                navMenu.classList.remove('active');
                menuOverlay.classList.remove('active');
                document.body.style.overflow = '';
            });
        });
        
        // Close menu when clicking on overlay
        menuOverlay.addEventListener('click', () => {
            mobileToggle.classList.remove('active');
            navMenu.classList.remove('active');
            menuOverlay.classList.remove('active');
            document.body.style.overflow = '';
        });

        // Scroll Reveal Animation
        const revealElements = document.querySelectorAll('.reveal');
        
        const revealOnScroll = () => {
            const windowHeight = window.innerHeight;
            
            revealElements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const revealPoint = 100;
                
                if (elementTop < windowHeight - revealPoint) {
                    element.classList.add('active');
                }
            });
        };

        window.addEventListener('scroll', revealOnScroll);
        revealOnScroll();

        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });
    </script>
</body>
</html>


