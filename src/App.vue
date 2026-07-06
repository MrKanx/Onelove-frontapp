<script setup lang="ts">
// Cellular Center - Awwwards Style Landing Page
</script>

<template>
  <div class="smooth-scroll-wrapper">
    <!-- HERO SECTION -->
    <section class="hero">
      <div class="hero-bg" style="background-image: url('/images/tech_hero_bg.png');"></div>
      <div class="hero-overlay"></div>
      
      <nav class="nav">
        <div class="logo">CELLULAR CENTER</div>
        <a href="#contacto" class="btn-contact">Hablemos</a>
      </nav>

      <div class="hero-content">
        <div class="reveal-text">
          <h1 class="display-title">TU NUEVO <br/> IPHONE</h1>
        </div>
        <p class="hero-subtitle">iPhones seminuevos y servicio técnico especializado <br/> para mantenerte conectado.</p>
      </div>

      <div class="scroll-indicator">
        <div class="mouse"></div>
        <span>Descubre</span>
      </div>
    </section>

    <!-- MARQUEE -->
    <div class="marquee-container">
      <div class="marquee">
        <span>INNOVACIÓN CONSTANTE &mdash; TECNOLOGÍA DE PUNTA &mdash; IPHONES SEMINUEVOS &mdash; SERVICIO TÉCNICO &mdash; </span>
        <span>INNOVACIÓN CONSTANTE &mdash; TECNOLOGÍA DE PUNTA &mdash; IPHONES SEMINUEVOS &mdash; SERVICIO TÉCNICO &mdash; </span>
      </div>
    </div>

    <!-- PORTFOLIO / GALLERY -->
    <section class="gallery">
      <div class="gallery-header">
        <h2 class="section-title">NUESTRO <br/> CATÁLOGO</h2>
        <p class="section-desc">Desde iPhones garantizados hasta reparaciones expertas. En Cellular Center respiramos tecnología y calidad.</p>
      </div>

      <div class="gallery-grid">
        <div class="gallery-item large">
          <div class="image-wrapper">
            <img src="/images/premium_iphones.png" alt="iPhones Seminuevos" />
            <div class="item-overlay">
              <h3>iPhones</h3>
              <p>Calidad garantizada</p>
            </div>
          </div>
        </div>
        <div class="gallery-item">
          <div class="image-wrapper">
            <img src="/images/tech_repair.png" alt="Servicio Técnico" />
            <div class="item-overlay">
              <h3>Servicio Técnico</h3>
              <p>Rápido y Seguro</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- FOOTER / LEGAL INFO -->
    <footer id="contacto" class="legal-footer">
      <div class="footer-grid">
        <!-- Branding / Contact -->
        <div class="footer-col brand-col">
          <h2 class="footer-logo">CELLULAR CENTER.</h2>
          <p class="contact-email"><a href="mailto:h.ushu@hotmail.com">h.ushu@hotmail.com</a></p>
          <div class="phones">
            <a href="tel:0997197439">0997197439</a>
          </div>
          <p class="copyright">&copy; 2026 ORTEGA AVILES HENRY GIOVANNI. All rights reserved.</p>
        </div>

        <!-- Verification Data -->
        <div class="footer-col legal-data">
          <h4>Información Comercial y Tributaria</h4>
          <div class="data-grid">
            <div class="data-item">
              <span class="label">Razón Social / Propietario</span>
              <span class="value">ORTEGA AVILES HENRY GIOVANNI</span>
            </div>
            <div class="data-item">
              <span class="label">RUC</span>
              <span class="value">0917909616001</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Actividades</span>
              <span class="value">Venta al por mayor de teléfonos y equipos de comunicación, y servicios de reparación y mantenimiento de sistemas informáticos.</span>
            </div>
            <div class="data-item">
              <span class="label">Estado / Régimen</span>
              <span class="value">Activo / Régimen General</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Fechas SRI</span>
              <span class="value">Registro: 24/04/2007 | Última Actualización: 22/08/2024</span>
            </div>
            <div class="data-item span-2">
              <span class="label">Verificación SRI</span>
              <span class="value">RCR1783119672725484</span>
            </div>
          </div>
        </div>

        <!-- Address -->
        <div class="footer-col address-col">
          <h4>Ubicación</h4>
          <p>
            Av. Plaza Dañín 26 e Intersección 05,<br>
            (Frente a Andrés Borbor), Parroquia Tarqui,<br>
            Código Postal 090308<br>
            Guayaquil, Guayas, Zona 8<br>
            Ecuador
          </p>
          <div class="tax-badges">
            <span class="badge">IVA</span>
            <span class="badge">Declaración de IVA</span>
          </div>
        </div>
      </div>

      <div class="footer-bottom">
        <p class="developer-credit">
          Hecho por <a href="https://github.com/MrKanx" target="_blank" rel="noopener noreferrer">Kankox</a>
        </p>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Syne:wght@400;700;800&family=Inter:wght@300;400;500&display=swap');

$font-display: 'Syne', sans-serif;
$font-body: 'Inter', sans-serif;
$color-bg: #0a0a0a;
$color-text: #ffffff;
$color-accent: #f2295b;
$color-muted: #888888;

.smooth-scroll-wrapper {
  background-color: $color-bg;
  color: $color-text;
  font-family: $font-body;
  overflow-x: hidden;
  -webkit-font-smoothing: antialiased;
}

/* HERO SECTION */
.hero {
  position: relative;
  height: 100vh;
  width: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding: 2rem 4rem;
  box-sizing: border-box;
  overflow: hidden;

  .hero-bg {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background-size: cover;
    background-position: center;
    transform: scale(1.05);
    animation: slowZoom 20s infinite alternate linear;
    z-index: 1;
  }

  .hero-overlay {
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background: linear-gradient(180deg, rgba(0,0,0,0.3) 0%, rgba(0,0,0,0.8) 100%);
    z-index: 2;
  }

  .nav {
    position: relative;
    z-index: 10;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo {
      font-family: $font-display;
      font-weight: 800;
      font-size: 1.5rem;
      letter-spacing: -0.02em;
    }

    .btn-contact {
      border: 1px solid rgba(255,255,255,0.3);
      padding: 0.75rem 1.5rem;
      border-radius: 50px;
      color: $color-text;
      text-decoration: none;
      font-size: 0.9rem;
      transition: all 0.3s ease;
      backdrop-filter: blur(5px);

      &:hover {
        background: $color-text;
        color: $color-bg;
      }
    }
  }

  .hero-content {
    position: relative;
    z-index: 10;
    margin-bottom: 10vh;

    .reveal-text {
      overflow: hidden;
      .display-title {
        font-family: $font-display;
        font-size: clamp(4rem, 12vw, 10rem);
        font-weight: 800;
        line-height: 0.9;
        margin: 0;
        text-transform: uppercase;
        letter-spacing: -0.04em;
        animation: revealUp 1s cubic-bezier(0.77, 0, 0.175, 1) forwards;
      }
    }

    .hero-subtitle {
      margin-top: 2rem;
      font-size: clamp(1rem, 2vw, 1.5rem);
      font-weight: 300;
      opacity: 0;
      animation: fadeIn 1s ease 1s forwards;
    }
  }

  .scroll-indicator {
    position: absolute;
    bottom: 2rem;
    left: 50%;
    transform: translateX(-50%);
    z-index: 10;
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 0.5rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    letter-spacing: 0.1em;
    opacity: 0.7;

    .mouse {
      width: 20px;
      height: 30px;
      border: 1px solid white;
      border-radius: 10px;
      position: relative;

      &::after {
        content: '';
        position: absolute;
        top: 5px;
        left: 50%;
        transform: translateX(-50%);
        width: 2px;
        height: 5px;
        background: white;
        border-radius: 2px;
        animation: scrollWheel 2s infinite ease-in-out;
      }
    }
  }
}

/* MARQUEE */
.marquee-container {
  padding: 4rem 0;
  background: $color-accent;
  color: $color-bg;
  overflow: hidden;
  white-space: nowrap;

  .marquee {
    display: inline-block;
    animation: marqueeMove 20s linear infinite;
    
    span {
      font-family: $font-display;
      font-weight: 800;
      font-size: 3rem;
      padding-right: 1rem;
    }
  }
}

/* GALLERY */
.gallery {
  padding: 10vw 4rem;

  .gallery-header {
    margin-bottom: 5rem;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    gap: 2rem;
    flex-wrap: wrap;

    .section-title {
      font-family: $font-display;
      font-size: clamp(3rem, 8vw, 6rem);
      line-height: 0.9;
      margin: 0;
    }

    .section-desc {
      max-width: 400px;
      font-size: 1.1rem;
      color: $color-muted;
      line-height: 1.6;
    }
  }

  .gallery-grid {
    display: grid;
    grid-template-columns: repeat(12, 1fr);
    gap: 2rem;

    .gallery-item {
      position: relative;
      overflow: hidden;
      border-radius: 8px;
      cursor: pointer;

      &.large {
        grid-column: span 7;
      }
      &:not(.large) {
        grid-column: span 5;
        margin-top: 10vw;
      }

      .image-wrapper {
        width: 100%;
        height: 100%;
        position: relative;

        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          transition: transform 0.7s cubic-bezier(0.25, 0.46, 0.45, 0.94);
        }

        .item-overlay {
          position: absolute;
          inset: 0;
          background: rgba(0,0,0,0.4);
          display: flex;
          flex-direction: column;
          justify-content: flex-end;
          padding: 2rem;
          opacity: 0;
          transition: opacity 0.4s ease;

          h3 {
            font-family: $font-display;
            font-size: 2rem;
            margin: 0 0 0.5rem;
          }
          p {
            margin: 0;
            font-size: 1rem;
            color: #ddd;
          }
        }
      }

      &:hover {
        .image-wrapper img {
          transform: scale(1.05);
        }
        .item-overlay {
          opacity: 1;
        }
      }
    }
  }
}

/* FOOTER */
.legal-footer {
  background: #050505;
  padding: 6rem 4rem 2rem;
  border-top: 1px solid rgba(255,255,255,0.1);

  .footer-grid {
    display: grid;
    grid-template-columns: 1fr 2fr 1fr;
    gap: 4rem;

    .footer-col {
      h4 {
        font-family: $font-display;
        font-size: 1.2rem;
        margin-bottom: 1.5rem;
        color: #fff;
        font-weight: 700;
      }
      p {
        color: $color-muted;
        font-size: 0.85rem;
        line-height: 1.6;
        margin-bottom: 0.5rem;
      }
      a {
        color: $color-muted;
        text-decoration: none;
        transition: color 0.3s;
        &:hover { color: $color-text; }
      }
    }

    .brand-col {
      .footer-logo {
        font-family: $font-display;
        font-size: 2rem;
        margin: 0 0 1rem;
      }
      .phones {
        font-size: 0.85rem;
        color: $color-muted;
        margin-bottom: 2rem;
      }
      .copyright {
        margin-top: 3rem;
        font-size: 0.75rem;
        opacity: 0.5;
      }
    }

    .address-col {
      .tax-badges {
        display: flex;
        gap: 0.5rem;
        margin-top: 1.5rem;
        flex-wrap: wrap;

        .badge {
          font-size: 0.7rem;
          padding: 0.25rem 0.5rem;
          border: 1px solid rgba(255, 255, 255, 0.15);
          border-radius: 4px;
          color: $color-muted;
          text-transform: uppercase;
          letter-spacing: 0.05em;
          transition: all 0.3s ease;
          cursor: default;

          &:hover {
            border-color: rgba(255, 255, 255, 0.5);
            color: #fff;
            background: rgba(255, 255, 255, 0.05);
          }
        }
      }
    }

    .legal-data {
      .data-grid {
        display: grid;
        grid-template-columns: 1fr 1fr;
        gap: 1.5rem 2rem;
        
        .data-item {
          display: flex;
          flex-direction: column;
          gap: 0.2rem;

          &.span-2 {
            grid-column: span 2;
          }

          .label {
            font-size: 0.7rem;
            text-transform: uppercase;
            letter-spacing: 0.05em;
            color: #555;
          }
          .value {
            font-size: 0.85rem;
            color: #ccc;
          }
        }
      }
    }
  }

  .footer-bottom {
    margin-top: 3rem;
    padding-top: 1.5rem;
    border-top: 1px solid rgba(255, 255, 255, 0.05);
    text-align: center;

    .developer-credit {
      font-size: 0.8rem;
      color: #555;
      letter-spacing: 0.05em;

      a {
        color: #777;
        text-decoration: underline;
        text-underline-offset: 3px;
        transition: color 0.3s ease;

        &:hover {
          color: #ccc;
        }
      }
    }
  }
}

/* ANIMATIONS */
@keyframes slowZoom {
  0% { transform: scale(1) translate(0, 0); }
  100% { transform: scale(1.1) translate(-2%, 2%); }
}
@keyframes revealUp {
  0% { transform: translateY(100%); opacity: 0; }
  100% { transform: translateY(0); opacity: 1; }
}
@keyframes fadeIn {
  to { opacity: 1; }
}
@keyframes scrollWheel {
  0% { transform: translate(-50%, 0); opacity: 1; }
  100% { transform: translate(-50%, 15px); opacity: 0; }
}
@keyframes marqueeMove {
  0% { transform: translateX(0); }
  100% { transform: translateX(-50%); }
}

/* RESPONSIVE */
@media (max-width: 1024px) {
  .hero { padding: 2rem; }
  .gallery { padding: 5vw 2rem; }
  .legal-footer .footer-grid {
    grid-template-columns: 1fr;
    gap: 3rem;
  }
  .gallery .gallery-grid {
    .gallery-item {
      &.large, &:not(.large) {
        grid-column: span 12;
        margin-top: 0;
      }
    }
  }
}
@media (max-width: 768px) {
  .legal-footer .legal-data .data-grid {
    grid-template-columns: 1fr;
    
    .span-2 {
      grid-column: span 1;
    }
  }
}
</style>
