---
layout: default
title: Inicio
nav_order: 1
permalink: /
---

<style>
  /* ==========================================
     RESET AGRESIVO PARA ELIMINAR MÁRGENES DEL TEMA
     ========================================== */
  .side-bar, .main-header, .site-header, .site-footer { display: none !important; }
  
  .main, .main-content, .main-content-wrap { 
    margin: 0 !important; 
    padding: 0 !important; 
    max-width: 100% !important; 
    width: 100% !important;
    background-color: #0d1117 !important; 
  }
  
  .main-content {
    color: #c9d1d9 !important; 
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif !important;
  }
  
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
     NAVBAR SUPERIOR (MÍNIMO E ICONOGRÁFICO)
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
  
  .ln-nav-links { 
    display: flex !important; 
    gap: 1.6rem !important; 
    margin: 0 !important; 
    padding: 0 !important; 
    align-items: center;
  }
  .ln-nav-links a { 
    color: var(--text-muted) !important; 
    text-decoration: none !important; 
    font-weight: 500; 
    font-size: 0.95rem; 
    transition: color 0.2s ease; 
  }
  .ln-nav-links a:hover { color: var(--text-main) !important; }
  
  .nav-divider {
    color: var(--border-color);
    font-size: 0.9rem;
    user-select: none;
    margin: 0 0.2rem;
  }

  /* Estilos para íconos del nav con colores de marca en hover */
  .nav-icon {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    color: var(--text-muted) !important;
    transition: color 0.2s ease, transform 0.2s ease;
  }
  .nav-icon svg { width: 18px; height: 18px; }
  .nav-icon:hover { transform: scale(1.1); }
  .nav-linkedin:hover { color: #0077b5 !important; }
  .nav-upwork:hover { color: #14a800 !important; }
  .nav-workana:hover { color: #00bcd4 !important; }

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
    color: var(--text-main) !important;
    line-height: 1.15;
    margin: 0 0 1rem 0 !important;
    letter-spacing: -1px;
  }
  .ln-hero h2 {
    font-size: 1.8rem;
    font-weight: 600;
    color: #58a6ff !important;
    margin: 0 0 1.5rem 0 !important;
  }
  .ln-hero p {
    font-size: 1.15rem;
    line-height: 1.6;
    color: var(--text-muted);
    max-width: 750px;
    margin: 0 0 2.5rem 0 !important;
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

  /* ==========================================
     BLOQUE 2: GRID DE SERVICIOS
     ========================================== */
  .services-section {
    padding: 6rem 10%;
    background-color: var(--bg-secondary);
    border-bottom: 1px solid var(--border-color);
  }
  .section-title {
    font-size: 2rem;
    font-weight: 700;
    color: var(--text-main) !important;
    margin-bottom: 0.5rem !important;
  }
  .section-subtitle {
    font-size: 1rem;
    color: var(--text-muted);
    margin-bottom: 3.5rem !important;
  }
  .services-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 2rem;
  }
  .service-card {
    background-color: var(--bg-primary);
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 2.5rem 2rem;
    transition: border-color 0.3s ease, transform 0.3s ease;
  }
  .service-card:hover {
    border-color: #444c56;
    transform: translateY(-4px);
  }
  .service-icon {
    font-size: 2rem;
    margin-bottom: 1.2rem;
    display: inline-block;
  }
  .service-card h3 {
    font-size: 1.35rem;
    font-weight: 600;
    color: var(--text-main) !important;
    margin: 0 0 0.8rem 0 !important;
  }
  .service-card p {
    font-size: 0.95rem;
    line-height: 1.6;
    color: var(--text-muted);
    margin: 0 !important;
  }

  /* ==========================================
     BLOQUE 3: BANNER DE IMPACTO / CASO DE ÉXITO
     ========================================== */
  .impact-section {
    padding: 6rem 10%;
    background-color: var(--bg-primary);
    border-bottom: 1px solid var(--border-color);
    display: flex;
    align-items: center;
    gap: 4rem;
    flex-wrap: wrap;
  }
  .impact-metric {
    flex: 1;
    min-width: 280px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background: radial-gradient(circle at center, rgba(31, 111, 235, 0.1) 0%, transparent 70%);
    border: 1px solid rgba(56, 139, 253, 0.2);
    border-radius: 12px;
    padding: 3.5rem 2rem;
    text-align: center;
    box-shadow: 0 8px 24px rgba(0, 0, 0, 0.2);
  }
  .impact-number {
    font-size: 4.5rem;
    font-weight: 800;
    color: #58a6ff;
    line-height: 1;
    margin-bottom: 0.5rem;
    letter-spacing: -1px;
  }
  .impact-label {
    font-size: 0.9rem;
    font-weight: 700;
    color: var(--text-main);
    text-transform: uppercase;
    letter-spacing: 2px;
  }
  .impact-content {
    flex: 2;
    min-width: 320px;
  }
  .impact-badge {
    background-color: rgba(56, 139, 253, 0.15);
    color: #58a6ff;
    padding: 0.3rem 0.8rem;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 600;
    margin-bottom: 1.2rem;
    display: inline-block;
    border: 1px solid rgba(56, 139, 253, 0.2);
  }
  .impact-content h2 {
    font-size: 2.2rem;
    font-weight: 700;
    color: var(--text-main) !important;
    margin: 0 0 1.2rem 0 !important;
    line-height: 1.2;
  }
  .impact-content p {
    font-size: 1.05rem;
    line-height: 1.6;
    color: var(--text-muted);
    margin-bottom: 1.8rem !important;
  }

  /* ==========================================
     BLOQUE 4: ECOSISTEMA TECNOLÓGICO (TECH STACK)
     ========================================== */
  .tech-section {
    padding: 6rem 10%;
    background-color: var(--bg-secondary);
    border-bottom: 1px solid var(--border-color);
  }
  .tech-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 1.5rem;
    margin-top: 3rem;
  }
  .tech-category {
    background-color: var(--bg-primary);
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 1.8rem;
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }
  .tech-category h3 {
    font-size: 1.1rem;
    font-weight: 600;
    color: #58a6ff !important;
    margin: 0 !important;
    padding-bottom: 0.6rem;
    border-bottom: 1px solid var(--border-color);
  }
  .tech-badges-container {
    display: flex;
    flex-wrap: wrap;
    gap: 0.6rem;
  }
  .tech-badges-container img {
    height: 28px;
    border-radius: 4px;
  }

  /* ==========================================
     BLOQUE 5: FILOSOFÍA DE TRABAJO
     ========================================== */
  .about-section {
    padding: 6rem 10%;
    background-color: var(--bg-primary);
    border-bottom: 1px solid var(--border-color);
  }
  .about-container {
    display: flex;
    align-items: center;
    gap: 4rem;
    flex-wrap: wrap;
  }
  .about-content {
    flex: 1.2;
    min-width: 320px;
  }
  .about-card {
    flex: 0.8;
    min-width: 280px;
    background-color: var(--bg-secondary);
    border: 1px solid var(--border-color);
    border-radius: 8px;
    padding: 2.5rem;
    box-shadow: 0 4px 20px rgba(0,0,0,0.15);
  }
  .about-card h4 {
    color: #d2a8ff !important;
    margin: 0 0 1.2rem 0 !important;
    font-size: 1.1rem;
    text-transform: uppercase;
    letter-spacing: 1px;
    font-weight: 700;
  }
  .about-features {
    display: flex;
    flex-direction: column;
    gap: 1.2rem;
  }
  .about-item {
    font-size: 0.95rem;
    line-height: 1.5;
    color: var(--text-muted);
  }
  .about-item strong {
    color: var(--text-main);
    display: block;
    font-size: 1rem;
    margin-bottom: 0.2rem;
  }

  /* ==========================================
     BLOQUE 6: GRID DE CONTACTO ICONOGRÁFICO PREMIUM
     ========================================== */
  .contact-section {
    padding: 6rem 10%;
    background-color: var(--bg-secondary);
    text-align: center;
  }
  .contact-icons-grid {
    display: flex;
    justify-content: center;
    gap: 1.8rem;
    flex-wrap: wrap;
    margin-top: 3.5rem;
  }
  .contact-icon-card {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 65px;
    height: 65px;
    border-radius: 10px;
    border: 1px solid var(--border-color);
    background-color: var(--bg-primary);
    color: var(--text-muted) !important;
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
  }
  .contact-icon-card svg {
    width: 26px;
    height: 26px;
  }
  .contact-icon-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 24px rgba(0,0,0,0.3);
  }
  
  /* Colores dinámicos específicos para cada red en hover */
  .card-email:hover { border-color: #ea4335; color: #ea4335 !important; }
  .card-linkedin:hover { border-color: #0077b5; color: #0077b5 !important; }
  .card-upwork:hover { border-color: #14a800; color: #14a800 !important; }
  .card-workana:hover { border-color: #00bcd4; color: #00bcd4 !important; }
  .card-github:hover { border-color: #8957e5; color: #8957e5 !important; }
</style>

<!-- Barra de Navegación Premium -->
<nav class="ln-navbar">
  <a href="/" class="ln-brand">alejandro<span>bepmale</span></a>
  <div class="ln-nav-links">
    <a href="/">Inicio</a>
    <a href="/infraestructura">Infraestructura</a>
    <a href="/ciberseguridad">Ciberseguridad</a>
    <a href="#contacto">Contacto</a>
    <span class="nav-divider">|</span>
    <!-- LinkedIn -->
    <a href="https://www.linkedin.com/in/alejandrobepmale" target="_blank" class="nav-icon nav-linkedin" title="LinkedIn">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
    </a>
    <!-- Upwork -->
    <a href="https://www.upwork.com" target="_blank" class="nav-icon nav-upwork" title="Upwork">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.35 5.63c-2.31 0-4.14 1.56-4.82 3.82l-.17.62-.57-2.38C11.12 4.96 8.79 3 6.14 3 2.75 3 0 5.75 0 9.14v5.73h2.72V9.14c0-1.88 1.53-3.42 3.42-3.42 1.67 0 3.09 1.2 3.38 2.84l.91 3.81H7.71v2.72h5.44l.21.87c.59 2.46 2.5 3.99 5.01 3.99 3.47 0 6.29-2.82 6.29-6.29 0-3.47-2.82-6.29-6.29-6.29zm1 9.87c-1.39 0-2.38-.81-2.73-2.12l-.31-1.26c.55-1.48 1.68-2.45 3.04-2.45 1.97 0 3.57 1.6 3.57 3.57 0 1.97-1.6 3.57-3.57 3.57z"/></svg>
    </a>
    <!-- Workana -->
    <a href="https://www.workana.com" target="_blank" class="nav-icon nav-workana" title="Workana">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1.12 14.28L8.12 9.44h1.9l1.43 4.5 1.41-4.5h1.9l-2.76 6.84h-1.12z"/></svg>
    </a>
  </div>
</nav>

<!-- Bloque 1: Hero Section -->
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

<!-- Bloque 2: Grid de Servicios -->
<section id="servicios" class="services-section">
  <h2 class="section-title">Servicios de Consultoría Especializada</h2>
  <p class="section-subtitle">Soluciones diseñadas para optimizar operaciones, mitigar riesgos y asegurar la escalabilidad tecnológica.</p>
  
  <div class="services-grid">
    <div class="service-card">
      <span class="service-icon">🤖</span>
      <h3>Automatización de Procesos</h3>
      <p>Construcción de ecosistemas altamente eficientes mediante la integración de APIs con Make.com y el despliegue de pasarelas de comunicación automatizada utilizando WAHA para optimizar flujos críticos de negocio.</p>
    </div>
    
    <div class="service-card">
      <span class="service-icon">🏗️</span>
      <h3>Gestión de Infraestructura</h3>
      <p>Despliegue, migración y mantenimiento de arquitecturas virtuales sobre VMware ESXi, entornos corporativos complejos basados en Citrix LTSR y configuraciones avanzadas en servidores de producción Linux/Ubuntu.</p>
    </div>
    
    <div class="service-card">
      <span class="service-icon">🛡️</span>
      <h3>Monitoreo y Continuidad operativa</h3>
      <p>Implementación desde cero de servidores de monitoreo (Zabbix) para visibilidad total de red. Diseño de políticas robustas de respaldo de bases de datos para garantizar la integridad ante contingencias críticas.</p>
    </div>
  </div>
</section>

<!-- Bloque 3: Banner de Impacto / Caso de Éxito -->
<section class="impact-section">
  <div class="impact-metric">
    <span class="impact-number">+30 TB</span>
    <span class="impact-label">Datos Migrados</span>
  </div>
  <div class="impact-content">
    <span class="impact-badge">Caso de Éxito: Infraestructura Resiliente</span>
    <h2>Migración crítica de datos masivos sobre hardware degradado</h2>
    <p>Diseño e implementación de un motor de automatización bajo demanda mediante scripts avanzados para la sincronización de grandes volúmenes de información corporativa. Ante la inestabilidad de la red y fallas de hardware físico de dispositivos de almacenamiento tradicionales, se estructuró una solución de bajo nivel con tolerancia a fallas capaz de gestionar reintentos automáticos, mitigar el estrés de lectura/escritura y garantizar la integridad total de la data sin interrupciones operativas.</p>
    <a href="/infraestructura" class="btn-ln btn-outline">Ver Detalles Técnicos</a>
  </div>
</section>

<!-- Bloque 4: Ecosistema Tecnológico (Tech Stack) -->
<section id="tecnologias" class="tech-section">
  <h2 class="section-title">Ecosistema Tecnológico</h2>
  <p class="section-subtitle">Herramientas y tecnologías integradas para el diseño de soluciones robustas y seguras.</p>
  
  <div class="tech-grid">
    <div class="tech-category">
      <h3>Infraestructura & Cloud</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/VMware_ESXi-6151B1?style=flat-square&logo=vmware&logoColor=white" alt="VMware">
        <img src="https://img.shields.io/badge/Citrix_LTSR-00A4E4?style=flat-square&logo=citrix&logoColor=white" alt="Citrix">
        <img src="https://img.shields.io/badge/cPanel_/_WHM-FF6C2C?style=flat-square&logo=cpanel&logoColor=white" alt="cPanel">
        <img src="https://img.shields.io/badge/Ubuntu_Server-E95420?style=flat-square&logo=ubuntu&logoColor=white" alt="Ubuntu">
        <img src="https://img.shields.io/badge/Windows_Server-0078D6?style=flat-square&logo=windows&logoColor=white" alt="Windows Server">
      </div>
    </div>

    <div class="tech-category">
      <h3>Automatización</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
        <img src="https://img.shields.io/badge/Make.com-010101?style=flat-square&logo=make&logoColor=white" alt="Make.com">
        <img src="https://img.shields.io/badge/WAHA_API-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="WAHA">
      </div>
    </div>

    <div class="tech-category">
      <h3>Scripting & Desarrollo</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white" alt="PowerShell">
        <img src="https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white" alt="Bash">
        <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python">
        <img src="https://img.shields.io/badge/SQL_Server-CC2927?style=flat-square&logo=microsoft-sql-server&logoColor=white" alt="SQL Server">
        <img src="https://img.shields.io/badge/Flutter_/_Dart-02569B?style=flat-square&logo=flutter&logoColor=white" alt="Flutter">
      </div>
    </div>

    <div class="tech-category">
      <h3>Monitoreo & Seguridad</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/Zabbix-CC292F?style=flat-square&logo=zabbix&logoColor=white" alt="Zabbix">
        <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=flat-square&logo=kali-linux&logoColor=white" alt="Kali Linux">
        <img src="https://img.shields.io/badge/Shodan-212121?style=flat-square&logo=shodan&logoColor=white" alt="Shodan">
      </div>
    </div>
  </div>
</section>

<!-- Bloque 5: Filosofía de Trabajo / Tu Aliado Digital -->
<section class="about-section">
  <div class="about-container">
    <div class="about-content">
      <h2 class="section-title">De Humano a Humano: Tu Aliado Digital</h2>
      <p class="section-subtitle" style="margin-bottom: 1.5rem !important;">Por qué trabajar con un consultor dedicado marca la diferencia.</p>
      <p>Detrás de cada gran infraestructura o automatización exitosa hay decisiones estratégicas que no se resuelven con un sistema automatizado de tickets cerrados al azar. A través de <strong>Insertbog</strong>, opero bajo una estructura de asociación directa, convirtiéndome en un verdadero aliado tecnológico para tu negocio.</p>
      <p>Mi objetivo no es venderte horas de soporte reactivo, sino diseñar e integrar ecosistemas robustos de alto valor que prevengan las caídas de servicio, agilicen tus flujos operativos diarios y protejan tus activos digitales de extremo a extremo.</p>
    </div>
    <div class="about-card">
      <h4>El Enfoque de Trabajo</h4>
      <div class="about-features">
        <div class="about-item">
          <strong>Asociación Directa</strong>
          Sin intermediarios corporativos ni burocracia comercial. Comunicación técnica fluida de un profesional a otro.
        </div>
        <div class="about-item">
          <strong>Soluciones de Alto Valor</strong>
          Foco absoluto en la estabilidad del entorno, la seguridad de la red y la automatización inteligente de procesos.
        </div>
        <div class="about-item">
          <strong>Criterio de Continuidad</strong>
          Sistemas preparados para contingencias reales, respaldos consistentes y monitoreo proactivo constante.
        </div>
      </div>
    </div>
  </div>
</section>

<!-- Bloque 6: Sección de Contacto Iconográfica Premium -->
<section id="contacto" class="contact-section">
  <h2 class="section-title">¿Hablamos de tu próximo proyecto?</h2>
  <p class="section-subtitle">Ya sea para integraciones complejas, auditorías de seguridad o estabilidad de infraestructura, conéctame por cualquiera de mis canales oficiales.</p>
  
  <div class="contact-icons-grid">
    <!-- Email -->
    <a href="mailto:contacto@alejandrobepmale.com" class="contact-icon-card card-email" title="Enviar un Correo Electrónico">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
    </a>
    <!-- LinkedIn -->
    <a href="https://www.linkedin.com/in/alejandrobepmale" target="_blank" class="contact-icon-card card-linkedin" title="Ver Perfil de LinkedIn">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
    </a>
    <!-- Upwork -->
    <a href="https://www.upwork.com" target="_blank" class="contact-icon-card card-upwork" title="Ver Perfil de Upwork">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M17.35 5.63c-2.31 0-4.14 1.56-4.82 3.82l-.17.62-.57-2.38C11.12 4.96 8.79 3 6.14 3 2.75 3 0 5.75 0 9.14v5.73h2.72V9.14c0-1.88 1.53-3.42 3.42-3.42 1.67 0 3.09 1.2 3.38 2.84l.91 3.81H7.71v2.72h5.44l.21.87c.59 2.46 2.5 3.99 5.01 3.99 3.47 0 6.29-2.82 6.29-6.29 0-3.47-2.82-6.29-6.29-6.29zm1 9.87c-1.39 0-2.38-.81-2.73-2.12l-.31-1.26c.55-1.48 1.68-2.45 3.04-2.45 1.97 0 3.57 1.6 3.57 3.57 0 1.97-1.6 3.57-3.57 3.57z"/></svg>
    </a>
    <!-- Workana -->
    <a href="https://www.workana.com" target="_blank" class="contact-icon-card card-workana" title="Ver Perfil de Workana">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1.12 14.28L8.12 9.44h1.9l1.43 4.5 1.41-4.5h1.9l-2.76 6.84h-1.12z"/></svg>
    </a>
    <!-- GitHub -->
    <a href="https://github.com/alejandrobepmale" target="_blank" class="contact-icon-card card-github" title="Ver Repositorios en GitHub">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
    </a>
  </div>
</section>
