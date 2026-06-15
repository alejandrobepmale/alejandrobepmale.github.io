---
layout: default
title: Inicio
nav_order: 1
permalink: /
---

<style>
  /* ==========================================
     RESET & DISEÑO GLOBAL DE LA LANDING
     ========================================== */
  .side-bar, .main-header, .site-header, .site-footer { display: none !important; }
  .main { margin-left: 0 !important; max-width: 100% !important; padding: 0 !important; background-color: #0d1117 !important; color: #c9d1d9 !important; font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif; }
  
  /* Variables de Color para fácil edición */
  :root {
    --bg-primary: #0d1117;
    --bg-secondary: #161b22;
    --accent-purple: #8957e5;
    --accent-blue: #1f6feb;
    --accent-green: #238636;
    --text-main: #f0f6fc;
    --text-muted: #8b949e;
    --border-color: #30363d;
  }

  /* ==========================================
     NAVBAR SUPERIOR
     ========================================== */
  .ln-navbar {
    background-color: rgba(22, 27, 34, 0.95);
    backdrop-filter: blur(10px);
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.2rem 10%;
    position: sticky;
    top: 0;
    z-index: 1000;
    border-bottom: 1px solid var(--border-color);
  }
  .ln-brand {
    color: var(--text-main) !important;
    font-weight: 700;
    font-size: 1.4rem;
    text-decoration: none;
    letter-spacing: -0.5px;
  }
  .ln-brand span { color: var(--accent-purple); }
  .ln-nav-links { display: flex; gap: 2.5rem; list-style: none; margin: 0; padding: 0; }
  .ln-nav-links a { color: var(--text-muted) !important; text-decoration: none; font-weight: 500; font-size: 0.95rem; transition: color 0.2s ease; }
  .ln-nav-links a:hover { color: var(--text-main) !important; }

  /* ==========================================
     HERO SECTION
     ========================================== */
  .ln-hero {
    padding: 7rem 10% 6rem 10%;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: center;
    background: radial-gradient(circle at 90% 10%, rgba(137, 87, 229, 0.08) 0%, transparent 40%),
                radial-gradient(circle at 10% 90%, rgba(31, 111, 235, 0.05) 0%, transparent 50%);
    border-bottom: 1px solid var(--border-color);
  }
  .ln-hero-tag {
    background-color: rgba(137, 87, 229, 0.15);
    color: #d2a8ff;
    padding: 0.4rem 1rem;
    border-radius: 20px;
    font-size: 0.85rem;
    font-weight: 600;
    margin-bottom: 1.5rem;
    border: 1px solid rgba(137, 87, 229, 0.3);
  }
  .ln-hero h1 {
    font-size: 3.2rem;
    font-weight: 800;
    color: var(--text-main);
    line-height: 1.15;
    margin: 0 0 1rem 0;
    letter-spacing: -1px;
  }
  .ln-hero h2 {
    font-size: 1.8rem;
    font-weight: 600;
    color: #58a6ff;
    margin: 0 0 1.5rem 0;
  }
  .ln-hero p {
    font-size: 1.15rem;
    line-height: 1.6;
    color: var(--text-muted);
    max-width: 750px;
    margin: 0 0 2.5rem 0;
  }
  .ln-hero-buttons { display: flex; gap: 1rem; flex-wrap: wrap; }
  .btn-ln {
    padding: 0.8rem 1.8rem;
    border-radius: 6px;
    font-weight: 600;
    font-size: 0.95rem;
    text-decoration: none;
    transition: transform 0.2s ease, filter 0.2s ease;
  }
  .btn-ln:hover { transform: translateY(-2px); filter: brightness(1.1); }
  .btn-purple { background-color: var(--accent-purple); color: #fff !important; }
  .btn-outline { border: 1px solid var(--border-color); color: var(--text-main) !important; background-color: transparent; }
</style>

<nav class="ln-navbar">
  <a href="/" class="ln-brand">alejandro<span>bepmale</span></a>
  <ul class="ln-nav-links">
    <li><a href="/">Inicio</a></li>
    <li><a href="/infraestructura">Infraestructura</a></li>
    <li><a href="/ciberseguridad">Ciberseguridad</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
</nav>

<header class="ln-hero">
  <span class="ln-hero-tag">Consultoría TI & Integración Eficiente</span>
  <h1>Tu aliado digital en infraestructura y automatización</h1>
  <h2>Soluciones robustas para la continuidad de tu negocio</h2>
  <p>Diseño e implemento ecosistemas estables conectando el desarrollo de software con arquitecturas cloud, virtualización avanzada y flujos de automatización inteligentes. Menos fricción operativa, máxima seguridad.</p>
  
  <div class="ln-hero-buttons">
    <a href="#servicios" class="btn-ln btn-purple">Explorar Servicios</a>
    <a href="#contacto" class="btn-ln btn-outline">Hablemos Directo</a>
  </div>
</header>
