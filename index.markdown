---
layout: default
title: "Entre Casca"
---

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    color: #333;
}

/* Hide Jekyll default elements */
.masthead, .page__hero, .page__hero--overlay {
    display: none !important;
}

/* NAVIGATION */
.custom-nav {
    background: #1A1A1A;
    padding: 1rem 0;
    position: sticky;
    top: 0;
    z-index: 100;
}

.nav-container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.nav-logo {
    color: white;
    font-size: 1.5rem;
    font-weight: bold;
    text-decoration: none;
}

.nav-logo img {
    height: 40px;
    width: auto;
    max-width: 100%;
    display: block;
}

.nav-menu {
    display: flex;
    list-style: none;
    gap: 2rem;
    margin: 0;
}

.nav-menu a {
    color: #ccc;
    text-decoration: none;
    transition: color 0.3s;
}

.nav-menu a:hover {
    color: #E91E63;
}

.menu-toggle {
    display: none;
    background: none;
    border: none;
    color: white;
    font-size: 1.5rem;
    cursor: pointer;
}

/* HERO */
.hero {
    background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('{{ "/assets/images/painel_de_ferramenta.jpg" | relative_url }}');
    background-size: cover;
    background-position: center;
    height: 50vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: white;
}

.hero-content h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
    text-shadow: 2px 2px 4px rgba(0,0,0,0.7);
}

.hero-content p {
    font-size: 1.2rem;
    margin-bottom: 2rem;
    max-width: 600px;
}

a:visited {
    color: #ffffff;
} 

.btn {
    background: #000000;
    color: white;
    padding: 1rem 2rem;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    display: inline-block;
    transition: background 0.3s;
}

.btn:hover {
    background: #FAC200;
    color: white;
}

/* SERVICES */
.services {
    padding: 2rem 0;
    background: #f8f8f8;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

.section-title {
    text-align: center;
    font-size: 2.5rem;
    margin-bottom: 1rem;
    margin-top: 1rem;
    color: #1A1A1A;
}

.section-subtitle {
    text-align: center;
    font-size: 1.1rem;
    color: #666;
    margin-bottom: 2rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
}

.cards-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-bottom: 3rem;
}

.card {
    background: white;
    border-radius: 10px;
    overflow: hidden;
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
    transition: transform 0.3s;
}

.card:hover {
    transform: translateY(-5px);
}

.card img {
    width: 100%;
    height: 250px;
    object-fit: cover;
}

.card-content {
    padding: 1.5rem;
}

.card h3 {
    margin: 0.5em 0 0.5em;
    font-size: 1.2rem;
    margin-bottom: 1rem;
    color: #1A1A1A;
}

.card p {
    color: #666;
    margin-bottom: 1.5rem;
    line-height: 1.6;
    font-size: 1rem;
}

.card .btn {
    font-size: 0.9rem;
    padding: 0.75rem 1.5rem;
}

/* QUEM SOMOS */
.quem-somos {
    padding: 2rem 0;
    background: white;
}

.quem-somos-content {
    text-align: center;
    margin-bottom: 2rem;
}

.quem-somos h2 {
    font-size: 2.5rem;
    margin-bottom: 1rem;
    margin-top: 1rem;
    color: #1A1A1A;
}

.quem-somos-text {
    font-size: 1.1rem;
    color: #666;
    max-width: 800px;
    margin: 0 auto;
    line-height: 1.7;
}

.gallery {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 1rem;
    margin-top: 2rem;
}

.gallery-item {
    aspect-ratio: 1;
    overflow: hidden;
    border-radius: 8px;
    transition: transform 0.3s;
}

.gallery-item:hover {
    transform: scale(1.05);
}

.gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
}

/* WhatsApp Button */
.whatsapp {
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    box-shadow: 0 4px 12px rgba(0,0,0,0);
    z-index: 1000;
    transition: transform 0.3s;
    overflow: hidden;
}

.whatsapp:hover {
    transform: scale(1.1);
}

/* MOBILE */
@media (max-width: 768px) {
    .menu-toggle {
        display: block;
    }

    .nav-menu {
        display: none;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: #1A1A1A;
        flex-direction: column;
        padding: 1rem;
        gap: 1rem;
    }

    .nav-menu.active {
        display: flex;
    }

    .hero-content h1 {
        font-size: 2rem;
    }

    .hero-content p {
        font-size: 1rem;
    }

    .cards-grid {
        grid-template-columns: 1fr;
        gap: 1.5rem;
    }

    .section-title {
        font-size: 2rem;
        margin-top: 1rem;
    }

    .gallery {
        grid-template-columns: repeat(2, 1fr);
        gap: 0.75rem;
    }

    .whatsapp {
        width: 50px;
        height: 50px;
        bottom: 15px;
        right: 15px;
    }
}
</style>

<!-- Navigation -->
<nav class="custom-nav">
    <div class="nav-container">
        <a href="#" class="nav-logo"><img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Entre Casca">
</a>
        <button class="menu-toggle" onclick="toggleMenu()">☰</button>
        <ul class="nav-menu" id="navMenu">
            <li><a href="#services">Oficinas</a></li>
            <li><a href="#quem-somos">Quem Somos</a></li>
            <li><a href="https://wa.me/5519989801351">Contato</a></li>
        </ul>
    </div>
</nav>

<!-- Hero -->
<section class="hero">
    <div class="hero-content">
        <h1>Entre Casca</h1>
        <p>Ateliê de marcenaria artesanal onde transformamos madeira em arte há mais de 10 anos</p>
        <a href="#services" class="btn">Descobrir Serviços</a>
    </div>
</section>

<!-- Services -->
<section class="services" id="services">
    <div class="container">
        <h2 class="section-title">Nossas Oficinas</h2>
        <p class="section-subtitle">Do aprendizado à criação, oferecemos experiências completas em marcenaria artesanal</p>
        
        <div class="cards-grid">
            <div class="card">
                <img src="{{ '/assets/images/bandeirola.png' | relative_url }}" alt="Oficina De Banco Bandeirola">
                <div class="card-content">
                    <h3>Oficina de Banco Bandeirola</h3>
                    <p>Talvez o banco mais brasileiro que existe, fiel companheiro das obras que levantam este Brasil.</p>
                    <a href="{{ '/oficina-banco-bandeirola' | relative_url }}" class="btn">Ver Oficina</a>                
                </div>
            </div>

            <div class="card">
                <img src="{{ '/assets/images/composteira.jpeg' | relative_url }}" alt="Aulas Personalizadas">
                <div class="card-content">
                    <h3>Oficina de Composteira</h3>
                    <p>ESPERANDO O LUCAS</p>
                    <a href="#" class="btn">Ver Oficina</a>
                </div>
            </div>
            <div class="card">
                <img src="{{ '/assets/images/abelhas.jpeg' | relative_url }}" alt="Aulas Personalizadas">
                <div class="card-content">
                    <h3>Oficina Semeando Meliponários</h3>
                    <p>Com a chegada da Primavera, convidamos você para uma oficina especial de construção de meliponários.</p>
                    <a href="#" class="btn">Ver Oficina</a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Quem Somos -->
<section class="quem-somos" id="quem-somos">
    <div class="container">
        <div class="quem-somos-content">
            <h2>Quem Somos</h2>
            <p class="quem-somos-text">
                Há mais de 10 anos, o Entre Casca é um ateliê de marcenaria artesanal dedicado a transformar madeira em arte. 
                Nosso espaço é onde tradição e criatividade se encontram, oferecendo oficinas que ensinam técnicas ancestrais 
                de marcenaria enquanto criamos peças únicas e funcionais. Acreditamos que trabalhar com madeira é uma forma 
                de conexão com a natureza e com nossa própria essência criativa.
            </p>
        </div>
        
        <div class="gallery">
            <div class="gallery-item">
                <img src="{{ '/assets/images/ping_pong.jpg' | relative_url }}" alt="Ateliê Entre Casca">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/oficina_falando.jpeg' | relative_url }}" alt="Oficina de marcenaria">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/suporte_planta.jpg' | relative_url }}" alt="Ferramentas artesanais">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/movel_pia.jpg' | relative_url }}" alt="Peças em madeira">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/casa_criança.jpg' | relative_url }}" alt="Processo criativo">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/caixinha.jpg' | relative_url }}" alt="Detalhes em madeira">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/oficina_folha.jpg' | relative_url }}" alt="Trabalho artesanal">
            </div>
            <div class="gallery-item">
                <img src="{{ '/assets/images/super_mesa.jpg' | relative_url }}" alt="Ateliê em ação">
            </div>
        </div>
    </div>
</section>

<!-- WhatsApp -->
<a href="https://wa.me/5519989801351" class="whatsapp" target="_blank">
    <img src="{{ '/assets/images/whatsapp.webp' | relative_url }}" alt="WhatsApp">
</a>

<script>
function toggleMenu() {
    const menu = document.getElementById('navMenu');
    menu.classList.toggle('active');
}

// Close menu when clicking on links
document.querySelectorAll('.nav-menu a').forEach(link => {
    link.addEventListener('click', () => {
        document.getElementById('navMenu').classList.remove('active');
    });
});

// Smooth scroll
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({ behavior: 'smooth' });
        }
    });
});
</script>