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
/* Importação das fontes / Import des polices */
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap');

/* Reset e configuração global / Reset et configuration globale */
* {
  box-sizing: border-box;
}

body {
  font-family: 'Inter', sans-serif;
  line-height: 1.6;
  color: #2C2C2C;
  background: #FAFAFA;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  color: #1A1A1A;
}

/* Container principal / Conteneur principal */
.main-container {
  max-width: 1400px;
  margin: 0 auto;
  padding: 0 2rem;
}

/* Header navigation style woodwork.nl / Navigation header style woodwork.nl */
.top-nav {
  background: #1A1A1A;
  color: white;
  padding: 1rem 0;
  position: relative;
  z-index: 10;
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

.logo img:hover {
  opacity: 0.8;
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

/* Hero section style woodwork.nl / Section hero style woodwork.nl */
.hero-section {
  background: linear-gradient(rgba(26, 26, 26, 0.6), rgba(26, 26, 26, 0.6)), url('/assets/images/stock_oficina.jpg') center/cover;
  padding: 8rem 0 6rem;
  color: white;
  text-align: center;
  position: relative;
}

.hero-content {
  max-width: 800px;
  margin: 0 auto;
}

.hero-title {
  font-family: 'Montserrat', sans-serif;
  font-size: 3.5rem;
  font-weight: 700;
  color: white;
  margin-bottom: 1.5rem;
  line-height: 1.2;
  text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
}

.hero-subtitle {
  font-size: 1.3rem;
  color: rgba(255,255,255,0.9);
  margin-bottom: 2rem;
  font-weight: 400;
  line-height: 1.6;
  text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
}

/* Services section style industriel / Section services style industriel */
.services-section {
  padding: 6rem 0;
  background: #F8F8F8;
}

.section-header {
  text-align: center;
  margin-bottom: 4rem;
}

.section-title {
  font-family: 'Montserrat', sans-serif;
  font-size: 2.5rem;
  font-weight: 600;
  color: #1A1A1A;
  margin-bottom: 1rem;
}

.section-subtitle {
  color: #666;
  font-size: 1.1rem;
  max-width: 600px;
  margin: 0 auto;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(400px, 1fr));
  gap: 2rem;
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
  font-size: 0.85rem;
  font-weight: 600;
}

.service-content {
  padding: 2rem;
}

.service-title {
  font-family: 'Montserrat', sans-serif;
  font-size: 1.5rem;
  font-weight: 600;
  color: #1A1A1A;
  margin-bottom: 1rem;
}

.service-description {
  color: #666;
  line-height: 1.7;
  margin-bottom: 1.5rem;
}

.service-features {
  list-style: none;
  padding: 0;
  margin: 0 0 1.5rem 0;
}

.service-features li {
  color: #666;
  font-size: 0.9rem;
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
  font-size: 0.95rem;
  border-bottom: 2px solid #E91E63;
  padding-bottom: 2px;
  transition: all 0.3s ease;
}

.service-link:hover {
  color: #E91E63;
  text-decoration: none;
}

/* About section style atelier / Section about style atelier */
.about-section {
  padding: 6rem 0;
  background: white;
}

.about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 4rem;
  align-items: center;
}

.about-content h2 {
  font-family: 'Montserrat', sans-serif;
  font-size: 2.2rem;
  font-weight: 600;
  color: #1A1A1A;
  margin-bottom: 1.5rem;
  line-height: 1.3;
}

.about-text {
  color: #666;
  line-height: 1.8;
  margin-bottom: 1.5rem;
}

.about-highlight {
  background: #FFF8E1;
  border-left: 4px solid #E91E63;
  padding: 1.5rem;
  margin: 2rem 0;
  border-radius: 4px;
}

.about-highlight p {
  margin: 0;
  color: #666;
  font-style: italic;
}

.about-image {
  width: 100%;
  height: 400px;
  background: url('/assets/images/madeiras_patchwork.webp') center/cover;
  border-radius: 8px;
  border: 1px solid #F0F0F0;
}

/* Footer style novo / Nouveau style footer */
.footer-section {
  background: #1A1A1A;
  color: white;
  padding: 4rem 0 2rem;
  position: relative;
}

.footer-content {
  display: grid;
  grid-template-columns: 1fr auto auto;
  gap: 3rem;
  align-items: center;
  margin-bottom: 2rem;
}

.newsletter-content {
  max-width: 500px;
}

.newsletter-title {
  font-family: 'Montserrat', sans-serif;
  font-size: 2rem;
  font-weight: 600;
  margin-bottom: 1rem;
  color: white;
}

.newsletter-description {
  color: #CCCCCC;
  font-size: 1.1rem;
  margin-bottom: 2rem;
}

.newsletter-form {
  display: flex;
  gap: 0;
  border-radius: 6px;
  overflow: hidden;
  border: 1px solid #333;
  max-width: 400px;
}

.newsletter-input {
  flex: 1;
  padding: 1rem 1.5rem;
  border: none;
  background: #2A2A2A;
  color: white;
  font-size: 1rem;
  outline: none;
  font-family: 'Inter', sans-serif;
}

.newsletter-input::placeholder {
  color: #888;
}

.newsletter-button {
  background: #E91E63;
  color: white;
  padding: 1rem 2rem;
  border: none;
  font-weight: 600;
  cursor: pointer;
  transition: background 0.3s ease;
  font-size: 1rem;
  font-family: 'Inter', sans-serif;
}

.newsletter-button:hover {
  background: #C2185B;
}

/* Instagram button / Bouton Instagram */
.instagram-button {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 50px;
  height: 50px;
  background: linear-gradient(45deg, #833AB4, #FD1D1D, #F77737);
  color: white;
  border-radius: 50%;
  text-decoration: none;
  font-size: 1.5rem;
  transition: transform 0.3s ease;
}

.instagram-button:hover {
  transform: scale(1.1);
  color: white;
  text-decoration: none;
}

/* Drapeau dans le footer / Drapeau dans le footer */
.footer-flag {
  width: 80px;
  height: 56px;
  opacity: 0.8;
  transition: opacity 0.3s ease;
}

.footer-flag:hover {
  opacity: 1;
}

/* WhatsApp floating button / Bouton WhatsApp flottant */
.whatsapp-float {
  position: fixed;
  bottom: 2rem;
  right: 2rem;
  width: 60px;
  height: 60px;
  background: #25D366;
  color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.8rem;
  text-decoration: none;
  box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4);
  transition: all 0.3s ease;
  z-index: 1000;
}

.whatsapp-float:hover {
  transform: scale(1.1);
  color: white;
  text-decoration: none;
  box-shadow: 0 6px 25px rgba(37, 211, 102, 0.6);
}

/* Copyright / Copyright */
.footer-bottom {
  border-top: 1px solid #333;
  padding-top: 2rem;
  text-align: center;
  color: #888;
  font-size: 0.9rem;
}

/* Responsividade / Responsive */
@media (max-width: 768px) {
  .main-container,
  .nav-content {
    padding: 0 1rem;
  }
  
  .hero-title {
    font-size: 2.5rem;
  }
  
  .services-grid {
    grid-template-columns: 1fr;
  }
  
  .about-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
  
  .nav-links {
    display: none;
  }
  
  .footer-content {
    grid-template-columns: 1fr;
    text-align: center;
    gap: 2rem;
  }
  
  .newsletter-form {
    flex-direction: column;
    border-radius: 6px;
  }
  
  .newsletter-input,
  .newsletter-button {
    border-radius: 6px;
  }
  
  .whatsapp-float {
    width: 50px;
    height: 50px;
    font-size: 1.5rem;
    bottom: 1rem;
    left: 1rem;
  }
}
</style>

<!-- Navigation Top -->
<nav class="top-nav">
  <div class="nav-content">
    <div class="logo">
      <img src="/assets/images/logo.png" alt="Entre Casca">
    </div>
    <ul class="nav-links">
      <li><a href="/oficinas/">Oficinas</a></li>
      <li><a href="/aulas/">Aulas</a></li>
      <li><a href="/criacoes/">Criações</a></li>
      <li><a href="/sobre/">Sobre</a></li>
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
<section class="services-section">
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
          <a href="/oficinas/" class="service-link">Ver oficinas disponíveis</a>
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
          <a href="/aulas/" class="service-link">Agendar uma aula</a>
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
          <a href="/criacoes/" class="service-link">Explorar coleção</a>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- About Section -->
<section class="about-section">
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
      <!-- Newsletter à gauche / Newsletter à gauche -->
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

      <!-- Instagram button / Bouton Instagram -->
      <a href="https://instagram.com/entrecasca" class="instagram-button" target="_blank">
        📷
      </a>

      <!-- Drapeau Mangueira à droite / Drapeau Mangueira à droite -->
      <div class="footer-flag">
        <svg viewBox="0 0 400 280" xmlns="http://www.w3.org/2000/svg" style="width: 100%; height: 100%;">
          <!-- Fundo rosa/magenta Mangueira / Background rose/magenta Mangueira -->
          <rect width="400" height="280" fill="#E91E63"/>
          
          <!-- Padrões tribais de fundo / Motifs tribaux en arrière-plan -->
          <defs>
            <pattern id="tribalPatternFooter" x="0" y="0" width="40" height="40" patternUnits="userSpaceOnUse">
              <path d="M20,5 L35,20 L20,35 L5,20 Z" fill="none" stroke="#C2185B" stroke-width="1" opacity="0.5"/>
              <circle cx="20" cy="20" r="3" fill="#C2185B" opacity="0.3"/>
            </pattern>
            
            <pattern id="barkTextureFooter" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
              <path d="M0,10 Q5,5 10,10 T20,10" fill="none" stroke="#C2185B" stroke-width="0.8" opacity="0.3"/>
              <path d="M0,15 Q5,12 10,15 T20,15" fill="none" stroke="#C2185B" stroke-width="0.8" opacity="0.3"/>
            </pattern>
          </defs>
          
          <rect width="400" height="280" fill="url(#tribalPatternFooter)"/>
          <rect width="400" height="280" fill="url(#barkTextureFooter)"/>
          
          <!-- Losango branco estilizado / Losange blanc stylisé -->
          <path d="M200,40 L360,140 L200,240 L40,140 Z" fill="#FFFFFF" stroke="#F0F0F0" stroke-width="3"/>
          
          <!-- Círculo verde Mangueira central / Cercle vert Mangueira central -->
          <circle cx="200" cy="140" r="80" fill="#4CAF50" stroke="#388E3C" stroke-width="4"/>
          
          <!-- Padrões tribais no círculo verde / Motifs tribaux sur le cercle vert -->
          <g stroke="#81C784" stroke-width="3" fill="none" opacity="0.9">
            <circle cx="200" cy="140" r="65" stroke-dasharray="12,6"/>
            <circle cx="200" cy="140" r="55" stroke-dasharray="8,4"/>
            <circle cx="200" cy="140" r="45" stroke-dasharray="6,3"/>
            <circle cx="200" cy="140" r="35" stroke-dasharray="4,2"/>
            
            <!-- Cruz direcional indígena / Croix directionnelle indigène -->
            <path d="M200,90 L200,190 M150,140 L250,140"/>
            <path d="M175,115 L225,165 M225,115 L175,165"/>
            
            <!-- Padrões radiais / Motifs radiaux -->
            <path d="M200,140 L170,110 M200,140 L230,110 M200,140 L230,170 M200,140 L170,170"/>
            <path d="M200,140 L185,105 M200,140 L215,105 M200,140 L215,175 M200,140 L185,175"/>
          </g>
          
          <!-- Pontos cardeais tribais maiores / Points cardinaux tribaux plus grands -->
          <g fill="#81C784" opacity="1">
            <circle cx="200" cy="100" r="8"/>
            <circle cx="200" cy="180" r="8"/>
            <circle cx="160" cy="140" r="8"/>
            <circle cx="240" cy="140" r="8"/>
          </g>
          
          <!-- Estrelas estilizadas no círculo verde / Étoiles stylisées dans le cercle vert -->
          <g fill="#FFFFFF" opacity="1">
            <path d="M180,120 L182,125 L187,125 L183,128 L185,133 L180,130 L175,133 L177,128 L173,125 L178,125 Z"/>
            <path d="M220,160 L222,165 L227,165 L223,168 L225,173 L220,170 L215,173 L217,168 L213,165 L218,165 Z"/>
            <circle cx="170" cy="155" r="3"/>
            <circle cx="230" cy="125" r="3"/>
            <circle cx="185" cy="170" r="2.5"/>
            <circle cx="215" cy="110" r="2.5"/>
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

<!-- WhatsApp Floating Button / Bouton WhatsApp flottant -->
<a href="https://wa.me/5511999999999" class="whatsapp-float" target="_blank">
  📱
</a>