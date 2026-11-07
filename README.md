# testeone.github.io
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    
    <!-- SEO Essencial -->
    <title>Studio Bella | Salão de Beleza e Estética</title>
    <meta name="description" content="Descubra sua melhor versão no Studio Bella. Especialistas em cabelo, coloração, manicure, estética facial e sobrancelhas. Agende seu horário pelo WhatsApp!">
    <meta name="keywords" content="salão de beleza, cabeleireiro, estética facial, manicure, design de sobrancelhas, Studio Bella">
    
    <!-- Open Graph / Redes Sociais -->
    <meta property="og:title" content="Studio Bella | Salão de Beleza e Estética">
    <meta property="og:description" content="Descubra sua melhor versão no Studio Bella. Cabelo, coloração, estética e bem-estar. Agende seu horário!">
    <meta property="og:image" content="https://images.unsplash.com/photo-1560066984-138dadb4c035?auto=format&fit=crop&w=1200&q=80">
    <meta property="og:url" content="https://www.studiobella.com.br">
    <meta property="og:type" content="website">

    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600&family=Playfair+Display:wght@500;600;700&display=swap" rel="stylesheet">
    
    <!-- FontAwesome para Ícones -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        /* Variáveis de Cores e Tipografia */
        :root {
            --primary-pink: #F3C6D3;
            --dark-pink: #D48C9F;
            --nude: #F9F3EE;
            --gold: #C5A059;
            --dark-text: #2C2C2C;
            --light-bg: #FCFAF8;
            --white: #FFFFFF;
            --transition: all 0.3s ease;
        }

        /* Reset e Estilos Globais */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: var(--light-bg);
            color: var(--dark-text);
            line-height: 1.6;
        }

        h1, h2, h3, h4 {
            font-family: 'Playfair Display', serif;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        ul {
            list-style: none;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Botões */
        .btn-primary {
            display: inline-block;
            background-color: var(--gold);
            color: var(--white);
            padding: 14px 28px;
            border-radius: 30px;
            font-weight: 600;
            text-transform: uppercase;
            font-size: 0.9rem;
            letter-spacing: 1px;
            transition: var(--transition);
            box-shadow: 0 4px 15px rgba(197, 160, 89, 0.3);
        }

        .btn-primary:hover {
            background-color: #b08d47;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(197, 160, 89, 0.4);
        }

        /* HEADER */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(255, 255, 255, 0.95);
            backdrop-filter: blur(5px);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            z-index: 1000;
        }

        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            height: 80px;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--dark-text);
            letter-spacing: 1px;
        }

        .logo span {
            color: var(--dark-pink);
        }

        .nav-menu {
            display: flex;
            gap: 30px;
            align-items: center;
        }

        .nav-menu a {
            font-size: 0.95rem;
            font-weight: 500;
            transition: var(--transition);
        }

        .nav-menu a:hover {
            color: var(--dark-pink);
        }

        /* HERO SECTION */
        .hero {
            height: 100vh;
            background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.4)), url('https://images.unsplash.com/photo-1560066984-138dadb4c035?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            display: flex;
            align-items: center;
            text-align: center;
            color: var(--white);
            padding-top: 80px;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            font-weight: 700;
            text-shadow: 0 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.15rem;
            margin-bottom: 30px;
            font-weight: 300;
            text-shadow: 0 1px 2px rgba(0,0,0,0.3);
        }

        /* QUEM SOMOS */
        .about {
            padding: 100px 0;
            background-color: var(--white);
        }

        .about-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .about-text h2 {
            font-size: 2.5rem;
            margin-bottom: 20px;
            color: var(--dark-text);
        }

        .about-text p {
            margin-bottom: 15px;
            color: #555;
        }

        .about-image img {
            width: 100%;
            border-radius: 12px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.08);
        }

        /* SERVIÇOS */
        .services {
            padding: 100px 0;
            background-color: var(--nude);
        }

        .section-header {
            text-align: center;
            margin-bottom: 60px;
        }

        .section-header h2 {
            font-size: 2.5rem;
            margin-bottom: 15px;
        }

        .section-header p {
            color: #666;
            max-width: 600px;
            margin: 0 auto;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: var(--white);
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.05);
            transition: var(--transition);
        }

        .service-card:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 30px rgba(0,0,0,0.1);
        }

        .service-img {
            height: 200px;
            width: 100%;
            object-fit: cover;
        }

        .service-info {
            padding: 25px;
        }

        .service-info h3 {
            font-size: 1.4rem;
            margin-bottom: 10px;
        }

        .service-info p {
            font-size: 0.9rem;
            color: #666;
            margin-bottom: 20px;
        }

        .service-footer {
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-top: 1px solid #eee;
            padding-top: 15px;
        }

        .service-price {
            font-weight: 600;
            color: var(--dark-pink);
            font-size: 1rem;
        }

        .service-btn {
            font-size: 0.85rem;
            font-weight: 600;
            color: var(--gold);
            transition: var(--transition);
        }

        .service-btn:hover {
            color: var(--dark-text);
        }

        /* DEPOIMENTOS */
        .testimonials {
            padding: 100px 0;
            background-color: var(--white);
        }

        .testimonials-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .testimonial-card {
            background-color: var(--light-bg);
            padding: 30px;
            border-radius: 12px;
            border-left: 4px solid var(--dark-pink);
            box-shadow: 0 4px 15px rgba(0,0,0,0.03);
        }

        .stars {
            color: var(--gold);
            margin-bottom: 15px;
        }

        .testimonial-card p {
            font-style: italic;
            color: #555;
            margin-bottom: 20px;
            font-size: 0.95rem;
        }

        .client-info h3 {
            font-size: 1.1rem;
            font-weight: 600;
        }

        .client-info span {
            font-size: 0.8rem;
            color: #888;
        }

        /* FOOTER / RODAPÉ */
        footer {
            background-color: #1A1A1A;
            color: var(--white);
            padding: 80px 0 30px 0;
        }

        .footer-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 60px;
        }

        .footer-col h3 {
            font-size: 1.3rem;
            margin-bottom: 20px;
            color: var(--primary-pink);
        }

        .footer-col p, .footer-col address {
            font-style: normal;
            font-size: 0.9rem;
            color: #bbb;
            margin-bottom: 10px;
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
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            transition: var(--transition);
        }

        .social-links a:hover {
            background-color: var(--dark-pink);
            transform: translateY(-3px);
        }

        .footer-bottom {
            text-align: center;
            border-top: 1px solid rgba(255,255,255,0.1);
            padding-top: 20px;
            font-size: 0.85rem;
            color: #888;
        }

        /* BOTÃO FLUTUANTE WHATSAPP */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background-color: #25D366;
            color: var(--white);
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4);
            z-index: 1001;
            transition: var(--transition);
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
            box-shadow: 0 6px 25px rgba(37, 211, 102, 0.6);
        }

        /* RESPONSIVIDADE MOBILE */
        @media (max-width: 768px) {
            .nav-menu {
                display: none; /* Poderia adicionar menu hamburguer, mantido simples para focar na conversão mobile direta */
            }
            .hero h1 {
                font-size: 2.2rem;
            }
            .about-grid {
                grid-template-columns: 1fr;
            }
            .about-image {
                order: -1;
            }
        }
    </style>
</head>
<body>

    <!-- HEADER -->
    <header>
        <div class="container header-container">
            <a href="#" class="logo">Studio <span>Bella</span></a>
            <nav class="nav-menu">
                <a href="#sobre">Quem Somos</a>
                <a href="#servicos">Serviços</a>
                <a href="#depoimentos">Depoimentos</a>
                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20um%20horário." class="btn-primary" target="_blank" rel="noopener">Agendar Horário</a>
            </nav>
        </div>
    </header>

    <main>
        <!-- HERO SECTION -->
        <section class="hero">
            <div class="container hero-content">
                <h1>Realce a sua beleza natural</h1>
                <p>Experiências exclusivas de cuidado capilar, estética e bem-estar em um ambiente sofisticado feito para você.</p>
                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20um%20horário." class="btn-primary" target="_blank" rel="noopener">Agendar um Horário</a>
            </div>
        </section>

        <!-- QUEM SOMOS -->
        <section id="sobre" class="about">
            <div class="container about-grid">
                <div class="about-text">
                    <h2>Excelência em Autoestima e Cuidado</h2>
                    <p>Fundado com a missão de transformar rotinas de beleza em momentos únicos de relaxamento e autocuidado, o Studio Bella reúne profissionais altamente qualificados e produtos de altíssima qualidade.</p>
                    <p>Acreditamos que cada cliente é única. Por isso, oferecemos um atendimento totalmente personalizado, focado em valorizar os seus traços e elevar a sua confiança.</p>
                    <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20saber%20mais%20sobre%20o%20salão." class="btn-primary" style="margin-top: 15px;" target="_blank" rel="noopener">Fale Conosco</a>
                </div>
                <div class="about-image">
                    <img src="https://images.unsplash.com/photo-1522337360788-8b13dee7a37e?auto=format&fit=crop&w=800&q=80" alt="Interior elegante e moderno do Studio Bella com foco em atendimento personalizado">
                </div>
            </div>
        </section>

        <!-- SERVIÇOS -->
        <section id="servicos" class="services">
            <div class="container">
                <div class="section-header">
                    <h2>Nossos Serviços</h2>
                    <p>Conheça os tratamentos preferidos das nossas clientes e escolha o seu próximo momento de cuidado.</p>
                </div>
                <div class="services-grid">
                    <!-- Serviço 1 -->
                    <article class="service-card">
                        <img src="https://images.unsplash.com/photo-1562322140-8baeececf3df?auto=format&fit=crop&w=600&q=80" alt="Profissional realizando coloração e tratamento capilar em cliente" class="service-img">
                        <div class="service-info">
                            <h3>Cabelo & Coloração</h3>
                            <p>Cortes modernos, mechas personalizadas, balayage, hidratações profundas e reconstrução capilar.</p>
                            <div class="service-footer">
                                <span class="service-price">A partir de R$ 120</span>
                                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20Cabelo%20e%20Coloração." class="service-btn" target="_blank" rel="noopener">Agendar <i class="fa-solid fa-chevron-right"></i></a>
                            </div>
                        </div>
                    </article>

                    <!-- Serviço 2 -->
                    <article class="service-card">
                        <img src="https://images.unsplash.com/photo-1632345031435-8727f6c97d34?auto=format&fit=crop&w=600&q=80" alt="Manicure fazendo unhas decoradas e cuidadas de uma cliente" class="service-img">
                        <div class="service-info">
                            <h3>Manicure & Pedicure</h3>
                            <p>Esmaltação em gel, cutilagem impecável, spa dos pés e técnicas avançadas de fortalecimento.</p>
                            <div class="service-footer">
                                <span class="service-price">A partir de R$ 50</span>
                                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20Manicure%20e%20Pedicure." class="service-btn" target="_blank" rel="noopener">Agendar <i class="fa-solid fa-chevron-right"></i></a>
                            </div>
                        </div>
                    </article>

                    <!-- Serviço 3 -->
                    <article class="service-card">
                        <img src="https://images.unsplash.com/photo-1570172619644-dfd03ed5d881?auto=format&fit=crop&w=600&q=80" alt="Mulher recebendo tratamento de limpeza de pele e estética facial" class="service-img">
                        <div class="service-info">
                            <h3>Estética Facial</h3>
                            <p>Limpeza de pele profunda, peeling revitalizante, hidratação facial e protocolos rejuvenescedores.</p>
                            <div class="service-footer">
                                <span class="service-price">A partir de R$ 150</span>
                                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20Estética%20Facial." class="service-btn" target="_blank" rel="noopener">Agendar <i class="fa-solid fa-chevron-right"></i></a>
                            </div>
                        </div>
                    </article>

                    <!-- Serviço 4 -->
                    <article class="service-card">
                        <img src="https://images.unsplash.com/photo-1512290900672-178490a9829f?auto=format&fit=crop&w=600&q=80" alt="Sobrancelhas perfeitamente desenhadas e modeladas" class="service-img">
                        <div class="service-info">
                            <h3>Sobrancelhas & Cílios</h3>
                            <p>Design personalizado de sobrancelhas com henna, tintura, brow lamination e extensão de cílios fio a fio.</p>
                            <div class="service-footer">
                                <span class="service-price">A partir de R$ 60</span>
                                <a href="https://wa.me/5511999999999?text=Olá!%20Gostaria%20de%20agendar%20Sobrancelhas." class="service-btn" target="_blank" rel="noopener">Agendar <i class="fa-solid fa-chevron-right"></i></a>
                            </div>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- DEPOIMENTOS -->
        <section id="depoimentos" class="testimonials">
            <div class="container">
                <div class="section-header">
                    <h2>O que nossas clientes dizem</h2>
                    <p>A satisfação de quem confia no nosso trabalho é o nosso maior orgulho.</p>
                </div>
                <div class="testimonials-grid">
                    <!-- Depoimento 1 -->
                    <article class="testimonial-card">
                        <div class="stars">
                            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                        </div>
                        <p>"Simplesmente o melhor salão que já frequentei! O atendimento é impecável e o resultado da minha cor ficou exatamente como eu queria. Recomendo muito!"</p>
                        <div class="client-info">
                            <h3>Camila Souza</h3>
                            <span>Cliente do Instagram</span>
                        </div>
                    </article>

                    <!-- Depoimento 2 -->
                    <article class="testimonial-card">
                        <div class="stars">
                            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                        </div>
                        <p>"Fiz o design de sobrancelhas e manicure. O ambiente é super aconchegante, limpo e sofisticado. Dá vontade de passar o dia inteiro lá dentro!"</p>
                        <div class="client-info">
                            <h3>Beatriz Lima</h3>
                            <span>Google Avaliações</span>
                        </div>
                    </article>

                    <!-- Depoimento 3 -->
                    <article class="testimonial-card">
                        <div class="stars">
                            <i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i><i class="fa-solid fa-star"></i>
                        </div>
                        <p>"A limpeza de pele e a hidratação deixaram meu rosto renovado. Profissionais dedicadas e atenciosas aos mínimos detalhes. Ganharam uma cliente fiel!"</p>
                        <div class="client-info">
                            <h3>Juliana Martins</h3>
                            <span>Cliente Recorrente</span>
                        </div>
                    </article>
                </div>
            </div>
        </section>
    </main>

    <!-- FOOTER / RODAPÉ -->
    <footer>
        <div class="container">
            <div class="footer-grid">
                <!-- Coluna 1: Sobre -->
                <div class="footer-col">
                    <h3>Studio Bella</h3>
                    <p>Sua referência em beleza, estética e bem-estar. Venha viver uma experiência única de cuidado pessoal.</p>
                    <div class="social-links">
                        <a href="https://instagram.com" target="_blank" rel="noopener" aria-label="Instagram"><i class="fa-brands fa-instagram"></i></a>
                        <a href="https://facebook.com" target="_blank" rel="noopener" aria-label="Facebook"><i class="fa-brands fa-facebook-f"></i></a>
                        <a href="https://tiktok.com" target="_blank" rel="noopener" aria-label="TikTok"><i class="fa-brands fa-tiktok"></i></a>
                    </div>
                </div>

                <!-- Coluna 2: Contato e SEO Local -->
                <div class="footer-col">
                    <h3>Localização & Contato</h3>
                    <address>
                        <p><i class="fa-solid fa-location-dot"></i> Rua das Flores, 123 - Sala 402<br>Bairro Jardins, São Paulo - SP</p>
                    </address>
                    <p><i class="fa-solid fa-phone"></i> (11) 99999-9999</p>
                    <p><i class="fa-solid fa-envelope"></i> contato@studiobella.com.br</p>
                </div>

                <!-- Coluna 3: Horários -->
                <div class="footer-col">
                    <h3>Horário de Funcionamento</h3>
                    <p>Terça a Sexta: 09h às 20h</p>
                    <p>Sábado: 08h às 18h</p>
                    <p>Domingos e Segundas: Fechado</p>
                </div>
            </div>

            <div class="footer-bottom">
                <p>&copy; 2026 Studio Bella. Todos os direitos reservados. Desenvolvido para alta conversão mobile.</p>
            </div>
        </div>
    </footer>

    <!-- BOTÃO WHATSAPP FLUTUANTE -->
    <a href="https://wa.me/5511999999999?text=Olá!%20Vim%20pelo%20site%20e%20gostaria%20de%20agendar%20um%20horário." class="whatsapp-float" target="_blank" rel="noopener" aria-label="Fale conosco pelo WhatsApp">
        <i class="fa-brands fa-whatsapp"></i>
    </a>

</body>
</html>
