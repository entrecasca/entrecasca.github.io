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
    max-width: 120px;
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
    background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('{{ "/assets/images/stock_oficina.jpg" | relative_url }}');
    background-size: cover;
    background-position: center;
    height: 70vh;
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

.btn {
    background: #E91E63;
    color: white;
    padding: 1rem 2rem;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    display: inline-block;
    transition: background 0.3s;
}

.btn:hover {
    background: #C2185B;
    color: white;
}

/* SERVICES */
.services {
    padding: 4rem 0;
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
    color: #1A1A1A;
}

.section-subtitle {
    text-align: center;
    font-size: 1.1rem;
    color: #666;
    margin-bottom: 3rem;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
}

.cards-grid {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
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
    font-size: 1.3rem;
    margin-bottom: 1rem;
    color: #1A1A1A;
}

.card p {
    color: #666;
    margin-bottom: 1.5rem;
    line-height: 1.6;
}

.card .btn {
    font-size: 0.9rem;
    padding: 0.75rem 1.5rem;
}

/* CONTACT */
.contact {
    background: #1A1A1A;
    color: white;
    padding: 3rem 0;
    text-align: center;
}

.contact h2 {
    font-size: 2rem;
    margin-bottom: 1rem;
}

.contact p {
    font-size: 1.1rem;
    margin-bottom: 2rem;
    color: #ccc;
}

.contact-form {
    max-width: 500px;
    margin: 0 auto;
    display: flex;
    gap: 1rem;
}

.contact-form input {
    flex: 1;
    padding: 1rem;
    border: none;
    border-radius: 5px;
    font-size: 1rem;
}

.contact-form button {
    background: #E91E63;
    color: white;
    border: none;
    padding: 1rem 2rem;
    border-radius: 5px;
    cursor: pointer;
    font-weight: bold;
    transition: background 0.3s;
}

.contact-form button:hover {
    background: #C2185B;
}

/* WhatsApp Button */
.whatsapp {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background: #25D366;
    color: white;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    text-decoration: none;
    font-size: 1.5rem;
    box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    z-index: 1000;
    transition: transform 0.3s;
}

.whatsapp:hover {
    transform: scale(1.1);
    color: white;
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
    }

    .contact-form {
        flex-direction: column;
    }

    .whatsapp {
        width: 50px;
        height: 50px;
        bottom: 15px;
        right: 15px;
        font-size: 1.2rem;
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
            <li><a href="#services">Aulas</a></li>
            <li><a href="#services">Criações</a></li>
            <li><a href="#contact">Contato</a></li>
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
        <h2 class="section-title">Nossos Serviços</h2>
        <p class="section-subtitle">Do aprendizado à criação, oferecemos experiências completas em marcenaria artesanal</p>
        
        <div class="cards-grid">
            <div class="card">
                <img src="{{ '/assets/images/escrivaninha_pinceis.jpg' | relative_url }}" alt="Oficinas Práticas">
                <div class="card-content">
                    <h3>Oficinas Práticas</h3>
                    <p>Oficinas intensivas para todos os níveis, onde você aprende fazendo. Técnicas tradicionais e modernas em um ambiente colaborativo.</p>
                    <a href="#" class="btn">Ver Oficinas</a>
                </div>
            </div>

            <div class="card">
                <img src="{{ '/assets/images/cortando_madeira.jpg' | relative_url }}" alt="Aulas Personalizadas">
                <div class="card-content">
                    <h3>Aulas Personalizadas</h3>
                    <p>Aulas individuais ou em pequenos grupos, focadas nas suas necessidades específicas e ritmo de aprendizado.</p>
                    <a href="#" class="btn">Agendar Aula</a>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Contact -->
<section class="contact" id="contact">
    <div class="container">
        <h2>Entre em Contato</h2>
        <p>Interessado em nossos serviços? Envie seu email e entraremos em contato!</p>
        
        <form class="contact-form" name="contact" method="POST" data-netlify="true">
            <input type="email" name="email" placeholder="Seu email..." required>
            <button type="submit">Enviar</button>
            <input type="hidden" name="form-name" value="contact">
        </form>
    </div>
</section>

<!-- WhatsApp -->
<a href="https://wa.me/5511999999999" class="whatsapp" target="_blank">💬</a>

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

// Form handling
document.querySelector('.contact-form').addEventListener('submit', function(e) {
    const button = this.querySelector('button');
    button.textContent = 'Enviando...';
    button.disabled = true;
});
</script>