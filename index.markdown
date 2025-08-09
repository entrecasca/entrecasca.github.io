---
layout: single
title: "Bem-vindos ao Entre Casca"
header:
  overlay_color: "#F8F9FA"
  overlay_filter: "0.3"
  overlay_image: /assets/images/workshop-header.jpg
  excerpt: "Transformando madeira em arte há mais de 10 anos"
classes: wide
---

<style>
/* Importação da fonte Montserrat / Import de la police Montserrat */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap');

/* Configuração global da fonte / Configuration globale de la police */
body {
  font-family: 'Montserrat', sans-serif;
}

h1, h2, h3, h4, h5, h6 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
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
  opacity: 0.25;
  pointer-events: none;
}

/* Container das cartas em grid / Conteneur des cartes en grille */
.cards-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
  padding: 0 1rem;
}

/* Estilo das cartas principais / Style des cartes principales */
.card {
  position: relative;
  height: 350px;
  border-radius: 8px;
  overflow: hidden;
  cursor: pointer;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
}

/* Efeito hover das cartas / Effet hover des cartes */
.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 35px rgba(0,0,0,0.2);
}

/* Imagem de fundo das cartas / Image de fond des cartes */
.card-image {
  width: 100%;
  height: 100%;
  background-size: cover;
  background-position: center;
  transition: transform 0.3s ease;
}

.card:hover .card-image {
  transform: scale(1.1);
}

/* Overlay que aparece no hover / Overlay qui apparaît au survol */
.card-overlay {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(135deg, rgba(248, 249, 250, 0.95), rgba(255, 251, 240, 0.9));
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  opacity: 0;
  transition: opacity 0.3s ease;
  text-align: center;
  padding: 2rem;
}

.card:hover .card-overlay {
  opacity: 1;
}

/* Título das cartas / Titre des cartes */
.card-title {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0,0,0,0.8));
  color: white;
  padding: 2rem 1.5rem 1.5rem;
  font-size: 1.5rem;
  font-weight: 600;
  font-family: 'Montserrat', sans-serif;
  text-align: center;
}

/* Texto descritivo no overlay / Texte descriptif dans l'overlay */
.card-text {
  color: #495057;
  font-size: 1.1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  line-height: 1.6;
  margin-bottom: 1rem;
}

/* Botões das cartas / Boutons des cartes */
.card-button {
  background: #E91E63;
  color: white;
  padding: 0.8rem 2rem;
  border: none;
  border-radius: 4px;
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
  font-size: 0.95rem;
  transition: all 0.3s ease;
  text-decoration: none;
  display: inline-block;
  letter-spacing: 0.5px;
}

.card-button:hover {
  background: #C2185B;
  transform: scale(1.05);
  color: white;
  text-decoration: none;
}

/* Seção de introdução / Section d'introduction */
.intro-section {
  text-align: center;
  max-width: 800px;
  margin: 0 auto 3rem;
  padding: 0 1rem;
}

.intro-section h2 {
  color: #495057;
  margin-bottom: 1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 600;
}

.intro-section p {
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  font-size: 1.1rem;
  line-height: 1.7;
}

/* Responsividade para mobile / Responsive pour mobile */
@media (max-width: 768px) {
  .cards-container {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .card {
    height: 300px;
  }
  
  .card-title {
    font-size: 1.3rem;
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

<div class="intro-section">
  <!-- Cabeçalho principal / En-tête principal -->
  <h2>Descubra o Mundo da Marcenaria</h2>
  <p>Oferecemos oficinas práticas, aulas especializadas e criamos peças únicas originais. Explore nossos serviços e descubra como podemos ajudar a desenvolver suas habilidades em marcenaria.</p>
</div>

<div class="cards-container">
  <!-- Card 1: Nossas Oficinas / Carte 1: Nos Ateliers -->
  <div class="card" onclick="location.href='/oficinas/'">
    <div class="card-image" style="background-image: url('{{ "/assets/images/oficina_tropical.jpg" | relative_url }}')"></div>
    <div class="card-title">Nossas Oficinas</div>
    <div class="card-overlay">
      <div class="card-text">
        Oficinas práticas para todos os níveis. Aprenda técnicas tradicionais e modernas em um ambiente acolhedor e criativo.
      </div>
      <a href="/oficinas/" class="card-button">Ver Oficinas</a>
    </div>
  </div>

  <!-- Card 2: Aula de Marcenaria / Carte 2: Cours de Menuiserie -->
  <div class="card" onclick="location.href='/aulas/'">
    <div class="card-image" style="background-image: url('{{ "/assets/images/aula_marcenaria.png" | relative_url }}')"></div>
    <div class="card-title">Aulas de Marcenaria</div>
    <div class="card-overlay">
      <div class="card-text">
        Aulas personalizadas individuais ou em grupo. Reserve seu horário e venha aprender técnicas específicas com nossos especialistas.
      </div>
      <a href="/aulas/" class="card-button">Reservar Aula</a>
    </div>
  </div>

  <!-- Card 3: Criações Originais / Carte 3: Créations Originales -->
  <div class="card" onclick="location.href='/criacoes/'">
    <div class="card-image" style="background-image: url('{{ "/assets/images/banco_bandeirola.webp" | relative_url }}')"></div>
    <div class="card-title">Criações Originais</div>
    <div class="card-overlay">
      <div class="card-text">
        Descubra nosso portfólio de peças únicas e originais. Cada criação conta uma história e está disponível para aquisição.
      </div>
      <a href="/criacoes/" class="card-button">Ver Portfólio</a>
    </div>
  </div>

  <!-- Card 4: Saiba Mais / Carte 4: En Savoir Plus -->
  <div class="card" onclick="location.href='/sobre/'">
    <div class="card-image" style="background-image: url('{{ "/assets/images/madeiras_patchwork.webp" | relative_url }}')"></div>
    <div class="card-title">Saiba Mais</div>
    <div class="card-overlay">
      <div class="card-text">
        Conheça nossa história, filosofia e equipe. Descubra por que somos referência em marcenaria artesanal e criativa.
      </div>
      <a href="/sobre/" class="card-button">Nossa História</a>
    </div>
  </div>
</div>

<!-- Seção Newsletter / Section Newsletter -->
<div style="text-align: center; margin: 4rem 0; padding: 3rem; background: linear-gradient(135deg, #F8F9FA, #FFFBF0); border-radius: 8px; border: 1px solid #E9ECEF;">
  <h3 style="color: #495057; margin-bottom: 1rem; font-weight: 600;">Fique por dentro</h3>
  <p style="margin-bottom: 2rem; font-size: 1.1rem; color: #6C757D;">Receba em primeira mão as nossas novidades</p>
  
  <form name="newsletter" method="POST" data-netlify="true" style="max-width: 400px; margin: 0 auto;">
    <div style="display: flex; gap: 10px; flex-wrap: wrap; justify-content: center;">
      <input type="email" 
             name="email" 
             placeholder="Seu melhor email..." 
             required
             style="flex: 1; min-width: 250px; padding: 1rem; border: 2px solid #E9ECEF; border-radius: 4px; font-size: 1rem; outline: none; transition: all 0.3s ease; background: white;"
             onfocus="this.style.borderColor='#E91E63'; this.style.boxShadow='0 0 0 3px rgba(233, 30, 99, 0.1)'"
             onblur="this.style.borderColor='#E9ECEF'; this.style.boxShadow='none'">
      <button type="submit" 
              style="background: linear-gradient(135deg, #E91E63, #C2185B); color: white; padding: 1rem 2rem; border: none; border-radius: 4px; font-weight: 600; cursor: pointer; transition: all 0.3s ease; font-size: 1rem; box-shadow: 0 4px 14px rgba(233, 30, 99, 0.3);"
              onmouseover="this.style.transform='translateY(-2px)'; this.style.boxShadow='0 6px 20px rgba(233, 30, 99, 0.4)'" 
              onmouseout="this.style.transform='translateY(0px)'; this.style.boxShadow='0 4px 14px rgba(233, 30, 99, 0.3)'">
        Inscrever
      </button>
    </div>
    <input type="hidden" name="form-name" value="newsletter">
  </form>
</div>