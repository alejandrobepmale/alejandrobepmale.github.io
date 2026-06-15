---
layout: default
title: Inicio
nav_order: 1
permalink: /
---

<style>
  /* Ocultamos el sidebar única y exclusivamente en la Landing Page */
  .side-bar { display: none !important; }
  @media (min-width: 64rem) {
    .main { margin-left: 0 !important; max-width: 100% !important; }
  }
</style>

{% include navbar.html %}

<!-- Bloque 1: Hero Section -->
<header class="ln-hero">
  <span class="ln-hero-tag">Consultoría TI & Seguridad de Extremo a Extremo</span>
  <h1>Tu aliado digital en infraestructura y ciberseguridad</h1>
  <h2>Soluciones robustas para la continuidad de tu negocio</h2>
  <p>Diseño e implemento ecosistemas estables conectando el desarrollo de software con arquitecturas cloud, virtualización avanzada y flujos operativos blindados. Menos fricción, máxima postura de seguridad.</p>
  
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
    <!-- 1. Infraestructura -->
    <div class="service-card">
      <span class="service-icon">🏗️</span>
      <h3>Gestión de Infraestructura</h3>
      <p>Despliegue, migración y mantenimiento de arquitecturas virtuales sobre VMware ESXi, entornos corporativos complejos basados en Citrix LTSR y configuraciones avanzadas en servidores de producción Linux/Ubuntu.</p>
    </div>

    <!-- 2. Ciberseguridad -->
    <div class="service-card">
      <span class="service-icon">🛡️</span>
      <h3>Ciberseguridad y Monitoreo</h3>
      <p>Análisis práctico de vulnerabilidades, modelado de amenazas y despliegue desde cero de servidores de monitoreo (Zabbix) para lograr visibilidad completa de la red y prevenir contingencias críticas de conectividad.</p>
    </div>
    
    <!-- 3. Automatización -->
    <div class="service-card">
      <span class="service-icon">🤖</span>
      <h3>Automatización de Procesos</h3>
      <p>Construcción de ecosistemas altamente eficientes mediante la integración de APIs con Make.com y el despliegue de pasarelas de comunicación automatizada utilizando WAHA para optimizar flujos críticos de negocio.</p>
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

<!-- Bloque 4: Ecosistema Tecnológico -->
<section id="tecnologias" class="tech-section">
  <h2 class="section-title">Ecosistema Tecnológico</h2>
  <p class="section-subtitle">Herramientas y tecnologías integradas para el diseño de soluciones robustas y seguras.</p>
  
  <div class="tech-grid">
    <!-- 1. Infraestructura -->
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

    <!-- 2. Ciberseguridad -->
    <div class="tech-category">
      <h3>Monitoreo & Seguridad</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/Zabbix-CC292F?style=flat-square&logo=zabbix&logoColor=white" alt="Zabbix">
        <img src="https://img.shields.io/badge/Kali_Linux-557C94?style=flat-square&logo=kali-linux&logoColor=white" alt="Kali Linux">
        <img src="https://img.shields.io/badge/Shodan-212121?style=flat-square&logo=shodan&logoColor=white" alt="Shodan">
      </div>
    </div>

    <!-- 3. Automatización -->
    <div class="tech-category">
      <h3>Automatización</h3>
      <div class="tech-badges-container">
        <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white" alt="Docker">
        <img src="https://img.shields.io/badge/Make.com-010101?style=flat-square&logo=make&logoColor=white" alt="Make.com">
        <img src="https://img.shields.io/badge/WAHA_API-25D366?style=flat-square&logo=whatsapp&logoColor=white" alt="WAHA">
      </div>
    </div>

    <!-- 4. Scripting & Desarrollo -->
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
  </div>
</section>

<!-- Bloque 5: Filosofía de Trabajo / Tu Aliado Digital -->
<section class="about-section">
  <div class="about-container">
    <div class="about-content">
      <h2 class="section-title">De Humano a Humano: Tu Aliado Digital</h2>
      <p class="section-subtitle" style="margin-bottom: 1.5rem !important;">Por qué trabajar con un consultor dedicado marca la diferencia.</p>
      <p>Detrás de cada gran infraestructura o entorno auditado exitosamente hay decisiones estratégicas que no se resuelven con un sistema automatizado de tickets cerrados al azar. A través de <strong>Insertbog</strong>, opero bajo una estructura de asociación directa, convirtiéndome en un verdadero aliado tecnológico para tu negocio.</p>
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

<!-- Bloque 6: Sección de Contacto Sólida -->
<section id="contacto" class="contact-section">
  <h2 class="section-title">¿Hablamos de tu próximo proyecto?</h2>
  <p class="section-subtitle">Ya sea para estabilidad de infraestructura, auditorías de seguridad o integraciones complejas, conéctame por cualquiera de mis canales oficiales.</p>
  
  <div class="contact-social-row">
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
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 0C5.373 0 0 5.373 0 12s5.373 12 12 12 12-5.373 12-12S18.627 0 12 0zm-1.071 15.6H8.25l-2.073-6h1.76l1.247 4.14 1.207-4.14h1.74l-2.002 6z"/></svg>
    </a>
    
    <!-- GitHub -->
    <a href="https://github.com/alejandrobepmale" target="_blank" class="contact-icon-card card-github" title="Ver Repositorios en GitHub">
      <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 .297c-6.63 0-12 5.373-12 12 0 5.303 3.438 9.8 8.205 11.385.6.113.82-.258.82-.577 0-.285-.01-1.04-.015-2.04-3.338.724-4.042-1.61-4.042-1.61C4.422 18.07 3.633 17.7 3.633 17.7c-1.087-.744.084-.729.084-.729 1.205.084 1.838 1.236 1.838 1.236 1.07 1.835 2.809 1.305 3.495.998.108-.776.417-1.305.76-1.605-2.665-.3-5.466-1.332-5.466-5.93 0-1.31.465-2.38 1.235-3.22-.135-.303-.54-1.523.105-3.176 0 0 1.005-.322 3.3 1.23.96-.267 1.98-.399 3-.405 1.02.006 2.04.138 3 .405 2.28-1.552 3.285-1.23 3.285-1.23.645 1.653.24 2.873.12 3.176.765.84 1.23 1.91 1.23 3.22 0 4.61-2.805 5.625-5.475 5.92.42.36.81 1.096.81 2.22 0 1.606-.015 2.896-.015 3.286 0 .315.21.69.825.57C20.565 22.092 24 17.592 24 12.297c0-6.627-5.373-12-12-12"/></svg>
    </a>
  </div>

  <div class="contact-email-row">
    <a href="mailto:contacto@alejandrobepmale.com" class="contact-btn-email" title="Enviar un Correo Electrónico">
      <svg viewBox="0 0 24 24" fill="currentColor" style="width: 20px; height: 20px; margin-right: 10px;"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
      contacto@alejandrobepmale.com
    </a>
  </div>
</section>
