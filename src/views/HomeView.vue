<script></script>

<template>
  <main class="home">
    <!-- Landing Section -->
    <section class="landing">
      <article class="profile-section">
        <header class="profile-header">
          <figure class="profile-image">
            <img src="../assets/mario_isamitt.jpg" alt="Dr. Mario Isamitt" width="250" height="250">
          </figure>
          <p class="big-shoulders-text name">Dr. Mario Isamitt</p>
          <p class="specialty">Medicina general y deportiva</p>
        </header>
      </article>

      <nav class="actions">
        <a href="https://www.doctoralia.cl/mario-isamitt-pualuan/medico-general/concepcion" class="action-button" target="_blank"  role="button">
          Agendar hora consulta
        </a>
        <a href="https://www.facebook.com/mario.isamitt" target="_blank" class="action-button" role="button">
          Perfil Facebook
        </a>
        <a href="https://www.instagram.com/mario.isamitt/" class="action-button" target="_blank"  role="button">
          Perfil Instagram
        </a>
        <a href="https://www.amazon.com/viaje-salud-Spanish-Mario-Isamitt/dp/9564091381" class="action-button" target="_blank"  role="button">
          Libro "Un viaje a la salud"
        </a>
      </nav>

      <section class="contact-info">
        <h2>Contacto:</h2>
        <ul class="contact-list">
          <li>Fono Diagnomed: <a href="tel:6004010019">600 401 0019</a></li>
          <li>Correo: <a href="mailto:medico@marioisamitt.com">medico@marioisamitt.com</a></li>
        </ul>
      </section>
    </section>

    <!-- About Section -->
    <section class="about">
      <article class="about-content">
        <header>
          <h2 class="big-shoulders-text">SOBRE MÍ</h2>
        </header>
        <p class="about-text">
          Mi norte, como médico, es acercar la salud a las personas. A través de la promoción de hábitos saludables —deporte, nutrición y consciencia—, y su correcta aplicación, busco elevar tu bienestar físico, mental y social. 
Durante la consulta me esforzaré en encontrar el origen de tu dolencia. Una vez identificada la causa te enseñaré a comprenderla para que, cuando sea posible, puedas corregir con tus propias herramientas aquello que te está enfermando. 
Me comprometo a escucharte con atención y tratarte con respeto. Me sentiré feliz y agradecido si logro ayudarte.
        </p>
        <footer class="about-signature">
          <h2 class="big-shoulders-text">Dr. Mario Isamitt</h2>
        </footer>
      </article>

      <figure class="about-image">
        <img src="../assets/mario_isamitt.jpg" alt="Dr. Mario Isamitt en consulta">
      </figure>
    </section>
  </main>
</template>

<style>
:root {
  --primary-color: #150B3B;
  --secondary-color: #200688;
  --accent-color: #E8F1FB;
  --text-color: #484756;
  --gray-color:#D9D9D9;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.home {
  font-family: "Karla", sans-serif;
  line-height: 1.6;
  color: var(--text-color);
}

/* Landing Section */
.landing {
  background: var(--accent-color);
  padding: 2rem;
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.profile-header {
  text-align: center;
  margin-bottom: 2rem;
}

.profile-image {
  width: 200px;
  height: 200px;
  border-radius: 10px;
  background: var(--primary-color);
  margin: 0 auto;
}

img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 20px;
}

.contact-info {
  order: 2; /* Moves it to the bottom in flex layout */
}

.contact-list {
  margin-top: 1rem;
}

.contact-list li {
  margin-bottom: 0.5rem;
  margin-left: 2rem;
}

/* Actions */
.actions {
  order: 1;
  display: grid;
  gap: 2.5rem;
  background-color: var(--secondary-color);
  padding: 2rem 1rem;
  border-radius: 15px;
}

.action-button {
  background: white;
  padding: 0.5rem;
  border-radius: 30px;
  text-decoration: none;
  color: var(--text-color);
  text-align: center;
  box-shadow: 4px 4px 4px rgba(0, 0, 0, 0.25);
  transition: transform 0.2s ease;
}

/* About Section */
.about {
  padding: 2rem;
  display: grid;
  gap: 2rem;
}

.about-content {
  max-width: 800px;
  margin: 0 auto;
  text-align: center;
}

.about-text {
  margin: 1.5rem 0;
}

.about-image {
  width: 80%;
  height: auto;
  margin: 0 auto;
  border-radius: 30px;
  background: var(--gray-color);
  display: none;
}

.about-image img {
  width: 100%;
  height: auto;
  border-radius: 10px;
}

/* Typography */
.big-shoulders-text {
  font-family: "Big Shoulders Text", sans-serif;
}

h1 { font-size: 2.5rem; }
h2 { font-size: 2rem; }

/* Desktop layout */
@media (min-width: 768px) {
  .landing {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: center;
    min-height: 100vh;
  }

  .profile-image {
  width: 250px;
  height: 250px;
  border-radius: 15px;
  background: var(--primary-color);
  margin: 0 auto 1rem;
}

  .name {
    font-size: 2rem;
  }

  .specialty {
    font-size: 2rem;
  }

  .contact-info {
    order: initial; /* Reset order for grid layout */
    margin-left: 2rem;
  }

  .actions {
    order: initial;
    padding: 3rem 2rem;
    margin: 5rem 3rem;
    gap: 5rem;
  }

  .action-button {
    font-size: 1.25rem;
    padding: 0.4rem;
    border-radius: 10px;
  }

  .about {
    grid-template-columns: 1fr 1fr;
    align-items: center;
    min-height: 100vh;
  }
  .about-content {
    padding: 15%;
  }
  .about-image {
    display: block;
  }

}
</style>
