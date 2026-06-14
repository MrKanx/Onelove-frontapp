<script setup lang="ts">
// Componente de página única para MOKALU S.A.S.
</script>

<template>
  <div class="app-container">
    <header class="header">
      <div class="header-content">
        <h1>MOKALU S.A.S.</h1>
        <p class="subtitle">Portafolio Comercial y Verificación Tributaria</p>
      </div>
    </header>

    <main class="main-content">
      <section class="card">
        <h2>Información General</h2>
        <ul class="info-list">
          <li><strong>Razón Social:</strong> MOKALU S.A.S.</li>
          <li><strong>Número RUC:</strong> 0993285811001</li>
          <li><strong>Representante Legal:</strong> Oyola Galarza Monica Alexandra</li>
          <li><strong>Tipo de Contribuyente:</strong> Sociedades</li>
          <li><strong>Estado:</strong> Activo</li>
          <li><strong>Régimen:</strong> RIMPE Emprendedor</li>
          <li><strong>Obligado a llevar contabilidad:</strong> No</li>
        </ul>
      </section>

      <section class="card">
        <h2>Actividades Económicas</h2>
        <ul class="info-list">
          <li>Venta al por mayor de material de papelería.</li>
          <li>Venta al por menor de artículos de papelería como lápices, bolígrafos, papel, etc., en establecimientos especializados.</li>
        </ul>
      </section>

      <section class="card">
        <h2>Ubicación y Domicilio Tributario</h2>
        <ul class="info-list">
          <li><strong>Jurisdicción:</strong> Zona 8 / Guayas / Guayaquil</li>
          <li><strong>Dirección:</strong> Vía a la Costa Km 12.5, C.C. Laguna Plaza, Local 317 (Primer piso alto junto al ascensor), Parroquia Tarqui.</li>
        </ul>
      </section>

      <section class="card">
        <h2>Medios de Contacto</h2>
        <div class="contact-grid">
          <div class="contact-item">
            <strong>Ventas:</strong>
            <a href="mailto:mokaluventas@gmail.com">mokaluventas@gmail.com</a>
            <a href="tel:0967472310">0967472310</a>
          </div>
          <div class="contact-item">
            <strong>Administración:</strong>
            <a href="mailto:lamg5208@gmail.com">lamg5208@gmail.com</a>
            <a href="tel:0983849378">0983849378</a>
          </div>
        </div>
      </section>

      <section class="card">
        <h2>Información de Constitución y SRI</h2>
        <ul class="info-list">
          <li><strong>Fecha de constitución:</strong> 20/10/2020</li>
          <li><strong>Inicio de actividades:</strong> 23/10/2020</li>
          <li><strong>Establecimientos abiertos:</strong> 1</li>
          <li><strong>Código de verificación (SRI):</strong> CATRCR2022002933710</li>
        </ul>
        <div class="tax-obligations">
          <h3>Obligaciones Tributarias</h3>
          <ul class="tag-list">
            <li>Declaración Semestral IVA</li>
            <li>Impuesto a la Renta Sociedades</li>
            <li>Anexo Relación Dependencia</li>
            <li>Anexo Transaccional Simplificado</li>
            <li>Anexo Socios / Accionistas</li>
            <li>Anexo de Dividendos (ADI)</li>
          </ul>
        </div>
      </section>
    </main>

    <footer class="footer">
      <p>&copy; {{ new Date().getFullYear() }} MOKALU S.A.S. Todos los derechos reservados.</p>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
.app-container {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  background-color: #f4f6f9;
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
  color: #333;
}

.header {
  background: linear-gradient(135deg, #1e3c72 0%, #2a5298 100%);
  color: white;
  padding: 3rem 1rem;
  text-align: center;

  .header-content {
    max-width: 800px;
    margin: 0 auto;

    h1 {
      margin: 0;
      font-size: 2.5rem;
      font-weight: 700;
      letter-spacing: 1px;
    }

    .subtitle {
      margin-top: 0.5rem;
      font-size: 1.2rem;
      opacity: 0.9;
    }
  }
}

.main-content {
  flex: 1;
  max-width: 900px;
  margin: -2rem auto 2rem;
  padding: 0 1rem;
  display: grid;
  gap: 1.5rem;
  width: 100%;
  box-sizing: border-box;
}

.card {
  background: white;
  border-radius: 12px;
  padding: 2rem;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05), 0 1px 3px rgba(0, 0, 0, 0.1);
  transition: transform 0.2s ease, box-shadow 0.2s ease;

  &:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(0, 0, 0, 0.08);
  }

  h2 {
    margin-top: 0;
    color: #1e3c72;
    font-size: 1.4rem;
    border-bottom: 2px solid #e2e8f0;
    padding-bottom: 0.5rem;
    margin-bottom: 1.5rem;
  }
}

.info-list {
  list-style: none;
  padding: 0;
  margin: 0;

  li {
    margin-bottom: 0.75rem;
    line-height: 1.5;
    
    strong {
      color: #4a5568;
      display: inline-block;
      min-width: 200px;
    }
  }
}

.contact-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;

  .contact-item {
    display: flex;
    flex-direction: column;
    gap: 0.5rem;

    strong {
      color: #4a5568;
    }

    a {
      color: #2a5298;
      text-decoration: none;
      font-weight: 500;
      transition: color 0.2s;

      &:hover {
        color: #1e3c72;
        text-decoration: underline;
      }
    }
  }
}

.tax-obligations {
  margin-top: 2rem;

  h3 {
    font-size: 1.1rem;
    color: #4a5568;
    margin-bottom: 1rem;
  }
}

.tag-list {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
  list-style: none;
  padding: 0;
  margin: 0;

  li {
    background-color: #e2e8f0;
    color: #4a5568;
    padding: 0.4rem 0.8rem;
    border-radius: 9999px;
    font-size: 0.85rem;
    font-weight: 500;
  }
}

.footer {
  text-align: center;
  padding: 2rem;
  background-color: #2d3748;
  color: #cbd5e0;
  font-size: 0.9rem;
}

@media (max-width: 768px) {
  .main-content {
    margin-top: 1rem;
  }

  .info-list li strong {
    display: block;
    margin-bottom: 0.25rem;
  }
}
</style>
