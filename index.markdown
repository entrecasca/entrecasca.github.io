---
layout: single
title: "Entre Casca"
header:
  overlay_color: "#FFFFFF"
  overlay_filter: "0.1"
  overlay_image: /assets/images/workshop-header.jpg
  excerpt: "Ateliê de marcenaria artesanal"
classes: wide
---

<style>
/* Importação da fonte Montserrat / Import de la police Montserrat */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap');

/* Reset e configuração global / Reset et configuration globale */
* {
  box-sizing: border-box;
}

body {
  font-family: 'Montserrat', sans-serif;
  line-height: 1.6;
  color: #333;
  background: #FFFFFF;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  color: #2C2C2C;
}

/* Bandeira grande de fundo / Grand drapeau d'arrière-plan */
.background-flag {
  position: fixed;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  min-width: 100vw;
  min-height: 100vh;
  width: 120vw;
  height: auto;
  z-index: -1;
  opacity: 0.08;
  pointer-events: none;
}

/* Hero section estilo oficina.cc / Hero section style oficina.cc */
.hero-section {
  text-align: center;
  padding: 6rem 2rem 4rem;
  background: linear-gradient(135deg, #FAFAFA 0%, #F5F5F5 100%);
  margin: -3rem -2rem 0;
}

.hero-title {
  font-size: 4rem;
  font-weight: 700;
  color: #2C2C2C;
  margin-bottom: 1rem;
  letter-spacing: -0.02em;
}

.hero-subtitle {
  font-size: 1.5rem;
  font-weight: 300;
  color: #666;
  margin-bottom: 2rem;
  max-width: 600px;
  margin-left: auto;
  margin-right: auto;
}

.hero-description {
  font-size: 1.1rem;
  color: #666;
  max-width: 700px;
  margin: 0 auto 3rem;
  line-height: 1.8;
}

/* Botão CTA principal / Bouton CTA principal */
.cta-button {
  display: inline-block;
  background: #E91E63;
  color: white;
  padding: 1.2rem 3rem;
  font-size: 1.1rem;
  font-weight: 600;
  text-decoration: none;
  border-radius: 6px;
  transition: all 0.3s ease;
  letter-spacing: 0.5px;
  margin-bottom: 4rem;
}

.cta-button:hover {
  background: #C2185B;
  transform: translateY(-2px);
  box-shadow: 0 8px 25px rgba(233, 30, 99, 0.3);
  color: white;
  text-decoration: none;
}

/* Grid de serviços estilo oficina.cc / Grille de services style oficina.cc */
.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  gap: 3rem;
  max-width: 1200px;
  margin: 4rem auto;
  padding: 0 2rem;
}

.service-card {
  background: white;
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 4px 20px rgba(0,0,0,0.08);
  transition: all 0.3s ease;
  border: 1px solid #F0F0F0;
}

.service-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 12px 40px rgba(0,0,0,0.15);
}

.service-image {
  width: 100%;
  height: 250px;
  background-size: cover;
  background-position: center;
  position: relative;
}

.service-content {
  padding: 2rem;
}

.service-title {
  font-size: 1.5rem;
  font-weight: 600;
  color: #2C2C2C;
  margin-bottom: 1rem;
}

.service-description {
  color: #666;
  line-height: 1.7;
  margin-bottom: 1.5rem;
}

.service-link {
  color: #E91E63;
  font-weight: 600;
  text-decoration: none;
  font-size: 0.95rem;
  letter-spacing: 0.5px;
  transition: color 0.3s ease;
}

.service-link:hover {
  color: #C2185B;
  text-decoration: none;
}

/* About section / Section à propos */
.about-section {
  background: #FAFAFA;
  padding: 6rem 2rem;
  margin: 4rem -2rem 0;
  text-align: center;
}

.about-content {
  max-width: 800px;
  margin: 0 auto;
}

.about-title {
  font-size: 2.5rem;
  font-weight: 600;
  color: #2C2C2C;
  margin-bottom: 2rem;
}

.about-text {
  font-size: 1.1rem;
  color: #666;
  line-height: 1.8;
  margin-bottom: 2rem;
}

/* Newsletter section minimaliste / Section newsletter minimaliste */
.newsletter-section {
  background: white;
  padding: 4rem 2rem;
  text-align: center;
  border-top: 1px solid #E5E5E5;
}

.newsletter-title {
  font-size: 2rem;
  font-weight: 600;
  color: #2C2C2C;
  margin-bottom: 1rem;
}

.newsletter-description {
  color: #666;
  font-size: 1.1rem;
  margin-bottom: 2.5rem;
  max-width: 500px;
  margin-left: auto;
  margin-right: auto;
}

.newsletter-form {
  display: flex;
  max-width: 400px;
  margin: 0 auto;
  gap: 1rem;
  flex-wrap: wrap;
  justify-content: center;
}

.newsletter-input {
  flex: 1;
  min-width: 250px;
  padding: 1rem 1.5rem;
  border: 2px solid #E5E5E5;
  border-radius: 6px;
  font-size: 1rem;
  outline: none;
  transition: border-color 0.3s ease;
  font-family: 'Montserrat', sans-serif;
}

.newsletter-input:focus {
  border-color: #E91E63;
}

.newsletter-button {
  background: #E91E63;
  color: white;
  padding: 1rem 2rem;
  border: none;
  border-radius: 6px;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
  font-size: 1rem;
  font-family: 'Montserrat', sans-serif;
}

.newsletter-button:hover {
  background: #C2185B;
  transform: translateY(-2px);
}

/* Responsividade / Responsive */
@media (max-width: 768px) {
  .hero-title {
    font-size: 2.5rem;
  }
  
  .hero-subtitle {
    font-size: 1.2rem;
  }
  
  .services-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
    padding: 0 1rem;
  }
  
  .hero-section,
  .about-section,
  .newsletter-section {
    padding-left: 1rem;
    padding-right: 1rem;
  }
  
  .newsletter-form {
    flex-direction: column;
    align-items: center;
  }
  
  .newsletter-input {
    width: 100%;
    min-width: auto;
  }
}
</style>

<!-- Bandeira grande de fundo da Mangueira / Grand drapeau d'arrière-plan de la Mangueira -->
<div class="background-flag">
  <svg viewBox="0 0 400 280" xmlns="http://www.w3.org/2000/svg" style="width: 100%; height: auto;">
    <!-- Fundo rosa/magenta Mangueira / Background rose/magenta Mangueira -->
    <rect width="400" height="280" fill="#E91E63"/>
    
    <!-- Padrões tribais de fundo / Motifs tribaux en arrière-plan -->
    <defs>
      <pattern id="tribalPatternBg" x="0" y="0" width="40" height="40" patternUnits="userSpaceOnUse">
        <path d="M20,5 L35,20 L20,35 L5,20 Z" fill="none" stroke="#C2185B" stroke-width="1" opacity="0.5"/>
        <circle cx="20" cy="20" r="3" fill="#C2185B" opacity="0.3"/>
      </pattern>
      
      <pattern id="barkTextureBg" x="0" y="0" width="20" height="20" patternUnits="userSpaceOnUse">
        <path d="M0,10 Q5,5 10,10 T20,10" fill="none" stroke="#C2185B" stroke-width="0.8" opacity="0.3"/>
        <path d="M0,15 Q5,12 10,15 T20,15" fill="none" stroke="#C2185B" stroke-width="0.8" opacity="0.3"/>
      </pattern>
    </defs>
    
    <rect width="400" height="280" fill="url(#tribalPatternBg)"/>
    <rect width="400" height="280" fill="url(#barkTextureBg)"/>
    
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

<!-- Hero Section -->
<section class="hero-section">
  <h1 class="hero-title">Entre Casca</h1>
  <p class="hero-subtitle">Ateliê de marcenaria artesanal</p>
  <p class="hero-description">
    Transformamos madeira em arte há mais de 10 anos. Oferecemos oficinas práticas, aulas especializadas e criamos peças únicas originais que contam histórias através da madeira.
  </p>
  <a href="#servicos" class="cta-button">Descubra nossos serviços</a>
</section>

<!-- Services Grid -->
<section id="servicos" class="services-grid">
  <div class="service-card">
    <div class="service-image" style="background-image: url('/assets/images/oficinas_grupo.webp')"></div>
    <div class="service-content">
      <h3 class="service-title">Nossas Oficinas</h3>
      <p class="service-description">
        Oficinas práticas para todos os níveis. Aprenda técnicas tradicionais e modernas em um ambiente acolhedor e criativo, desenvolvendo suas habilidades com a madeira.
      </p>
      <a href="/oficinas/" class="service-link">Ver todas as oficinas →</a>
    </div>
  </div>

  <div class="service-card">
    <div class="service-image" style="background-image: url('/assets/images/oficina_tropical.webp')"></div>
    <div class="service-content">
      <h3 class="service-title">Aulas de Marcenaria</h3>
      <p class="service-description">
        Aulas personalizadas individuais ou em grupo. Reserve seu horário e venha aprender técnicas específicas com nossos especialistas em marcenaria.
      </p>
      <a href="/aulas/" class="service-link">Reservar uma aula →</a>
    </div>
  </div>

  <div class="service-card">
    <div class="service-image" style="background-image: url('/assets/images/banco_bandeirola.webp')"></div>
    <div class="service-content">
      <h3 class="service-title">Criações Originais</h3>
      <p class="service-description">
        Descubra nosso portfólio de peças únicas e originais. Cada criação conta uma história e está disponível para aquisição por colecionadores e amantes da madeira.
      </p>
      <a href="/criacoes/" class="service-link">Explorar portfólio →</a>
    </div>
  </div>
</section>

<!-- About Section -->
<section class="about-section">
  <div class="about-content">
    <h2 class="about-title">Nossa História</h2>
    <p class="about-text">
      O Entre Casca nasceu da paixão pela madeira e pelo artesanato brasileiro. Há mais de uma década, criamos um espaço onde tradição e inovação se encontram, oferecendo experiências únicas de aprendizado e criação.
    </p>
    <p class="about-text">
      Nosso ateliê é mais que um local de trabalho - é um ponto de encontro para artesãos, aprendizes e amantes da marcenaria que compartilham o amor pela transformação da madeira em arte.
    </p>
    <a href="/sobre/" class="cta-button">Conheça nossa equipe</a>
  </div>
</section>

<!-- Newsletter Section -->
<section class="newsletter-section">
  <h3 class="newsletter-title">Fique por dentro</h3>
  <p class="newsletter-description">
    Receba em primeira mão as nossas novidades, dicas de marcenaria e informações sobre novas oficinas.
  </p>
  
  <form name="newsletter" method="POST" data-netlify="true" class="newsletter-form">
    <input type="email" 
           name="email" 
           placeholder="Seu melhor email..." 
           required
           class="newsletter-input">
    <button type="submit" class="newsletter-button">
      Inscrever-se
    </button>
    <input type="hidden" name="form-name" value="newsletter">
  </form>
</section>