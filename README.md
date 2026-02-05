
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gloria - Tu Clínica Dental de Confianza</title>
    <meta name="description" content="Clínica dental Gloria con más de 15 años de experiencia. Implantes, ortodoncia invisible, estética dental y urgencias 24/7. Primera consulta gratuita.">
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;600;700&family=DM+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">

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
        
        /* Header & Navigation */
        .header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0);
            backdrop-filter: blur(18px);
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .header.scrolled {
            box-shadow: var(--shadow-md);
            background: rgba(255, 255, 255, 0);
            backdrop-filter: blur(18px);
        }
        .titulo-clinica {
            color: #00a2ff8e; /* elige el color que quieras */
            position: relative; top: 35px; /* subir */ /* top: 15px; bajar */
            position: relative; left: -80px; /* mueve a la derecha */ /* left: -20px; mueve a la izquierda */
    font-family: "Poppins", sans-serif;
    font-size: 28px;
    font-weight: 600;
}

        
        .nav-container {
            max-width: 1400px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
            padding: 1.25rem 2rem .5rem 2rem;
        }
        
        .header.scrolled .nav-container {
            align-items: center;
        }
        
        .logo {
            background: transparent;
            display: flex;
            align-items: center;
            animation: logoEntrance 1s ease-out;
        }
        
        .logo img {
            height: auto;
            width: 280px;
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
        
        /* Responsive logo */
        @media (max-width: 1024px) {
            .logo img {
                height: 180px;
            }
        }
        
        @media (max-width: 768px) {
            .logo img {
                height: auto;
                max-width: 180px;
            }
        }
        
        @media (max-width: 768px) {
            .logo img {
                height: auto;
                max-width: 120px;
            }
        }
        
        .nav-menu {
            display: flex;
            flex-direction: column;
            list-style: none;
            gap: 0.75rem;
            align-items: flex-end;
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
        }
        
        .header.scrolled .nav-menu {
            flex-direction: row;
            gap: 0.5rem;
        }
        
        .nav-menu li {
            transition: all 0.3s ease;
        }
        
        .nav-menu a {
            font-weight: 500;
            color: var(--color-neutral-700);
            transition: all 0.3s ease;
            position: relative;
            padding: 0.75rem 1.5rem;
            border-radius: var(--radius-sm);
            background: linear-gradient(135deg, rgba(10, 77, 104, 0.08), rgba(5, 191, 219, 0.08));
            border: 1px solid rgba(10, 77, 104, 0.15);
            display: inline-block;
            backdrop-filter: blur(4px);
            box-shadow: 0 2px 8px rgba(10, 77, 104, 0.08);
        }
        
        .header.scrolled .nav-menu a {
            padding: 0.5rem 1rem;
            font-size: 0.875rem;
            background: rgba(255, 255, 255, 0.6);
            backdrop-filter: blur(8px);
            border: 1px solid rgba(10, 77, 104, 0.1);
            box-shadow: 0 2px 4px rgba(10, 77, 104, 0.05);
        }
        
        .nav-menu a:hover {
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(10, 77, 104, 0.2);
            border-color: transparent;
        }
        
        .header.scrolled .nav-menu a:hover {
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            color: white;
            transform: translateY(-2px);
            box-shadow: 0 4px 12px rgba(10, 77, 104, 0.25);
        }
        
        .nav-menu a::after {
            display: none;
        }
        
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
            position: relative;
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
            padding-top: 80px;
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
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
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
        
        /* Team Section */
        .team {
            background: white;
        }
        
        .team-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2.5rem;
        }
        
        .team-member {
            text-align: center;
            transition: transform 0.3s ease;
        }
        
        .team-member:hover {
            transform: scale(1.02);
        }
        
        .member-photo {
            width: 220px;
            height: 220px;
            border-radius: 50%;
            margin: 0 auto 1.5rem;
            background: linear-gradient(135deg, var(--color-neutral-200), var(--color-neutral-300));
            box-shadow: var(--shadow-md);
            overflow: hidden;
            position: relative;
        }
        
        .member-photo img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        .member-photo::after {
            content: '👨‍⚕️';
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            font-size: 5rem;
            opacity: 0.3;
        }
        
        .team-member h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }
        
        .member-role {
            color: var(--color-accent);
            font-weight: 600;
            margin-bottom: 1rem;
        }
        
        .member-bio {
            color: var(--color-neutral-700);
            margin-bottom: 1rem;
            line-height: 1.7;
        }
        
        .member-credentials {
            font-size: 0.875rem;
            color: var(--color-neutral-700);
            opacity: 0.8;
        }
        
        /* Technology Section */
        .technology {
            background: var(--color-primary);
            color: white;
        }
        
        .technology .section-subtitle {
            color: var(--color-accent);
        }
        
        .technology .section-title,
        .technology .section-description {
            color: white;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }
        
        .tech-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
            padding: 2rem;
            border-radius: var(--radius-md);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.3s ease;
        }
        
        .tech-card:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateY(-4px);
        }
        
        .tech-icon {
            width: 56px;
            height: 56px;
            background: rgba(255, 255, 255, 0.2);
            border-radius: 14px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.75rem;
            margin-bottom: 1.5rem;
        }
        
        .tech-card h3 {
            color: white;
            font-size: 1.25rem;
            margin-bottom: 0.75rem;
        }
        
        .tech-benefit {
            color: var(--color-accent);
            font-weight: 600;
            margin-bottom: 0.75rem;
            font-size: 0.9375rem;
        }
        
        .tech-card p {
            color: rgba(255, 255, 255, 0.9);
            font-size: 0.9375rem;
        }
        
        /* Testimonials Section */
        .testimonials {
            background: var(--color-neutral-100);
        }
        
        .testimonials-slider {
            position: relative;
            overflow: hidden;
            padding: 2rem 0;
        }
        
        .testimonials-track {
            display: flex;
            gap: 2rem;
            transition: transform 0.5s ease;
        }
        
        .testimonial-card {
            min-width: 400px;
            background: white;
            padding: 2.5rem;
            border-radius: var(--radius-md);
            box-shadow: var(--shadow-md);
            flex-shrink: 0;
        }
        
        .testimonial-header {
            display: flex;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1.5rem;
        }
        
        .testimonial-avatar {
            width: 64px;
            height: 64px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--color-accent), var(--color-primary-light));
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.75rem;
            font-weight: 700;
        }
        
        .testimonial-info h4 {
            font-size: 1.125rem;
            margin-bottom: 0.25rem;
        }
        
        .testimonial-treatment {
            color: var(--color-accent);
            font-size: 0.875rem;
        }
        
        .testimonial-rating {
            color: #FFB84D;
            font-size: 1.25rem;
            margin-bottom: 1rem;
        }
        
        .testimonial-text {
            color: var(--color-neutral-700);
            line-height: 1.8;
            font-style: italic;
        }
        
        .slider-controls {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin-top: 2rem;
        }
        
        .slider-btn {
            width: 48px;
            height: 48px;
            border-radius: 50%;
            background: white;
            border: 2px solid var(--color-primary);
            color: var(--color-primary);
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .slider-btn:hover {
            background: var(--color-primary);
            color: white;
        }
        
        /* FAQ Section */
        .faq {
            background: white;
        }
        
        .faq-container {
            max-width: 900px;
            margin: 0 auto;
        }
        
        .faq-item {
            margin-bottom: 1rem;
            background: var(--color-neutral-100);
            border-radius: var(--radius-md);
            overflow: hidden;
            transition: all 0.3s ease;
        }
        
        .faq-question {
            padding: 1.75rem 2rem;
            cursor: pointer;
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 600;
            color: var(--color-neutral-900);
            font-size: 1.125rem;
            transition: all 0.3s ease;
        }
        
        .faq-question:hover {
            background: var(--color-neutral-200);
        }
        
        .faq-icon {
            font-size: 1.5rem;
            color: var(--color-primary);
            transition: transform 0.3s ease;
        }
        
        .faq-item.active .faq-icon {
            transform: rotate(45deg);
        }
        
        .faq-answer {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.4s ease, padding 0.4s ease;
        }
        
        .faq-item.active .faq-answer {
            max-height: 500px;
            padding: 0 2rem 1.75rem;
        }
        
        .faq-answer p {
            color: var(--color-neutral-700);
            line-height: 1.7;
        }
        
        /* CTA Section */
        .cta {
            background: linear-gradient(135deg, var(--color-primary), var(--color-primary-light));
            color: white;
            text-align: center;
        }
        
        .cta-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .cta h2 {
            color: white;
            margin-bottom: 1.5rem;
        }
        
        .cta p {
            font-size: 1.25rem;
            margin-bottom: 2.5rem;
            opacity: 0.95;
        }
        
        .cta-badges {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin-top: 3rem;
            flex-wrap: wrap;
        }
        
        .cta-badge {
            display: flex;
            align-items: center;
            gap: 0.75rem;
            background: rgba(255, 255, 255, 0.15);
            padding: 1rem 1.5rem;
            border-radius: var(--radius-sm);
        }
        
        .cta-badge-icon {
            font-size: 1.5rem;
        }
        
        /* Contact Section */
        .contact {
            background: white;
        }
        
        .contact-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 4rem;
        }
        
        .contact-info h3 {
            font-size: 1.75rem;
            margin-bottom: 2rem;
        }
        
        .info-item {
            display: flex;
            gap: 1.5rem;
            margin-bottom: 2rem;
        }
        
        .info-icon {
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
        
        .info-text h4 {
            font-size: 1rem;
            margin-bottom: 0.5rem;
            color: var(--color-neutral-900);
        }
        
        .info-text p {
            color: var(--color-neutral-700);
            margin: 0;
        }
        
        .info-text a {
            color: var(--color-primary);
            font-weight: 600;
        }
        
        .contact-form {
            background: var(--color-neutral-100);
            padding: 2.5rem;
            border-radius: var(--radius-md);
        }
        
        .form-group {
            margin-bottom: 1.5rem;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
            color: var(--color-neutral-900);
        }
        
        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 1rem;
            border: 2px solid var(--color-neutral-300);
            border-radius: var(--radius-sm);
            font-family: var(--font-body);
            font-size: 1rem;
            transition: all 0.3s ease;
        }
        
        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            outline: none;
            border-color: var(--color-primary);
            box-shadow: 0 0 0 3px rgba(10, 77, 104, 0.1);
        }
        
        .form-group textarea {
            resize: vertical;
            min-height: 120px;
        }
        
        .form-checkbox {
            display: flex;
            gap: 0.75rem;
            align-items: flex-start;
        }
        
        .form-checkbox input {
            margin-top: 4px;
            width: auto;
        }
        
        .form-checkbox label {
            font-weight: 400;
            font-size: 0.875rem;
        }
        
        /* Footer */
        .footer {
            background: var(--color-neutral-900);
            color: rgba(255, 255, 255, 0.8);
            padding: 4rem 2rem 2rem;
        }
        
        .footer-grid {
            max-width: 1400px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 3rem;
            margin-bottom: 3rem;
        }
        
        .footer-section h4 {
            color: white;
            font-size: 1.25rem;
            margin-bottom: 1.5rem;
        }
        
        .footer-section p {
            font-size: 0.9375rem;
            margin-bottom: 1rem;
            line-height: 1.6;
        }
        
        .footer-links {
            list-style: none;
        }
        
        .footer-links li {
            margin-bottom: 0.75rem;
        }
        
        .footer-links a {
            color: rgba(255, 255, 255, 0.8);
            transition: color 0.3s ease;
        }
        
        .footer-links a:hover {
            color: var(--color-accent);
        }
        
        .social-links {
            display: flex;
            gap: 1rem;
            margin-top: 1.5rem;
        }
        
        .social-icon {
            width: 40px;
            height: 40px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
            font-size: 1.25rem;
        }
        
        .social-icon:hover {
            background: var(--color-accent);
            transform: translateY(-3px);
        }
        
        .footer-bottom {
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            padding-top: 2rem;
            text-align: center;
            font-size: 0.875rem;
            max-width: 1400px;
            margin: 0 auto;
        }
        
        /* Utilities */
        .text-center { text-align: center; }
        .mb-1 { margin-bottom: 1rem; }
        .mb-2 { margin-bottom: 2rem; }
        .mt-2 { margin-top: 2rem; }
        
        /* Responsive */
        @media (max-width: 1024px) {
            .hero-container,
            .about-content,
            .contact-grid {
                grid-template-columns: 1fr;
            }
            
            .hero-image {
                order: -1;
            }
            
            .services-grid {
                grid-template-columns: 1fr;
            }
            
            .testimonial-card {
                min-width: 350px;
            }
            
            .floating-card {
                display: none;
            }
        }
        
        @media (max-width: 768px) {
            .nav-menu {
                position: fixed;
                top: 80px;
                right: -100%;
                width: 280px;
                height: calc(100vh - 80px);
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
            
            .header.scrolled .nav-menu {
                flex-direction: column;
                gap: 1rem;
            }
            
            .header.scrolled .nav-menu a {
                padding: 1rem 1.5rem;
                font-size: 1rem;
                width: 100%;
            }
            
            .mobile-toggle {
                display: flex;
                cursor: pointer;
                z-index: 1000;
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
            
            .hero {
                min-height: auto;
                padding: 6rem 0 4rem;
            }
            
            section {
                padding: 4rem 1.5rem;
            }
            
            .about-features,
            .hero-stats {
                grid-template-columns: 1fr;
            }
            
            .testimonial-card {
                min-width: 300px;
            }
            
            .footer-grid {
                grid-template-columns: 1fr;
                gap: 2rem;
            }
            
            .hero-buttons {
                flex-direction: column;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
        }
        
        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }
        
        .fade-in-up {
            animation: fadeInUp 0.6s ease-out;
        }
        
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
        .logo-wrapper {
    display: flex;
    align-items: center;
    gap: 1rem;
}

.logo svg {
    width: 150px;
    height: auto;
}

    </style>
</head>
<body>
    <!-- Header -->
    <header class="header" id="header">
        <nav class="nav-container">
            <div class="logo-wrapper">
            <a href="#inicio" class="logo">
    
<svg width="300.58136mm" height="144.21629mm" inkscape:version="1.3.2 (091e20e, 2023-11-25, custom)" sodipodi:docname="A,SyGloria300.svg" version="1.1" viewBox="0 0 300.58136 144.21629" xmlns="http://www.w3.org/2000/svg" xmlns:inkscape="http://www.inkscape.org/namespaces/inkscape" xmlns:sodipodi="http://sodipodi.sourceforge.net/DTD/sodipodi-0.dtd" xmlns:xlink="http://www.w3.org/1999/xlink">
<sodipodi:namedview bordercolor="#000000" borderopacity="0.25" inkscape:current-layer="layer1" inkscape:cx="565.57692" inkscape:cy="296.80703" inkscape:deskcolor="#d1d1d1" inkscape:document-units="mm" inkscape:pagecheckerboard="0" inkscape:pageopacity="0.0" inkscape:showpageshadow="2" inkscape:window-height="1017" inkscape:window-maximized="1" inkscape:window-width="1920" inkscape:window-x="-8" inkscape:window-y="-8" inkscape:zoom="0.51717104" pagecolor="#ffffff"/>
<defs>
<linearGradient x1="79.385048" x2="1543.7415" y1="424.87003" y2="424.87003" gradientUnits="userSpaceOnUse">
<stop offset="0"/>
<stop stop-opacity="0" offset="1"/>
</linearGradient>
<linearGradient x1="80.703011" x2="643.63751" y1="424.86765" y2="420.2865" gradientTransform="translate(-155.607,-680.49032)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient id="linearGradient3">
<stop stop-color="#00b8e1" offset="0"/>
<stop stop-color="#00b8e1" stop-opacity="0" offset="1"/>
</linearGradient>
<linearGradient x1="273.45444" x2="567.8078" y1="442.61176" y2="442.61176" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse">
<stop stop-opacity="0" offset="0"/>
<stop stop-color="#007c97" stop-opacity=".94117647" offset="1"/>
</linearGradient>
<linearGradient x1="689.62054" x2="986.24384" y1="448.20474" y2="448.26901" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="689.62054" x2="968.48035" y1="448.20474" y2="448.20474" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse">
<stop stop-opacity="0" offset="0"/>
<stop stop-color="#007d97" offset="1"/>
</linearGradient>
<linearGradient x1="555.65271" x2="714.49695" y1="383.79941" y2="383.23587" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="555.65271" x2="727.77161" y1="383.79941" y2="383.79941" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse">
<stop stop-opacity="0" offset="0"/>
<stop stop-color="#007d97" stop-opacity=".94509804" offset="1"/>
</linearGradient>
<linearGradient x1="950.18274" x2="1186.9813" y1="452.7973" y2="445.94653" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="950.18274" x2="1191.2963" y1="452.7973" y2="452.7973" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient>
<stop stop-opacity="0" offset="0"/>
<stop stop-color="#007c97" offset="1"/>
</linearGradient>
<linearGradient x1="1170.8168" x2="1314.8687" y1="452.26401" y2="453.57938" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="1170.8168" x2="1306.6501" y1="452.26401" y2="452.26401" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="1177.944" x2="1334.4293" y1="292.8754" y2="292.8754" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="1177.944" x2="1319.649" y1="292.8754" y2="292.8754" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="1342.7385" x2="1557.657" y1="451.2569" y2="454.64105" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient x1="1302.6755" x2="1542.4299" y1="452.99878" y2="452.99878" gradientTransform="translate(-132.38208,-678.16783)" gradientUnits="userSpaceOnUse" xlink:href="#linearGradient3"/>
<linearGradient>
<stop stop-opacity="0" offset="0"/>
<stop stop-color="#0084a0" offset="1"/>
</linearGradient>
</defs>
<g transform="translate(-71.452842,66.382215)" inkscape:groupmode="layer" inkscape:label="Capa 1">
<g transform="matrix(.20297656 0 0 .26052706 85.459424 65.810558)" fill="#00d3fc" fill-rule="evenodd" stroke="#000" stroke-linecap="round" stroke-width="3.65145">
<path d="m443.62492-502.42057c-902.89962-52.84193-377.776466 579.174673-162.52472 333.83583-66.84103 238.635613-295.040016 118.723413-279.8771959 10.52537-32.1697901-10.7726-54.3407561-24.57436-64.9603501-33.03957 13.047104 290.389533 457.752986 232.420623 472.913396 227.516623 101.4785-32.8256803-38.17509-163.341373-38.23041-311.572603-8e-3 -18.39389 3.56835-26.95166 33.30628-33.25227l-225.36072 0.66213c19.84214 3.61011 78.21337 10.4945 83.72403 26.69849 3.46809 10.19784 2.60983 24.29681 3.50485 36.88997 1.9712 41.79109-7.56897 68.40504-36.63461 75.9243-268.176532 69.377063-37.23497-351.64894 121.31064-186.14297 5.16097-90.20692 46.03299-118.86834 92.82881-148.0453z"/>
<path d="m695.95588-326.45714c-179.99824-1.43625-190.25862 190.3942 1.19692 192.97381 178.87592 2.41013 191.94962-191.43264-1.19692-192.97381zm-6.04503 18.37112c104.13608-1.88393 101.53929 157.72926 3.89684 153.94843-102.93805-3.98588-95.37572-152.29347-3.89684-153.94843z"/>
<path d="m423.27063-126.32109c14.79644-3.22894 31.78474-6.9362 34.84647-44.1199 3.06174-37.18372-5.22693-128.77458 4.1005-185.71394 9.32741-56.93933 31.5531-77.63809 58.15989-91.05833 26.6068-13.42027 50.0563-15.12767 75.01202-16.94474-20.13585 5.87306-40.27169 11.74612-50.51378 55.77028-10.24208 44.02419-10.59043 126.19773-11.23381 178.9252-0.54073 44.31745-3.03625 66.34491 0.12562 78.06302 2.87536 10.65634 31.96882 27.93249 49.4245-2.65296l-2.70903 29.47365z"/>
<path d="m843.09288-323.39262c35.19504 0.19967 70.39004 0.39934 105.58504 0.599-8.4312 3.56983-13.8573 6.82416-15.621 14.02477-0.7927 3.53224-1.2153 7.49301-2.3305 10.83381 57-54.28177 140.97778-17.23291 126.54748 13.62733-8.2205 17.57997-54.8868 34.2108-97.08728 23.361 0 0 2.9097-0.86078 6.7895-2.27051 51.59548-18.7472 43.87558-43.37451 25.7129-48.09777-24.9315 1.14772-56.1977 23.67208-58.8735 31.97025-4.6528 14.42924-3.7979 118.17383-3.9608 134.47233 1.0438 14.50113 13.7765 17.05696 23.7793 19.03089-44.2378 0.53044-91.59571 0.18799-135.83339 0.71843 11.70607-4.73527 31.12171-1.28656 35.02996-20.68621 5.23248-45.90298 6.4074-109.9283 8.81977-158.37979 0.75964-15.25711-11.35392-14.96436-18.55748-19.20353z"/>
<path d="m1063.727-325.0386c35.195 0.19967 70.39 0.39934 105.585 0.599-8.4312 3.56982-15.0268 6.71836-15.621 14.02477-4.337 53.32844-6.4583 109.41435-7.1024 163.89644 1.0437 14.50112 17.6768 17.05696 27.6795 19.03089-44.2377 0.53044-91.5957 0.18799-135.8334 0.71843 11.7061-4.73527 31.1218-1.28657 35.03-20.68621 5.2325-45.903 6.4074-109.9283 8.8198-158.3798 0.7596-15.2571-11.3539-14.96435-18.5575-19.20352z"/>
<path d="m1115.4623-407.42388c66.2064-63.10161 121.3766 16.8241 0 67.50514-110.1581-43.21931-74.5584-128.92809 0-67.50514z"/>
<path d="m1235.722-319.45291c-62.5598 18.09297-38.0755 57.41593-34.4373 58.9482 14.2236 5.99049 46.9946-2.12241 51.5334-3.37397 12.0476-3.32216-14.3439-39.1441 22.3598-50.09573 42.5287-12.68966 71.5423 16.63312 51.8746 46.75006-14.6496 22.43285-79.307 8.38927-129.8142 43.45068-72.8524 50.57324 15.0765 138.497423 108.6883 76.52701 7.8137-5.17261 14.5612-12.65849 16.5764-14.69526 2.2728-2.2972-0.1479 14.81728-2.7337 25.81922-2.405 10.23195-26.2381 10.93534-19.0416 11.0361 45.3806 0.63538 63.42 1.12883 108.8814 2.13444 2.6194 0.058-7.2149-5.81955-10.3352-7.80789-11.8908-7.57717-0.5657-80.72632-3.4437-139.52062-0.9079-18.54758-6.6178-39.74465-43.0988-49.95044-33.6582-9.41608-79.7138-9.92316-117.0094 0.7782zm95.033 72.82243c-1.003 18.84554-6.2359 66.36275-7.6378 68.03103-57.0117 67.8449-108.8523-8.13858-50.2952-47.75437 14.7183-9.28618 33.2928-15.35615 51.3-20.17779 4.0655-0.97559 6.691-1.18959 6.633-0.0988z"/>
</g>
</g>
</svg>
</a>

            </div>
            <ul class="nav-menu">
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#nosotros">Nosotros</a></li>
                <li><a href="#servicios">Servicios</a></li>
                <li><a href="#equipo">Equipo</a></li>
                <li><a href="#testimonios">Opiniones</a></li>
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
                <div class="hero-subtitle">Bienvenido a Gloria</div>
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
                        En Gloria, entendemos que ir al dentista puede generar nerviosismo. Por eso hemos creado 
                        un espacio donde la tecnología más avanzada se combina con un trato cercano y humano.
                    </p>
                    
                    <p>
                        Con más de 15 años cuidando la salud dental de familias como la tuya, nuestro equipo de 
                        especialistas está comprometido con tu bienestar. Desde una simple limpieza hasta tratamientos 
                        complejos de implantología, cada procedimiento lo realizamos con la máxima precisión y dedicación.
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

    <!-- Team Section -->
    <section class="team" id="equipo">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Nuestro Equipo</div>
                <h2>Conoce al equipo que cuidará de tu sonrisa</h2>
                <p class="section-description">
                    Odontólogos especializados con formación continua y años de experiencia
                </p>
            </div>
            
            <div class="team-grid">
                <div class="team-member reveal">
                    <div class="member-photo">
                        <!-- Placeholder for doctor photo -->
                    </div>
                    <h3>Dra. María González</h3>
                    <p class="member-role">Directora Médica - Implantología</p>
                    <p class="member-bio">
                        Más de 20 años de experiencia en implantología avanzada. Formada en la Universidad 
                        Complutense y con certificaciones internacionales en técnicas de regeneración ósea.
                    </p>
                    <p class="member-credentials">Máster en Implantología | Miembro SEPA</p>
                </div>
                
                <div class="team-member reveal">
                    <div class="member-photo">
                        <!-- Placeholder for doctor photo -->
                    </div>
                    <h3>Dr. Carlos Martínez</h3>
                    <p class="member-role">Ortodoncista</p>
                    <p class="member-bio">
                        Especialista certificado en Invisalign® Platinum. Apasionado por transformar sonrisas 
                        combinando técnicas tradicionales con la última tecnología digital.
                    </p>
                    <p class="member-credentials">Especialista en Ortodoncia | Invisalign Platinum</p>
                </div>
                
                <div class="team-member reveal">
                    <div class="member-photo">
                        <!-- Placeholder for doctor photo -->
                    </div>
                    <h3>Dra. Laura Fernández</h3>
                    <p class="member-role">Odontopediatra</p>
                    <p class="member-bio">
                        Crear experiencias positivas en los más pequeños es su vocación. Con paciencia y 
                        técnicas adaptadas a cada edad, ayuda a que los niños crezcan sin miedo al dentista.
                    </p>
                    <p class="member-credentials">Especialista en Odontopediatría | Máster UB</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Technology Section -->
    <section class="technology">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Tecnología</div>
                <h2>Tecnología de vanguardia al servicio de tu salud</h2>
                <p class="section-description">
                    Invertimos en los equipos más avanzados para diagnósticos precisos y tratamientos mínimamente invasivos
                </p>
            </div>
            
            <div class="tech-grid">
                <div class="tech-card reveal">
                    <div class="tech-icon">📷</div>
                    <h3>Escáner Intraoral 3D</h3>
                    <p class="tech-benefit">Adiós a las molestas impresiones tradicionales</p>
                    <p>
                        Obtenemos modelos digitales precisos de tu boca en segundos, sin pastas ni moldes incómodos. 
                        Mayor precisión y comodidad para ti.
                    </p>
                </div>
                
                <div class="tech-card reveal">
                    <div class="tech-icon">🖼️</div>
                    <h3>Radiografía Digital</h3>
                    <p class="tech-benefit">90% menos radiación que sistemas convencionales</p>
                    <p>
                        Imágenes de alta resolución al instante con la mínima exposición. Diagnósticos más 
                        precisos y seguros para toda la familia.
                    </p>
                </div>
                
                <div class="tech-card reveal">
                    <div class="tech-icon">😌</div>
                    <h3>Sedación Consciente</h3>
                    <p class="tech-benefit">Tratamientos sin ansiedad ni miedo</p>
                    <p>
                        Para procedimientos largos o pacientes con fobia dental, ofrecemos sedación segura 
                        que te permite estar relajado mientras trabajamos.
                    </p>
                </div>
                
                <div class="tech-card reveal">
                    <div class="tech-icon">💻</div>
                    <h3>Cirugía Guiada por Ordenador</h3>
                    <p class="tech-benefit">Precisión milimétrica en implantes</p>
                    <p>
                        Planificamos cada implante digitalmente antes de la cirugía, garantizando resultados 
                        predecibles y tiempos de recuperación más cortos.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials" id="testimonios">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Testimonios</div>
                <h2>Lo que dicen nuestros pacientes</h2>
                <p class="section-description">
                    Miles de sonrisas recuperadas y opiniones reales que nos llenan de orgullo
                </p>
            </div>
            
            <div class="testimonials-slider">
                <div class="testimonials-track" id="testimonials-track">
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">ML</div>
                            <div class="testimonial-info">
                                <h4>María López</h4>
                                <p class="testimonial-treatment">Implante dental</p>
                            </div>
                        </div>
                        <div class="testimonial-rating">⭐⭐⭐⭐⭐</div>
                        <p class="testimonial-text">
                            "Después de años ocultando mi sonrisa por un diente perdido, finalmente di el paso. 
                            El equipo me explicó todo con una paciencia increíble. Hoy, tres meses después, no 
                            puedo estar más feliz con el resultado."
                        </p>
                    </div>
                    
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">CJ</div>
                            <div class="testimonial-info">
                                <h4>Carlos Jiménez</h4>
                                <p class="testimonial-treatment">Ortodoncia invisible</p>
                            </div>
                        </div>
                        <div class="testimonial-rating">⭐⭐⭐⭐⭐</div>
                        <p class="testimonial-text">
                            "Trabajo de cara al público y necesitaba algo discreto. Invisalign fue la solución perfecta. 
                            En 14 meses mi sonrisa cambió por completo y nadie notó que llevaba ortodoncia."
                        </p>
                    </div>
                    
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">AM</div>
                            <div class="testimonial-info">
                                <h4>Ana Martínez</h4>
                                <p class="testimonial-treatment">Odontología familiar</p>
                            </div>
                        </div>
                        <div class="testimonial-rating">⭐⭐⭐⭐⭐</div>
                        <p class="testimonial-text">
                            "Toda mi familia viene aquí desde hace 5 años. Con los niños son súper pacientes y 
                            cariñosos. Mi hija de 6 años ya no tiene miedo al dentista, ¡hasta le gusta venir!"
                        </p>
                    </div>
                    
                    <div class="testimonial-card">
                        <div class="testimonial-header">
                            <div class="testimonial-avatar">RS</div>
                            <div class="testimonial-info">
                                <h4>Roberto Sánchez</h4>
                                <p class="testimonial-treatment">Urgencia dental</p>
                            </div>
                        </div>
                        <div class="testimonial-rating">⭐⭐⭐⭐⭐</div>
                        <p class="testimonial-text">
                            "Un sábado por la noche tuve un dolor terrible. Llamé al número de urgencias y en 
                            menos de una hora me estaban atendiendo. Profesionalidad total."
                        </p>
                    </div>
                </div>
            </div>
            
            <div class="slider-controls">
                <button class="slider-btn" id="prev-btn">←</button>
                <button class="slider-btn" id="next-btn">→</button>
            </div>
        </div>
    </section>

    <!-- FAQ Section -->
    <section class="faq">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Preguntas Frecuentes</div>
                <h2>Resuelve tus dudas</h2>
                <p class="section-description">
                    Las preguntas más comunes sobre nuestros tratamientos y servicios
                </p>
            </div>
            
            <div class="faq-container">
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿La primera consulta es gratuita?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Sí, tu primera visita incluye revisión completa, diagnóstico y plan de tratamiento 
                            personalizado sin coste. Solo pagas si decides iniciar algún tratamiento.
                        </p>
                    </div>
                </div>
                
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿Ofrecen facilidades de pago?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Por supuesto. Trabajamos con financiación hasta 36 meses sin intereses y aceptamos 
                            todas las formas de pago. Nuestro equipo te explicará las opciones que mejor se 
                            adapten a tu presupuesto.
                        </p>
                    </div>
                </div>
                
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿Aceptan seguros dentales?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Sí, trabajamos con las principales compañías aseguradoras. Consulta con tu seguro y 
                            nosotros gestionamos la documentación necesaria.
                        </p>
                    </div>
                </div>
                
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿Cuánto dura un tratamiento de implantes?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Depende de cada caso, pero generalmente entre 3-6 meses desde la cirugía hasta la 
                            colocación de la corona definitiva. En casos favorables podemos hacer carga inmediata.
                        </p>
                    </div>
                </div>
                
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿Qué hago en caso de urgencia dental?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Llama a nuestro número de urgencias 24/7: +34 900 123 456. Te atenderemos en el menor 
                            tiempo posible, incluso fuera del horario habitual.
                        </p>
                    </div>
                </div>
                
                <div class="faq-item reveal">
                    <div class="faq-question">
                        <span>¿Atienden a niños pequeños?</span>
                        <span class="faq-icon">+</span>
                    </div>
                    <div class="faq-answer">
                        <p>
                            Sí, contamos con especialista en odontopediatría. Recomendamos la primera visita al 
                            cumplir el primer año o cuando aparezca el primer diente.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- CTA Section -->
    <section class="cta">
        <div class="section-container">
            <div class="cta-content reveal">
                <h2>Tu mejor sonrisa comienza aquí</h2>
                <p>
                    Déjanos ser parte de tu historia. Primera consulta gratuita, trato personalizado 
                    y financiación a tu medida.
                </p>
                
                <div class="hero-buttons">
                    <button class="btn btn-primary">Empieza hoy mismo</button>
                    <button class="btn btn-secondary">Escríbenos por WhatsApp</button>
                </div>
                
                <div class="cta-badges">
                    <div class="cta-badge">
                        <span class="cta-badge-icon">✓</span>
                        <span>Primera consulta gratis</span>
                    </div>
                    <div class="cta-badge">
                        <span class="cta-badge-icon">🤝</span>
                        <span>Sin compromiso</span>
                    </div>
                    <div class="cta-badge">
                        <span class="cta-badge-icon">❤️</span>
                        <span>Atención personalizada</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contacto">
        <div class="section-container">
            <div class="section-header reveal">
                <div class="section-subtitle">Contacto</div>
                <h2>Hablemos de tu sonrisa</h2>
            </div>
            
            <div class="contact-grid">
                <div class="contact-info reveal">
                    <h3>Información de contacto</h3>
                    
                    <div class="info-item">
                        <div class="info-icon">📍</div>
                        <div class="info-text">
                            <h4>Dirección</h4>
                            <p>Calle Principal, 123<br>28001 Madrid, España</p>
                        </div>
                    </div>
                    
                    <div class="info-item">
                        <div class="info-icon">📞</div>
                        <div class="info-text">
                            <h4>Teléfono</h4>
                            <p><a href="tel:+34900123456">+34 900 123 456</a></p>
                        </div>
                    </div>
                    
                    <div class="info-item">
                        <div class="info-icon">💬</div>
                        <div class="info-text">
                            <h4>WhatsApp</h4>
                            <p><a href="https://wa.me/34900123456">+34 900 123 456</a></p>
                        </div>
                    </div>
                    
                    <div class="info-item">
                        <div class="info-icon">✉️</div>
                        <div class="info-text">
                            <h4>Email</h4>
                            <p><a href="mailto:info@dentalcare.com">info@dentalcare.com</a></p>
                        </div>
                    </div>
                    
                    <div class="info-item">
                        <div class="info-icon">⏰</div>
                        <div class="info-text">
                            <h4>Horario</h4>
                            <p>
                                Lunes a Viernes: 9:00 - 20:00h<br>
                                Sábados: 10:00 - 14:00h<br>
                                <strong>Urgencias 24/7</strong>
                            </p>
                        </div>
                    </div>
                </div>
                
                <form class="contact-form reveal" id="contact-form">
                    <div class="form-group">
                        <label for="name">Nombre completo *</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="phone">Teléfono *</label>
                        <input type="tel" id="phone" name="phone" required>
                    </div>
                    
                    <div class="form-group">
                        <label for="email">Email</label>
                        <input type="email" id="email" name="email">
                    </div>
                    
                    <div class="form-group">
                        <label for="service">Motivo de consulta</label>
                        <select id="service" name="service">
                            <option value="">Selecciona una opción</option>
                            <option value="revision">Revisión general</option>
                            <option value="implantes">Implantes</option>
                            <option value="ortodoncia">Ortodoncia</option>
                            <option value="estetica">Estética dental</option>
                            <option value="urgencia">Urgencia</option>
                            <option value="otro">Otro</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="message">Mensaje (opcional)</label>
                        <textarea id="message" name="message"></textarea>
                    </div>
                    
                    <div class="form-group form-checkbox">
                        <input type="checkbox" id="privacy" name="privacy" required>
                        <label for="privacy">Acepto la política de privacidad *</label>
                    </div>
                    
                    <button type="submit" class="btn btn-primary" style="width: 100%;">Solicitar cita</button>
                </form>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer">
        <div class="footer-grid">
            <div class="footer-section">
                <a href="#inicio" class="logo" style="margin-bottom: 1rem;">
                    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 336 192">
  <g fill="#ece800" stroke="#000" stroke-width="5.33">
    <path d="M34.39 121.87C64.75 86.95 125.45 16.79 125.45 16.79l52.10 56.54h-56.23l-33.21 48.87z"/>
    <path d="M156.55 104.09l46.40-0.05 45.99 52.43-49.31-0.32z"/>
    <path d="M108.57 98.70l15.46-21.44 165.53-0.15c13.32-0.12 21.24 9.15 18.69 16.65l-14.76 42.88c-2.48 7.30-11.50 15.04-19.40 15.04h-20.94l-22.48-23.79c10.65-0.14 15.00 0.16 23.17-0.29 5.93-1.43 6.20-5.61 7.54-10.55l2.90-18.12z"/>
    <path d="M184.50 73.33l3.46-29.86c0.68-5.23 1.44-15.54 22.61-16.39h113.39l-3.14 16.39c-0.73 4.46-8.12 7.22-13.19 6.96l-72.87-0.45c-6.21-0.38-9.71 1.83-10.37 6.06l-0.94 8.53 16.96 8.75z"/>
    <path d="M31.85 126.31h133.49l20.26 25.14H15.88z"/>
  </g>
</svg>

                </a>
                <p>
                    Clínica Dental Gloria. Tu clínica de confianza. Más de 15 años cuidando sonrisas con 
                    profesionalidad, tecnología y cercanía.
                </p>
                <div class="social-links">
                    <a href="#" class="social-icon">📘</a>
                    <a href="#" class="social-icon">📷</a>
                    <a href="#" class="social-icon">🔗</a>
                </div>
            </div>
            
            <div class="footer-section">
                <h4>Enlaces rápidos</h4>
                <ul class="footer-links">
                    <li><a href="#inicio">Inicio</a></li>
                    <li><a href="#nosotros">Sobre nosotros</a></li>
                    <li><a href="#servicios">Servicios</a></li>
                    <li><a href="#equipo">Equipo</a></li>
                    <li><a href="#contacto">Contacto</a></li>
                </ul>
            </div>
            
            <div class="footer-section">
                <h4>Servicios principales</h4>
                <ul class="footer-links">
                    <li><a href="#servicios">Implantes dentales</a></li>
                    <li><a href="#servicios">Ortodoncia invisible</a></li>
                    <li><a href="#servicios">Estética dental</a></li>
                    <li><a href="#servicios">Urgencias 24/7</a></li>
                </ul>
            </div>
            
            <div class="footer-section">
                <h4>Legal</h4>
                <ul class="footer-links">
                    <li><a href="#">Aviso legal</a></li>
                    <li><a href="#">Política de privacidad</a></li>
                    <li><a href="#">Política de cookies</a></li>
                    <li><a href="#">Libro de reclamaciones</a></li>
                </ul>
            </div>
        </div>
        
        <div class="footer-bottom">
            <p>
                © 2024 Gloria Clínica Dental. Todos los derechos reservados. 
                Clínica autorizada por la Consejería de Salud. Nº registro: 12345
            </p>
        </div>
    </footer>

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

        // FAQ Accordion
        const faqItems = document.querySelectorAll('.faq-item');
        faqItems.forEach(item => {
            const question = item.querySelector('.faq-question');
            question.addEventListener('click', () => {
                const isActive = item.classList.contains('active');
                
                // Close all items
                faqItems.forEach(i => i.classList.remove('active'));
                
                // Open clicked item if it wasn't active
                if (!isActive) {
                    item.classList.add('active');
                }
            });
        });

        // Testimonials Slider
        const track = document.getElementById('testimonials-track');
        const prevBtn = document.getElementById('prev-btn');
        const nextBtn = document.getElementById('next-btn');
        let currentIndex = 0;
        const cardWidth = 420; // 400px + 20px gap

        nextBtn.addEventListener('click', () => {
            const maxIndex = track.children.length - 3;
            if (currentIndex < maxIndex) {
                currentIndex++;
                track.style.transform = `translateX(-${currentIndex * cardWidth}px)`;
            }
        });

        prevBtn.addEventListener('click', () => {
            if (currentIndex > 0) {
                currentIndex--;
                track.style.transform = `translateX(-${currentIndex * cardWidth}px)`;
            }
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
        revealOnScroll(); // Initial check

        // Smooth scroll for navigation links
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

        // Form submission
        const contactForm = document.getElementById('contact-form');
        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            alert('¡Gracias! Nos pondremos en contacto contigo en menos de 24 horas.');
            contactForm.reset();
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
    </script>
</body>
</html>

