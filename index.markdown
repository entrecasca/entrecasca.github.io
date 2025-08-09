---
layout: single
title: "Entre Casca"
header:
  overlay_color: "#1A1A1A"
  overlay_filter: "0.3"
  overlay_image: /assets/images/workshop-header.jpg
  excerpt: "Ateliê de marcenaria artesanal"
classes: wide
---
<style>
    /* Importação das fontes */
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap');

    /* Reset e configuração global */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: 'Inter', sans-serif;
      line-height: 1.6;
      color: #2C2C2C;
      background: #FAFAFA;
      overflow-x: hidden;
    }

    h1, h2, h3, h4, h5, h6 {
      font-family: 'Montserrat', sans-serif;
      font-weight: 600;
      color: #1A1A1A;
    }

    /* Container principal avec breakpoints améliorés */
    .main-container {
      max-width: 1400px;
      margin: 0 auto;
      padding: 0 2rem;
    }

    /* Navigation améliorée */
    .top-nav {
      background: #1A1A1A;
      color: white;
      padding: 1rem 0;
      position: sticky;
      top: 0;
      z-index: 1000;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    .nav-content {
      max-width: 1400px;
      margin: 0 auto;
      padding: 0 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      display: flex;
      align-items: center;
    }

    .logo img {
      height: 40px;
      width: auto;
      transition: opacity 0.3s ease;
    }

    /* Menu burger pour mobile */
    .mobile-menu-toggle {
      display: none;
      background: none;
      border: none;
      color: white;
      font-size: 1.5rem;
      cursor: pointer;
      padding: 0.5rem;
    }

    .nav-links {
      display: flex;
      gap: 2rem;
      list-style: none;
      margin: 0;
      padding: 0;
    }

    .nav-links a {
      color: #CCCCCC;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.3s ease;
      font-size: 0.95rem;
    }

    .nav-links a:hover {
      color: #E91E63;
    }

    /* Hero section responsive */
    .hero-section {
       background: linear-gradient(rgba(26, 26, 26, 0.6), rgba(26, 26, 26, 0.6)), url('/assets/images/stock_oficina.jpg') center/cover;
      padding: 8rem 0 6rem;
      color: white;
      text-align: center;
      position: relative;
      min-height: 60vh;
      display: flex;
      align-items: center;
    }

    .hero-content {
      max-width: 800px;
      margin: 0 auto;
      padding: 0 1rem;
    }

    .hero-title {
      font-family: 'Montserrat', sans-serif;
      font-size: clamp(2rem, 8vw, 3.5rem);
      font-weight: 700;
      color: white;
      margin-bottom: 1.5rem;
      line-height: 1.2;
      text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
    }

    .hero-subtitle {
      font-size: clamp(1rem, 3vw, 1.3rem);
      color: rgba(255,255,255,0.9);
      margin-bottom: 2rem;
      font-weight: 400;
      line-height: 1.6;
      text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
    }

    /* Services section avec grid responsive amélioré */
    .services-section {
      padding: clamp(3rem, 8vw, 6rem) 0;
      background: #F8F8F8;
    }

    .section-header {
      text-align: center;
      margin-bottom: clamp(2rem, 6vw, 4rem);
      padding: 0 1rem;
    }

    .section-title {
      font-family: 'Montserrat', sans-serif;
      font-size: clamp(1.8rem, 5vw, 2.5rem);
      font-weight: 600;
      color: #1A1A1A;
      margin-bottom: 1rem;
    }

    .section-subtitle {
      color: #666;
      font-size: clamp(1rem, 2vw, 1.1rem);
      max-width: 600px;
      margin: 0 auto;
    }

    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(min(100%, 350px), 1fr));
      gap: 2rem;
      padding: 0 1rem;
    }

    .service-card {
      background: white;
      border-radius: 8px;
      overflow: hidden;
      box-shadow: 0 2px 12px rgba(0,0,0,0.06);
      transition: all 0.3s ease;
      border: 1px solid #F0F0F0;
    }

    .service-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 8px 30px rgba(0,0,0,0.12);
    }

    .service-image {
        width: 100%;
        height: 280px;
        background-size: cover;
        background-position: center;
        position: relative;
    }

    .service-overlay {
      position: absolute;
      top: 1rem;
      left: 1rem;
      background: rgba(26, 26, 26, 0.8);
      color: white;
      padding: 0.5rem 1rem;
      border-radius: 4px;
      font-size: clamp(0.75rem, 2vw, 0.85rem);
      font-weight: 600;
    }

    .service-content {
      padding: clamp(1.5rem, 3vw, 2rem);
    }

    .service-title {
      font-family: 'Montserrat', sans-serif;
      font-size: clamp(1.2rem, 3vw, 1.5rem);
      font-weight: 600;
      color: #1A1A1A;
      margin-bottom: 1rem;
    }

    .service-description {
      color: #666;
      line-height: 1.7;
      margin-bottom: 1.5rem;
      font-size: clamp(0.9rem, 2vw, 1rem);
    }

    .service-features {
      list-style: none;
      padding: 0;
      margin: 0 0 1.5rem 0;
    }

    .service-features li {
      color: #666;
      font-size: clamp(0.85rem, 2vw, 0.9rem);
      margin-bottom: 0.5rem;
      padding-left: 1.2rem;
      position: relative;
    }

    .service-features li:before {
      content: "→";
      color: #E91E63;
      font-weight: bold;
      position: absolute;
      left: 0;
    }

    .service-link {
      color: #1A1A1A;
      font-weight: 600;
      text-decoration: none;
      font-size: clamp(0.85rem, 2vw, 0.95rem);
      border-bottom: 2px solid #E91E63;
      padding-bottom: 2px;
      transition: all 0.3s ease;
      display: inline-block;
    }

    /* About section responsive */
    .about-section {
      padding: clamp(3rem, 8vw, 6rem) 0;
      background: white;
    }

    .about-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(min(100%, 350px), 1fr));
      gap: clamp(2rem, 4vw, 4rem);
      align-items: center;
      padding: 0 1rem;
    }

    .about-content h2 {
      font-family: 'Montserrat', sans-serif;
      font-size: clamp(1.5rem, 4vw, 2.2rem);
      font-weight: 600;
      color: #1A1A1A;
      margin-bottom: 1.5rem;
      line-height: 1.3;
    }

    .about-text {
      color: #666;
      line-height: 1.8;
      margin-bottom: 1.5rem;
      font-size: clamp(0.95rem, 2vw, 1rem);
    }

    .about-highlight {
      background: #FFF8E1;
      border-left: 4px solid #E91E63;
      padding: clamp(1rem, 3vw, 1.5rem);
      margin: 2rem 0;
      border-radius: 4px;
    }

    .about-highlight p {
      margin: 0;
      color: #666;
      font-style: italic;
      font-size: clamp(0.9rem, 2vw, 1rem);
    }

    .about-image {
      width: 100%;
      height: clamp(250px, 50vw, 400px);
      background: url('/assets/images/madeiras_patchwork.webp') center/cover;
      border-radius: 8px;
      border: 1px solid #F0F0F0;
    }

    /* Footer responsive */
    .footer-section {
      background: #1A1A1A;
      color: white;
      padding: clamp(2rem, 6vw, 4rem) 0 2rem;
      position: relative;
    }

    .footer-content {
      display: grid;
      grid-template-columns: 1fr auto auto;
      gap: clamp(1.5rem, 4vw, 3rem);
      align-items: center;
      margin-bottom: 2rem;
      padding: 0 1rem;
    }

    .newsletter-content {
      max-width: 500px;
    }

    .newsletter-title {
      font-family: 'Montserrat', sans-serif;
      font-size: clamp(1.3rem, 4vw, 2rem);
      font-weight: 600;
      margin-bottom: 1rem;
      color: white;
    }

    .newsletter-description {
      color: #CCCCCC;
      font-size: clamp(0.95rem, 2vw, 1.1rem);
      margin-bottom: 2rem;
    }

    .newsletter-form {
      display: flex;
      gap: 0;
      border-radius: 6px;
      overflow: hidden;
      border: 1px solid #333;
      max-width: 500px;
    }

    .newsletter-input {
      flex: 1;
      padding: clamp(0.75rem, 2vw, 1rem) clamp(1rem, 3vw, 1.5rem);
      border: none;
      background: #2A2A2A;
      color: white;
      font-size: clamp(0.9rem, 2vw, 1rem);
      outline: none;
      font-family: 'Inter', sans-serif;
    }

    .newsletter-button {
      background: #E91E63;
      color: white;
      padding: clamp(0.75rem, 2vw, 1rem) clamp(1.5rem, 3vw, 2rem);
      border: none;
      font-weight: 600;
      cursor: pointer;
      transition: background 0.3s ease;
      font-size: clamp(0.9rem, 2vw, 1rem);
      font-family: 'Inter', sans-serif;
      white-space: nowrap;
    }

    .instagram-button {
      display: flex;
      align-items: center;
      justify-content: center;
      width: clamp(40px, 8vw, 50px);
      height: clamp(40px, 8vw, 50px);
      background: linear-gradient(45deg, #833AB4, #FD1D1D, #F77737);
      color: white;
      border-radius: 50%;
      text-decoration: none;
      font-size: clamp(1.2rem, 3vw, 1.5rem);
      transition: transform 0.3s ease;
      flex-shrink: 0;
    }

    .footer-flag {
      width: clamp(60px, 12vw, 80px);
      height: clamp(42px, 8vw, 56px);
      opacity: 0.8;
      transition: opacity 0.3s ease;
      flex-shrink: 0;
    }

    /* WhatsApp button responsive */
    .whatsapp-float {
      position: fixed;
      bottom: clamp(1rem, 3vw, 2rem);
      right: clamp(1rem, 3vw, 2rem);
      width: clamp(50px, 10vw, 60px);
      height: clamp(50px, 10vw, 60px);
      background: #25D366;
      color: white;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: clamp(1.5rem, 3vw, 1.8rem);
      text-decoration: none;
      box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4);
      transition: all 0.3s ease;
      z-index: 999;
    }

    .footer-bottom {
      border-top: 1px solid #333;
      padding-top: 2rem;
      text-align: center;
      color: #888;
      font-size: clamp(0.8rem, 2vw, 0.9rem);
      padding: 2rem 1rem 0;
    }

    /* Breakpoints pour tablettes */
    @media (max-width: 1024px) {
      .main-container {
        padding: 0 1.5rem;
      }

      .services-grid {
        grid-template-columns: repeat(auto-fit, minmax(min(100%, 320px), 1fr));
        gap: 1.5rem;
      }

      .about-grid {
        gap: 3rem;
      }
    }

    /* Breakpoints pour mobile */
    @media (max-width: 768px) {
      /* Navigation mobile */
      .mobile-menu-toggle {
        display: block;
      }

      .nav-links {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: #1A1A1A;
        flex-direction: column;
        padding: 1rem;
        box-shadow: 0 4px 10px rgba(0,0,0,0.2);
      }

      .nav-links.active {
        display: flex;
      }

      .nav-links li {
        width: 100%;
      }

      .nav-links a {
        display: block;
        padding: 0.75rem 1rem;
        border-bottom: 1px solid #333;
      }

      /* Hero mobile */
      .hero-section {
        padding: 5rem 0 4rem;
        min-height: 50vh;
      }

      /* Services mobile */
      .services-grid {
        grid-template-columns: 1fr;
        padding: 0;
      }

      /* About mobile */
      .about-grid {
        grid-template-columns: 1fr;
      }

      /* Footer mobile */
      .footer-content {
        grid-template-columns: 1fr;
        text-align: center;
        gap: 2rem;
      }

      .newsletter-form {
        flex-direction: column;
        margin: 0 auto;
      }

      .newsletter-input,
      .newsletter-button {
        border-radius: 6px;
        width: 100%;
      }

      .newsletter-button {
        margin-top: 0.5rem;
      }

      .instagram-button,
      .footer-flag {
        margin: 0 auto;
      }
    }

    /* Petits mobiles */
    @media (max-width: 480px) {
      .main-container,
      .nav-content {
        padding: 0 1rem;
      }

      .hero-section {
        padding: 4rem 0 3rem;
      }

      .service-content {
        padding: 1.25rem;
      }

      .about-content {
        padding: 0 0.5rem;
      }
    }

    /* Grandes écrans */
    @media (min-width: 1400px) {
      .hero-title {
        font-size: 4rem;
      }

      .hero-subtitle {
        font-size: 1.5rem;
      }

      .services-grid {
        grid-template-columns: repeat(3, 1fr);
      }
    }

    /* Amélioration de l'accessibilité */
    @media (prefers-reduced-motion: reduce) {
      * {
        animation: none !important;
        transition: none !important;
      }
    }

    /* Mode sombre système */
    @media (prefers-color-scheme: light) {
      .services-section,
      .about-section {
        background: #1A1A1A;
        color: #E0E0E0;
      }

      .service-card {
        background: #2A2A2A;
        border-color: #333;
      }

      .service-title,
      .section-title,
      .about-content h2 {
        color: #E0E0E0;
      }

      .service-description,
      .service-features li,
      .about-text,
      .section-subtitle {
        color: #B0B0B0;
      }
    }
  </style>

  <!-- Navigation Top -->
  <nav class="top-nav">
    <div class="nav-content">
        <div class="logo">
        <img src="/assets/images/logo.png" alt="Entre Casca">
        </div>
      <button class="mobile-menu-toggle" onclick="toggleMenu()">☰</button>
      <ul class="nav-links" id="navLinks">
        <li><a href="#oficinas">Oficinas</a></li>
        <li><a href="#aulas">Aulas</a></li>
        <li><a href="#criacoes">Criações</a></li>
        <li><a href="#sobre">Sobre</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hero Section -->
  <section class="hero-section">
    <div class="main-container">
      <div class="hero-content">
        <h1 class="hero-title">Entre Casca</h1>
        <p class="hero-subtitle">
          Ateliê de marcenaria artesanal onde transformamos madeira em arte há mais de 10 anos
        </p>
      </div>
    </div>
  </section>

  <!-- Services Section -->
  <section class="services-section" id="services">
    <div class="main-container">
      <div class="section-header">
        <h2 class="section-title">Nossos Serviços</h2>
        <p class="section-subtitle">
          Do aprendizado à criação, oferecemos experiências completas em marcenaria artesanal
        </p>
      </div>
      
      <div class="services-grid">
        <div class="service-card">
          <div class="service-image" style="background-image: url('/assets/images/escrivaninha_pinceis.jpg')">
            <div class="service-overlay">Grupos pequenos</div>
          </div>
          <div class="service-content">
            <h3 class="service-title">Oficinas Práticas</h3>
            <p class="service-description">
              Oficinas intensivas para todos os níveis, onde você aprende fazendo. Técnicas tradicionais e modernas em um ambiente colaborativo.
            </p>
            <ul class="service-features">
              <li>Turmas de até 8 pessoas</li>
              <li>Ferramentas profissionais incluídas</li>
              <li>Projeto personalizado</li>
              <li>Certificado de participação</li>
            </ul>
            <a href="#oficinas" class="service-link">Ver oficinas disponíveis</a>
          </div>
        </div>

        <div class="service-card">
          <div class="service-image" style="background-image: url('/assets/images/cortando_madeira.jpg')">
            <div class="service-overlay">Aulas individuais</div>
          </div>
          <div class="service-content">
            <h3 class="service-title">Aulas Personalizadas</h3>
            <p class="service-description">
              Aulas individuais ou em pequenos grupos, focadas nas suas necessidades específicas e ritmo de aprendizado.
            </p>
            <ul class="service-features">
              <li>Horários flexíveis</li>
              <li>Atenção individualizada</li>
              <li>Técnicas específicas</li>
              <li>Material incluso</li>
            </ul>
            <a href="#aulas" class="service-link">Agendar uma aula</a>
          </div>
        </div>

        <div class="service-card">
          <div class="service-image" style="background-image: url('/assets/images/banco_bandeirola.webp')">
            <div class="service-overlay">Peças únicas</div>
          </div>
          <div class="service-content">
            <h3 class="service-title">Criações Originais</h3>
            <p class="service-description">
              Portfólio de peças únicas criadas em nosso ateliê. Cada obra é uma expressão artística que valoriza a beleza natural da madeira.
            </p>
            <ul class="service-features">
              <li>Peças assinadas</li>
              <li>Madeiras selecionadas</li>
              <li>Acabamento artesanal</li>
              <li>Certificado de autenticidade</li>
            </ul>
            <a href="#criacoes" class="service-link">Explorar coleção</a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section class="about-section" id="sobre">
    <div class="main-container">
      <div class="about-grid">
        <div class="about-content">
          <h2>A paixão pela madeira nos move</h2>
          <p class="about-text">
            O Entre Casca nasceu da paixão pela madeira e pelo artesanato brasileiro. Há mais de uma década, criamos um espaço onde tradição e inovação se encontram.
          </p>
          <p class="about-text">
            Nosso ateliê é mais que um local de trabalho - é um ponto de encontro para artesãos, aprendizes e amantes da marcenaria que compartilham o amor pela transformação da madeira em arte.
          </p>
          <div class="about-highlight">
            <p>"Cada peça de madeira tem sua própria personalidade. Nosso papel é revelá-la e dar-lhe nova vida através do artesanato."</p>
          </div>
        </div>
        <div class="about-image"></div>
      </div>
    </div>
  </section>

  <!-- Footer Section -->
  <footer class="footer-section">
    <div class="main-container">
      <div class="footer-content">
        <!-- Newsletter -->
        <div class="newsletter-content">
          <h3 class="newsletter-title">Fique conectado com o Entre Casca</h3>
          <p class="newsletter-description">
            Receba dicas de marcenaria, novidades sobre oficinas e histórias do nosso ateliê.
          </p>
          
          <form name="newsletter" method="POST" data-netlify="true" class="newsletter-form">
            <input type="email" 
                   name="email" 
                   placeholder="Seu email..." 
                   required
                   class="newsletter-input">
            <button type="submit" class="newsletter-button">
              Inscrever-se
            </button>
            <input type="hidden" name="form-name" value="newsletter">
          </form>
        </div>

        <!-- Instagram button -->
        <a href="https://instagram.com/entrecasca" class="instagram-button" target="_blank" aria-label="Instagram">
          📷
        </a>

        <!-- Bandeira Mangueira -->
        <div class="footer-flag">
          <svg viewBox="0 0 400 280" xmlns="http://www.w3.org/2000/svg" style="width: 100%; height: 100%;">
            <rect width="400" height="280" fill="#E91E63"/>
            <path d="M200,40 L360,140 L200,240 L40,140 Z" fill="#FFFFFF" stroke="#F0F0F0" stroke-width="3"/>
            <circle cx="200" cy="140" r="80" fill="#4CAF50" stroke="#388E3C" stroke-width="4"/>
            <g stroke="#81C784" stroke-width="3" fill="none" opacity="0.9">
              <circle cx="200" cy="140" r="65" stroke-dasharray="12,6"/>
              <path d="M200,90 L200,190 M150,140 L250,140"/>
            </g>
          </svg>
        </div>
      </div>

      <!-- Copyright -->
      <div class="footer-bottom">
        <p>&copy; 2024 Entre Casca. Todos os direitos reservados.</p>
      </div>
    </div>
  </footer>

  <!-- WhatsApp Floating Button -->
  <a href="https://wa.me/5511999999999" class="whatsapp-float" target="_blank" aria-label="WhatsApp">
    💬
  </a>

  <script>
    function toggleMenu() {
      const navLinks = document.getElementById('navLinks');
      navLinks.classList.toggle('active');
    }

    // Fermer le menu mobile lors du clic sur un lien
    document.querySelectorAll('.nav-links a').forEach(link => {
      link.addEventListener('click', () => {
        document.getElementById('navLinks').classList.remove('active');
      });
    });

    // Smooth scroll pour les ancres
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