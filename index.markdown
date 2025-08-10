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

<!-- 
  EXPLICAÇÃO GERAL:
  Este é um site para um ateliê de marcenaria chamado "Entre Casca".
  O código está dividido em 3 partes principais:
  1. CSS (estilo/aparência) - dentro da tag <style>
  2. HTML (estrutura/conteúdo) - as seções visíveis do site
  3. JavaScript (interatividade) - dentro da tag <script>
-->

<style>
    /* ===================================
       SEÇÃO 1: IMPORTAÇÃO DE FONTES
       =================================== */
    
    /* Importa fontes do Google Fonts para deixar o texto mais bonito */
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap');

    /* ===================================
       SEÇÃO 2: CONFIGURAÇÕES BÁSICAS
       =================================== */
    
    /* Remove margens e espaçamentos padrão de todos os elementos */
    * {
      box-sizing: border-box; /* Faz com que padding e border sejam incluídos no tamanho total */
      margin: 0;  /* Remove margem externa */
      padding: 0; /* Remove espaçamento interno */
    }

    /* Configurações gerais do corpo da página */
    body {
      font-family: 'Inter', sans-serif; /* Define a fonte principal */
      line-height: 1.6;                /* Espaçamento entre linhas do texto */
      color: #2C2C2C;                  /* Cor do texto (cinza escuro) */
      background: #FAFAFA;             /* Cor de fundo da página (cinza bem claro) */
      overflow-x: hidden;              /* Esconde barra de rolagem horizontal se aparecer */
    }

    /* Configurações para todos os títulos (h1, h2, h3, etc.) */
    h1, h2, h3, h4, h5, h6 {
      font-family: 'Montserrat', sans-serif; /* Fonte diferente para títulos */
      font-weight: 600;                      /* Peso da fonte (mais grosso) */
      color: #1A1A1A;                        /* Cor dos títulos (preto) */
    }

    /* ===================================
       SEÇÃO 3: CONTAINER PRINCIPAL
       =================================== */
    
    /* Container que centraliza o conteúdo e define largura máxima */
    .main-container {
      max-width: 1400px;  /* Largura máxima do conteúdo */
      margin: 0 auto;     /* Centraliza horizontalmente */
      padding: 0 2rem;    /* Espaçamento interno nas laterais */
    }

    /* ===================================
       SEÇÃO 4: NAVEGAÇÃO (MENU DO TOPO)
       =================================== */
    
    /* Barra de navegação no topo da página */
    .top-nav {
      background: #1A1A1A;    /* Fundo preto */
      color: white;           /* Texto branco */
      padding: 1rem 0;        /* Espaçamento interno vertical */
      position: sticky;       /* Fica grudado no topo quando rola a página */
      top: 0;                 /* Posição do topo */
      z-index: 1000;          /* Fica por cima de outros elementos */
      box-shadow: 0 2px 10px rgba(0,0,0,0.1); /* Sombra sutil embaixo */
    }

    /* Container interno da navegação */
    .nav-content {
      max-width: 1400px;           /* Largura máxima */
      margin: 0 auto;              /* Centraliza */
      padding: 0 2rem;             /* Espaçamento lateral */
      display: flex;               /* Layout flexível */
      justify-content: space-between; /* Espaça elementos nas extremidades */
      align-items: center;         /* Alinha verticalmente no centro */
    }

    /* Área do logo */
    .logo {
      display: flex;        /* Layout flexível */
      align-items: center;  /* Alinha verticalmente */
    }

    /* Imagem do logo */
    .logo img {
      height: 40px;                    /* Altura da imagem */
      width: auto;                     /* Largura automática (mantém proporção) */
      transition: opacity 0.3s ease;   /* Efeito suave de transição */
    }

    /* Botão do menu para celular (inicialmente escondido) */
    .mobile-menu-toggle {
      display: none;        /* Escondido por padrão */
      background: none;     /* Sem fundo */
      border: none;         /* Sem borda */
      color: white;         /* Texto branco */
      font-size: 1.5rem;    /* Tamanho da fonte */
      cursor: pointer;      /* Cursor vira mãozinha ao passar por cima */
      padding: 0.5rem;      /* Espaçamento interno */
    }

    /* Lista de links do menu */
    .nav-links {
      display: flex;    /* Layout em linha */
      gap: 2rem;        /* Espaço entre os itens */
      list-style: none; /* Remove bolinhas da lista */
      margin: 0;        /* Remove margem */
      padding: 0;       /* Remove espaçamento */
    }

    /* Links individuais do menu */
    .nav-links a {
      color: #CCCCCC;                  /* Cor cinza claro */
      text-decoration: none;           /* Remove sublinhado */
      font-weight: 500;                /* Peso da fonte */
      transition: color 0.3s ease;     /* Efeito suave na mudança de cor */
      font-size: 0.95rem;              /* Tamanho da fonte */
    }

    /* Efeito quando passa o mouse por cima dos links */
    .nav-links a:hover {
      color: #E91E63;  /* Muda para cor rosa */
    }

    /* ===================================
       SEÇÃO 5: SEÇÃO HERO (BANNER PRINCIPAL)
       =================================== */
    
    /* Seção principal com imagem de fundo e título */
    .hero-section {
       /* Gradiente escuro sobre a imagem para melhor legibilidade do texto */
       background: linear-gradient(rgba(26, 26, 26, 0.6), rgba(26, 26, 26, 0.6)), 
                   url('/assets/images/stock_oficina.jpg') center/cover;
      padding: 8rem 0 6rem;    /* Espaçamento interno grande */
      color: white;            /* Texto branco */
      text-align: center;      /* Texto centralizado */
      position: relative;      /* Posicionamento relativo */
      min-height: 60vh;        /* Altura mínima (60% da altura da tela) */
      display: flex;           /* Layout flexível */
      align-items: center;     /* Centraliza verticalmente */
    }

    /* Container do conteúdo do hero */
    .hero-content {
      max-width: 800px;  /* Largura máxima */
      margin: 0 auto;    /* Centraliza */
      padding: 0 1rem;   /* Espaçamento lateral */
    }

    /* Título principal do site */
    .hero-title {
      font-family: 'Montserrat', sans-serif;        /* Fonte especial */
      font-size: clamp(2rem, 8vw, 3.5rem);          /* Tamanho responsivo */
      font-weight: 700;                             /* Muito grosso */
      color: white;                                 /* Branco */
      margin-bottom: 1.5rem;                        /* Espaço embaixo */
      line-height: 1.2;                             /* Altura da linha */
      text-shadow: 2px 2px 4px rgba(0,0,0,0.3);     /* Sombra no texto */
    }

    /* Subtítulo do hero */
    .hero-subtitle {
      font-size: clamp(1rem, 3vw, 1.3rem);          /* Tamanho responsivo */
      color: rgba(255,255,255,0.9);                 /* Branco quase transparente */
      margin-bottom: 2rem;                          /* Espaço embaixo */
      font-weight: 400;                             /* Peso normal */
      line-height: 1.6;                             /* Altura da linha */
      text-shadow: 1px 1px 2px rgba(0,0,0,0.3);     /* Sombra sutil */
    }

    /* ===================================
       SEÇÃO 6: SEÇÃO DE SERVIÇOS
       =================================== */
    
    /* Seção que mostra os serviços oferecidos */
    .services-section {
      padding: clamp(3rem, 8vw, 6rem) 0;  /* Espaçamento responsivo */
      background: #F8F8F8;               /* Fundo cinza bem claro */
    }

    /* Cabeçalho das seções */
    .section-header {
      text-align: center;                          /* Centralizado */
      margin-bottom: clamp(2rem, 6vw, 4rem);       /* Espaço embaixo responsivo */
      padding: 0 1rem;                            /* Espaçamento lateral */
    }

    /* Título das seções */
    .section-title {
      font-family: 'Montserrat', sans-serif;      /* Fonte especial */
      font-size: clamp(1.8rem, 5vw, 2.5rem);      /* Tamanho responsivo */
      font-weight: 600;                           /* Grosso */
      color: #1A1A1A;                             /* Preto */
      margin-bottom: 1rem;                        /* Espaço embaixo */
    }

    /* Subtítulo das seções */
    .section-subtitle {
      color: #666;                    /* Cinza */
      font-size: clamp(1rem, 2vw, 1.1rem);  /* Tamanho responsivo */
      max-width: 600px;               /* Largura máxima */
      margin: 0 auto;                 /* Centraliza */
    }

    /* Grade de serviços (layout em colunas) */
    .services-grid {
      display: grid;                                                  /* Layout em grade */
      grid-template-columns: repeat(auto-fit, minmax(min(100%, 350px), 1fr)); /* Colunas responsivas */
      gap: 2rem;                                                     /* Espaço entre colunas */
      padding: 0 1rem;                                               /* Espaçamento lateral */
    }

    /* Cartão individual de serviço */
    .service-card {
      background: white;                           /* Fundo branco */
      border-radius: 8px;                         /* Cantos arredondados */
      overflow: hidden;                           /* Esconde conteúdo que vaza */
      box-shadow: 0 2px 12px rgba(0,0,0,0.06);    /* Sombra sutil */
      transition: all 0.3s ease;                  /* Efeito suave */
      border: 1px solid #F0F0F0;                  /* Borda cinza clara */
    }

    /* Efeito quando passa mouse por cima do cartão */
    .service-card:hover {
      transform: translateY(-4px);                /* Move pra cima */
      box-shadow: 0 8px 30px rgba(0,0,0,0.12);    /* Sombra mais forte */
    }

    /* Imagem do serviço */
    .service-image {
        width: 100%;               /* Largura total */
        height: 280px;             /* Altura fixa */
        background-size: cover;    /* Imagem cobre toda a área */
        background-position: center; /* Centraliza a imagem */
        position: relative;        /* Para posicionar elementos filhos */
    }

    /* Etiqueta sobreposta na imagem */
    .service-overlay {
      position: absolute;                    /* Posição absoluta */
      top: 1rem;                            /* Distância do topo */
      left: 1rem;                           /* Distância da esquerda */
      background: rgba(26, 26, 26, 0.8);    /* Fundo preto semitransparente */
      color: white;                         /* Texto branco */
      padding: 0.5rem 1rem;                 /* Espaçamento interno */
      border-radius: 4px;                   /* Cantos arredondados */
      font-size: clamp(0.75rem, 2vw, 0.85rem); /* Tamanho responsivo */
      font-weight: 600;                     /* Grosso */
    }

    /* Conteúdo textual do cartão */
    .service-content {
      padding: clamp(1.5rem, 3vw, 2rem);  /* Espaçamento interno responsivo */
    }

    /* Título do serviço */
    .service-title {
      font-family: 'Montserrat', sans-serif;     /* Fonte especial */
      font-size: clamp(1.2rem, 3vw, 1.5rem);     /* Tamanho responsivo */
      font-weight: 600;                          /* Grosso */
      color: #1A1A1A;                            /* Preto */
      margin-bottom: 1rem;                       /* Espaço embaixo */
    }

    /* Descrição do serviço */
    .service-description {
      color: #666;                               /* Cinza */
      line-height: 1.7;                          /* Altura da linha */
      margin-bottom: 1.5rem;                     /* Espaço embaixo */
      font-size: clamp(0.9rem, 2vw, 1rem);       /* Tamanho responsivo */
    }

    /* Lista de características do serviço */
    .service-features {
      list-style: none;        /* Remove bolinhas */
      padding: 0;              /* Remove espaçamento */
      margin: 0 0 1.5rem 0;    /* Espaço apenas embaixo */
    }

    /* Itens da lista de características */
    .service-features li {
      color: #666;                              /* Cinza */
      font-size: clamp(0.85rem, 2vw, 0.9rem);   /* Tamanho responsivo */
      margin-bottom: 0.5rem;                    /* Espaço embaixo */
      padding-left: 1.2rem;                     /* Espaço para a seta */
      position: relative;                       /* Para posicionar a seta */
    }

    /* Seta antes de cada item da lista */
    .service-features li:before {
      content: "→";        /* Caractere da seta */
      color: #E91E63;      /* Cor rosa */
      font-weight: bold;   /* Grosso */
      position: absolute;  /* Posição absoluta */
      left: 0;            /* Alinhado à esquerda */
    }

    /* Link no final de cada cartão */
    .service-link {
      color: #1A1A1A;                          /* Preto */
      font-weight: 600;                        /* Grosso */
      text-decoration: none;                   /* Sem sublinhado */
      font-size: clamp(0.85rem, 2vw, 0.95rem); /* Tamanho responsivo */
      border-bottom: 2px solid #E91E63;        /* Linha embaixo rosa */
      padding-bottom: 2px;                     /* Espaço entre texto e linha */
      transition: all 0.3s ease;               /* Efeito suave */
      display: inline-block;                   /* Para funcionar o padding */
    }

    /* ===================================
       SEÇÃO 7: SEÇÃO SOBRE
       =================================== */
    
    /* Seção "Sobre nós" */
    .about-section {
      padding: clamp(3rem, 8vw, 6rem) 0;  /* Espaçamento responsivo */
      background: white;                  /* Fundo branco */
    }

    /* Grade de duas colunas (texto e imagem) */
    .about-grid {
      display: grid;                                                  /* Layout em grade */
      grid-template-columns: repeat(auto-fit, minmax(min(100%, 350px), 1fr)); /* Colunas responsivas */
      gap: clamp(2rem, 4vw, 4rem);                                   /* Espaço entre colunas responsivo */
      align-items: center;                                           /* Alinha verticalmente */
      padding: 0 1rem;                                               /* Espaçamento lateral */
    }

    /* Título da seção sobre */
    .about-content h2 {
      font-family: 'Montserrat', sans-serif;       /* Fonte especial */
      font-size: clamp(1.5rem, 4vw, 2.2rem);       /* Tamanho responsivo */
      font-weight: 600;                            /* Grosso */
      color: #1A1A1A;                              /* Preto */
      margin-bottom: 1.5rem;                       /* Espaço embaixo */
      line-height: 1.3;                            /* Altura da linha */
    }

    /* Parágrafos da seção sobre */
    .about-text {
      color: #666;                              /* Cinza */
      line-height: 1.8;                         /* Altura da linha maior */
      margin-bottom: 1.5rem;                    /* Espaço embaixo */
      font-size: clamp(0.95rem, 2vw, 1rem);     /* Tamanho responsivo */
    }

    /* Caixa de destaque com citação */
    .about-highlight {
      background: #FFF8E1;                       /* Fundo amarelo claro */
      border-left: 4px solid #E91E63;            /* Borda esquerda rosa */
      padding: clamp(1rem, 3vw, 1.5rem);         /* Espaçamento interno responsivo */
      margin: 2rem 0;                           /* Espaço em cima e embaixo */
      border-radius: 4px;                       /* Cantos arredondados */
    }

    /* Parágrafo dentro da caixa de destaque */
    .about-highlight p {
      margin: 0;                               /* Remove margem */
      color: #666;                             /* Cinza */
      font-style: italic;                      /* Itálico */
      font-size: clamp(0.9rem, 2vw, 1rem);     /* Tamanho responsivo */
    }

    /* Imagem da seção sobre */
    .about-image {
      width: 100%;                                              /* Largura total */
      height: clamp(250px, 50vw, 400px);                        /* Altura responsiva */
      background: url('/assets/images/madeiras_patchwork.webp') center/cover; /* Imagem de fundo */
      border-radius: 8px;                                      /* Cantos arredondados */
      border: 1px solid #F0F0F0;                               /* Borda cinza clara */
    }

    /* ===================================
       SEÇÃO 8: RODAPÉ
       =================================== */
    
    /* Seção do rodapé */
    .footer-section {
      background: #1A1A1A;                        /* Fundo preto */
      color: white;                               /* Texto branco */
      padding: clamp(2rem, 6vw, 4rem) 0 2rem;     /* Espaçamento responsivo */
      position: relative;                         /* Para posicionar elementos */
    }

    /* Conteúdo principal do rodapé */
    .footer-content {
      display: grid;                    /* Layout em grade */
      grid-template-columns: 1fr auto auto; /* 3 colunas: flexível, auto, auto */
      gap: clamp(1.5rem, 4vw, 3rem);   /* Espaço entre colunas responsivo */
      align-items: center;              /* Alinha verticalmente */
      margin-bottom: 2rem;              /* Espaço embaixo */
      padding: 0 1rem;                  /* Espaçamento lateral */
    }

    /* Área do newsletter */
    .newsletter-content {
      max-width: 500px;  /* Largura máxima */
    }

    /* Título do newsletter */
    .newsletter-title {
      font-family: 'Montserrat', sans-serif;     /* Fonte especial */
      font-size: clamp(1.3rem, 4vw, 2rem);       /* Tamanho responsivo */
      font-weight: 600;                          /* Grosso */
      margin-bottom: 1rem;                       /* Espaço embaixo */
      color: white;                              /* Branco */
    }

    /* Descrição do newsletter */
    .newsletter-description {
      color: #CCCCCC;                            /* Cinza claro */
      font-size: clamp(0.95rem, 2vw, 1.1rem);    /* Tamanho responsivo */
      margin-bottom: 2rem;                       /* Espaço embaixo */
    }

    /* Formulário do newsletter */
    .newsletter-form {
      display: flex;          /* Layout em linha */
      gap: 0;                /* Sem espaço entre elementos */
      border-radius: 6px;     /* Cantos arredondados */
      overflow: hidden;       /* Esconde partes que vazam */
      border: 1px solid #333; /* Borda cinza escura */
      max-width: 500px;       /* Largura máxima */
    }

    /* Campo de entrada do email */
    .newsletter-input {
      flex: 1;                                     /* Ocupa espaço restante */
      padding: clamp(0.75rem, 2vw, 1rem) clamp(1rem, 3vw, 1.5rem); /* Espaçamento interno responsivo */
      border: none;                               /* Sem borda */
      background: #2A2A2A;                        /* Fundo cinza escuro */
      color: white;                               /* Texto branco */
      font-size: clamp(0.9rem, 2vw, 1rem);        /* Tamanho responsivo */
      outline: none;                              /* Remove contorno quando selecionado */
      font-family: 'Inter', sans-serif;           /* Mesma fonte do site */
    }

    /* Botão de inscrição no newsletter */
    .newsletter-button {
      background: #E91E63;                        /* Fundo rosa */
      color: white;                               /* Texto branco */
      padding: clamp(0.75rem, 2vw, 1rem) clamp(1.5rem, 3vw, 2rem); /* Espaçamento interno responsivo */
      border: none;                               /* Sem borda */
      font-weight: 600;                           /* Grosso */
      cursor: pointer;                            /* Cursor vira mãozinha */
      transition: background 0.3s ease;          /* Efeito suave */
      font-size: clamp(0.9rem, 2vw, 1rem);        /* Tamanho responsivo */
      font-family: 'Inter', sans-serif;           /* Mesma fonte do site */
      white-space: nowrap;                        /* Não quebra linha */
    }

    /* Botão do Instagram */
    .instagram-button {
      display: flex;                              /* Layout flexível */
      align-items: center;                        /* Centraliza verticalmente */
      justify-content: center;                    /* Centraliza horizontalmente */
      width: clamp(40px, 8vw, 50px);              /* Largura responsiva */
      height: clamp(40px, 8vw, 50px);             /* Altura responsiva */
      background: linear-gradient(45deg, #833AB4, #FD1D1D, #F77737); /* Gradiente do Instagram */
      color: white;                               /* Ícone branco */
      border-radius: 50%;                         /* Formato circular */
      text-decoration: none;                      /* Sem sublinhado */
      font-size: clamp(1.2rem, 3vw, 1.5rem);      /* Tamanho responsivo */
      transition: transform 0.3s ease;           /* Efeito de movimento */
      flex-shrink: 0;                             /* Não encolhe */
    }

    /* Bandeira no rodapé */
    .footer-flag {
      width: clamp(60px, 12vw, 80px);             /* Largura responsiva */
      height: clamp(42px, 8vw, 56px);             /* Altura responsiva */
      opacity: 0.8;                              /* Um pouco transparente */
      transition: opacity 0.3s ease;             /* Efeito suave */
      flex-shrink: 0;                             /* Não encolhe */
    }

    /* ===================================
       SEÇÃO 9: BOTÃO WHATSAPP FLUTUANTE
       =================================== */
    
    /* Botão do WhatsApp que fica fixo na tela */
    .whatsapp-float {
      position: fixed;                           /* Posição fixa (não rola com a página) */
      bottom: clamp(1rem, 3vw, 2rem);            /* Distância de baixo responsiva */
      right: clamp(1rem, 3vw, 2rem);             /* Distância da direita responsiva */
      width: clamp(50px, 10vw, 60px);            /* Largura responsiva */
      height: clamp(50px, 10vw, 60px);           /* Altura responsiva */
      background: #25D366;                       /* Verde do WhatsApp */
      color: white;                              /* Ícone branco */
      border-radius: 50%;                        /* Formato circular */
      display: flex;                             /* Layout flexível */
      align-items: center;                       /* Centraliza verticalmente */
      justify-content: center;                   /* Centraliza horizontalmente */
      font-size: clamp(1.5rem, 3vw, 1.8rem);     /* Tamanho responsivo */
      text-decoration: none;                     /* Sem sublinhado */
      box-shadow: 0 4px 20px rgba(37, 211, 102, 0.4); /* Sombra verde */
      transition: all 0.3s ease;                 /* Efeito suave */
      z-index: 999;                             /* Fica por cima de outros elementos */
    }

    /* Copyright no rodapé */
    .footer-bottom {
      border-top: 1px solid #333;               /* Linha separadora */
      padding-top: 2rem;                        /* Espaço em cima */
      text-align: center;                       /* Centralizado */
      color: #888;                              /* Cinza claro */
      font-size: clamp(0.8rem, 2vw, 0.9rem);    /* Tamanho responsivo */
      padding: 2rem 1rem 0;                     /* Espaçamento interno */
    }

    /* ===================================
       SEÇÃO 10: RESPONSIVIDADE (ADAPTAÇÃO PARA DIFERENTES TELAS)
       =================================== */
    
    /* Para tablets (telas médias) */
    @media (max-width: 1024px) {
      .main-container {
        padding: 0 1.5rem;  /* Menos espaçamento lateral */
      }

      .services-grid {
        grid-template-columns: repeat(auto-fit, minmax(min(100%, 320px), 1fr)); /* Colunas menores */
        gap: 1.5rem;        /* Menos espaço entre colunas */
      }

      .about-grid {
        gap: 3rem;          /* Menos espaço entre colunas */
      }
    }

    /* Para celulares (telas pequenas) */
    @media (max-width: 768px) {
      /* Mostra o botão do menu hamburger */
      .mobile-menu-toggle {
        display: block;
      }

      /* Esconde o menu normal e reconfigura para mobile */
      .nav-links {
        display: none;              /* Escondido por padrão */
        position: absolute;         /* Posição absoluta */
        top: 100%;                 /* Aparece abaixo da barra */
        left: 0;                   /* Alinhado à esquerda */
        right: 0;                  /* Alinhado à direita */
        background: #1A1A1A;        /* Fundo preto */
        flex-direction: column;     /* Itens em coluna */
        padding: 1rem;             /* Espaçamento interno */
        box-shadow: 0 4px 10px rgba(0,0,0,0.2); /* Sombra */
      }

      /* Mostra o menu quando tem a classe 'active' */
      .nav-links.active {
        display: flex;
      }

      /* Itens do menu ocupam largura total */
      .nav-links li {
        width: 100%;
      }

      /* Links do menu em formato de botão */
      .nav-links a {
        display: block;              /* Formato de bloco */
        padding: 0.75rem 1rem;       /* Espaçamento interno */
        border-bottom: 1px solid #333; /* Linha separadora */
      }

      /* Hero menor em celulares */
      .hero-section {
        padding: 5rem 0 4rem;  /* Menos espaçamento */
        min-height: 50vh;      /* Altura menor */
      }

      /* Serviços em coluna única */
      .services-grid {
        grid-template-columns: 1fr;  /* Uma coluna só */
        padding: 0;                  /* Remove espaçamento lateral */
      }

      /* Sobre em coluna única */
      .about-grid {
        grid-template-columns: 1fr;  /* Uma coluna só */
      }

      /* Rodapé reorganizado para mobile */
      .footer-content {
        grid-template-columns: 1fr;  /* Uma coluna só */
        text-align: center;          /* Centralizado */
        gap: 2rem;                   /* Espaço entre elementos */
      }

      /* Newsletter em coluna para mobile */
      .newsletter-form {
        flex-direction: column;      /* Campo e botão em coluna */
        margin: 0 auto;              /* Centralizado */
      }

      /* Campo e botão ocupam largura total */
      .newsletter-input,
      .newsletter-button {
        border-radius: 6px;          /* Cantos arredondados */
        width: 100%;                 /* Largura total */
      }

      /* Espaço entre campo e botão */
      .newsletter-button {
        margin-top: 0.5rem;
      }

      /* Centraliza Instagram e bandeira */
      .instagram-button,
      .footer-flag {
        margin: 0 auto;
      }
    }

    /* Para celulares muito pequenos */
    @media (max-width: 480px) {
      .main-container,
      .nav-content {
        padding: 0 1rem;  /* Menos espaçamento lateral */
      }

      .hero-section {
        padding: 4rem 0 3rem;  /* Ainda menos espaçamento */
      }

      .service-content {
        padding: 1.25rem;  /* Menos espaçamento interno nos cartões */
      }

      .about-content {
        padding: 0 0.5rem;  /* Menos espaçamento no texto sobre */
      }
    }

    /* Para telas muito grandes */
    @media (min-width: 1400px) {
      .hero-title {
        font-size: 4rem;  /* Título ainda maior */
      }

      .hero-subtitle {
        font-size: 1.5rem;  /* Subtítulo maior */
      }

      .services-grid {
        grid-template-columns: repeat(3, 1fr);  /* Sempre 3 colunas */
      }
    }

    /* ===================================
       SEÇÃO 11: ACESSIBILIDADE
       =================================== */
    
    /* Para pessoas que preferem menos animações */
    @media (prefers-reduced-motion: reduce) {
      * {
        animation: none !important;   /* Remove todas as animações */
        transition: none !important;  /* Remove todas as transições */
      }
    }

    /* Configuração para modo escuro (se o sistema estiver em modo escuro) */
    @media (prefers-color-scheme: dark) {
      .services-section,
      .about-section {
        background: #1A1A1A;  /* Fundo escuro */
        color: #E0E0E0;       /* Texto claro */
      }

      .service-card {
        background: #2A2A2A;  /* Cartões escuros */
        border-color: #333;   /* Bordas escuras */
      }

      .service-title,
      .section-title,
      .about-content h2 {
        color: #E0E0E0;  /* Títulos claros */
      }

      .service-description,
      .service-features li,
      .about-text,
      .section-subtitle {
        color: #B0B0B0;  /* Texto secundário claro */
      }
    }
  </style>

  <!-- ===================================
       PARTE 2: ESTRUTURA HTML (CONTEÚDO)
       =================================== -->

  <!-- Navegação do topo da página -->
  <nav class="top-nav">
    <div class="nav-content">
        <!-- Logo da empresa -->
        <div class="logo">
        <img src="/assets/images/logo.png" alt="Entre Casca">
        </div>
      <!-- Botão para abrir menu em celulares (☰ é o símbolo de 3 linhas) -->
      <button class="mobile-menu-toggle" onclick="toggleMenu()">☰</button>
      <!-- Lista de links do menu -->
      <ul class="nav-links" id="navLinks">
        <li><a href="#oficinas">Oficinas</a></li>
        <li><a href="#aulas">Aulas</a></li>
        <li><a href="#criacoes">Criações</a></li>
        <li><a href="#sobre">Sobre</a></li>
      </ul>
    </div>
  </nav>

  <!-- Seção principal da página (Hero) -->
  <section class="hero-section">
    <div class="main-container">
      <div class="hero-content">
        <!-- Título principal -->
        <h1 class="hero-title">Entre Casca</h1>
        <!-- Subtítulo explicativo -->
        <p class="hero-subtitle">
          Ateliê de marcenaria artesanal onde transformamos madeira em arte há mais de 10 anos
        </p>
      </div>
    </div>
  </section>

  <!-- Seção dos serviços oferecidos -->
  <section class="services-section" id="services">
    <div class="main-container">
      <!-- Cabeçalho da seção -->
      <div class="section-header">
        <h2 class="section-title">Nossos Serviços</h2>
        <p class="section-subtitle">
          Do aprendizado à criação, oferecemos experiências completas em marcenaria artesanal
        </p>
      </div>
      
      <!-- Grade com os 3 serviços -->
      <div class="services-grid">
        <!-- CARTÃO 1: Oficinas -->
        <div class="service-card">
          <!-- Imagem de fundo com etiqueta -->
          <div class="service-image" style="background-image: url('/assets/images/escrivaninha_pinceis.jpg')">
            <div class="service-overlay">Grupos pequenos</div>
          </div>
          <!-- Conteúdo do cartão -->
          <div class="service-content">
            <h3 class="service-title">Oficinas Práticas</h3>
            <p class="service-description">
              Oficinas intensivas para todos os níveis, onde você aprende fazendo. Técnicas tradicionais e modernas em um ambiente colaborativo.
            </p>
            <!-- Lista de benefícios -->
            <ul class="service-features">
              <li>Turmas de até 8 pessoas</li>
              <li>Ferramentas profissionais incluídas</li>
              <li>Projeto personalizado</li>
              <li>Certificado de participação</li>
            </ul>
            <!-- Link para mais informações -->
            <a href="#oficinas" class="service-link">Ver oficinas disponíveis</a>
          </div>
        </div>

        <!-- CARTÃO 2: Aulas -->
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

        <!-- CARTÃO 3: Criações -->
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

  <!-- Seção "Sobre nós" -->
  <section class="about-section" id="sobre">
    <div class="main-container">
      <div class="about-grid">
        <!-- Coluna com texto -->
        <div class="about-content">
          <h2>A paixão pela madeira nos move</h2>
          <p class="about-text">
            O Entre Casca nasceu da paixão pela madeira e pelo artesanato brasileiro. Há mais de uma década, criamos um espaço onde tradição e inovação se encontram.
          </p>
          <p class="about-text">
            Nosso ateliê é mais que um local de trabalho - é um ponto de encontro para artesãos, aprendizes e amantes da marcenaria que compartilham o amor pela transformação da madeira em arte.
          </p>
          <!-- Caixa de destaque com citação -->
          <div class="about-highlight">
            <p>"Cada peça de madeira tem sua própria personalidade. Nosso papel é revelá-la e dar-lhe nova vida através do artesanato."</p>
          </div>
        </div>
        <!-- Coluna com imagem -->
        <div class="about-image"></div>
      </div>
    </div>
  </section>

  <!-- Rodapé da página -->
  <footer class="footer-section">
    <div class="main-container">
      <div class="footer-content">
        <!-- Área do newsletter -->
        <div class="newsletter-content">
          <h3 class="newsletter-title">Fique conectado com o Entre Casca</h3>
          <p class="newsletter-description">
            Receba dicas de marcenaria, novidades sobre oficinas e histórias do nosso ateliê.
          </p>
          
          <!-- Formulário para inscrição no newsletter -->
          <form name="newsletter" method="POST" data-netlify="true" class="newsletter-form">
            <input type="email" 
                   name="email" 
                   placeholder="Seu email..." 
                   required
                   class="newsletter-input">
            <button type="submit" class="newsletter-button">
              Inscrever-se
            </button>
            <!-- Campo oculto necessário para o Netlify -->
            <input type="hidden" name="form-name" value="newsletter">
          </form>
        </div>

        <!-- Botão do Instagram -->
        <a href="https://instagram.com/entrecasca" class="instagram-button" target="_blank" aria-label="Instagram">
          📷
        </a>

        <!-- Bandeira (desenho em SVG) -->
        <div class="footer-flag">
          <!-- SVG é um formato de imagem vetorial criado com código -->
          <svg viewBox="0 0 400 280" xmlns="http://www.w3.org/2000/svg" style="width: 100%; height: 100%;">
            <!-- Retângulo de fundo rosa -->
            <rect width="400" height="280" fill="#E91E63"/>
            <!-- Losango branco -->
            <path d="M200,40 L360,140 L200,240 L40,140 Z" fill="#FFFFFF" stroke="#F0F0F0" stroke-width="3"/>
            <!-- Círculo verde -->
            <circle cx="200" cy="140" r="80" fill="#4CAF50" stroke="#388E3C" stroke-width="4"/>
            <!-- Detalhes decorativos -->
            <g stroke="#81C784" stroke-width="3" fill="none" opacity="0.9">
              <circle cx="200" cy="140" r="65" stroke-dasharray="12,6"/>
              <path d="M200,90 L200,190 M150,140 L250,140"/>
            </g>
          </svg>
        </div>
      </div>

      <!-- Linha de copyright -->
      <div class="footer-bottom">
        <p>&copy; 2024 Entre Casca. Todos os direitos reservados.</p>
      </div>
    </div>
  </footer>

  <!-- Botão flutuante do WhatsApp -->
  <a href="https://wa.me/5511999999999" class="whatsapp-float" target="_blank" aria-label="WhatsApp">
    💬
  </a>

  <!-- ===================================
       PARTE 3: JAVASCRIPT (INTERATIVIDADE)
       =================================== -->

  <script>
    /* 
      EXPLICAÇÃO DO JAVASCRIPT:
      Esta seção adiciona comportamentos interativos ao site.
      JavaScript é uma linguagem que roda no navegador e permite
      que elementos da página respondam a ações do usuário.
    */

    // FUNÇÃO 1: Abre e fecha o menu em celulares
    function toggleMenu() {
      // Encontra o elemento do menu pelo seu ID
      const navLinks = document.getElementById('navLinks');
      // Adiciona ou remove a classe 'active' (que mostra/esconde o menu)
      navLinks.classList.toggle('active');
    }

    // FUNÇÃO 2: Fecha o menu quando clica em um link (só em celulares)
    // Pega todos os links do menu
    document.querySelectorAll('.nav-links a').forEach(link => {
      // Para cada link, adiciona um "ouvinte" de evento de clique
      link.addEventListener('click', () => {
        // Quando clica no link, remove a classe 'active' (fecha o menu)
        document.getElementById('navLinks').classList.remove('active');
      });
    });

    // FUNÇÃO 3: Rolagem suave quando clica em links internos
    // Pega todos os links que começam com "#" (links internos da página)
    document.querySelectorAll('a[href^="#"]').forEach(anchor => {
      // Para cada link interno, adiciona um ouvinte de clique
      anchor.addEventListener('click', function (e) {
        // Previne o comportamento padrão (pular direto para a seção)
        e.preventDefault();
        // Encontra o elemento de destino usando o href do link
        const target = document.querySelector(this.getAttribute('href'));
        // Se o elemento existe, rola suavemente até ele
        if (target) {
          target.scrollIntoView({
            behavior: 'smooth',  // Rolagem suave
            block: 'start'       // Alinha no topo
          });
        }
      });
    });

    /* 
      RESUMO DAS FUNCIONALIDADES:
      1. Menu hamburger que abre/fecha em celulares
      2. Menu fecha automaticamente quando clica em um link
      3. Rolagem suave quando navega entre seções da página
      
      Estes scripts melhoram a experiência do usuário, tornando
      a navegação mais fluida e intuitiva.
    */
  </script>