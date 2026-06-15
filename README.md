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
  
  .ln-nav-links { 
    display: flex !important; 
    gap: 2.5rem !important; 
    list-style: none !important; 
    list-style-type: none !important;
    margin: 0 !important; 
    padding: 0 !important; 
  }
  .ln-nav-links li {
    list-style: none !important;
    list-style-type: none !important;
    margin: 0 !important;
    padding: 0 !important;
  }
  .ln-nav-links a { 
    color: var(--text-muted) !important; 
    text-decoration: none !important; 
    font-weight: 500; 
    font-size: 0.95rem; 
    transition: color 0.2s ease; 
  }
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
</style>

<!-- Barra de Navegación Premium -->
<nav class="ln-navbar">
  <a href="/" class="ln-brand">alejandro<span>bepmale</span></a>
  <ul class="ln-nav-links">
    <li><a href="/">Inicio</a></li>
    <li><a href="/infraestructura">Infraestructura</a></li>
    <li><a href="/ciberseguridad">Ciberseguridad</a></li>
    <li><a href="#contacto">Contacto</a></li>
  </ul>
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
    <!-- Categoría 1 -->
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

    <!-- Categoría 2 -->
    <div class="tech-category">
      <h3>Automatización</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
        <img src="https://img.shields.io/badge/Make.com-010101?style=flat-square&logo=make&logoColor=white" alt="Make.com">
        <img src="https://img.shields.io/badge/WAHA_API-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="WAHA">
      </div>
    </div>

    <!-- Categoría 3 -->
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

    <!-- Categoría 4 -->
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
