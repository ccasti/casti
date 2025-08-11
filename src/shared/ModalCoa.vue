<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-4-desktop is-size-5-mobile">Coaching</p>
        <button @click="closeModal" class="delete" aria-label="close"></button>
      </header>
      <section class="modal-card-body">
        <div class="container">
          <div class="columns">
            <div class="column is-paddingless">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-centered">
                <strong>Se complementa con:</strong><br/>
              </p>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-4-desktop is-offset-4-desktop is-4-tablet is-offset-4-tablet is-6-mobile is-offset-3-mobile">
              <figure class="image">
                <img class="img-up" src="../assets/icoa.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-justified">
                <strong>Más de 12 años potenciando personas y equipos</strong><br/>
                Combino mi experiencia en <strong>Coaching</strong> con habilidades en <strong>Capacitación</strong> y <strong>Desarrollo Web</strong> para impulsar el crecimiento personal y profesional.<br/><br/>
                Me especializo en fortalecer competencias clave como:<br/><br/>
                <strong>- Inteligencia Emocional</strong><br/>
                <strong>- Comunicación Efectiva</strong><br/>
                <strong>- Escucha Activa</strong><br/>
                <strong>- Trabajo en Equipo</strong><br/>
                <strong>- Liderazgo</strong><br/>
                <strong>- Motivación</strong><br/><br/>
                Integro el <strong>Coaching</strong> en cada proyecto, creando espacios de trabajo productivos y estrategias de gestión de personas con impacto real.<br/>
                El <strong>Desarrollo Web</strong> me permite diseñar herramientas digitales de autoconocimiento y reflexión, que enriquecen los procesos formativos.<br/><br/>
                Debajo encontrarás <strong>"Carta a mi niñez"</strong>, una experiencia emotiva de reflexión y autodescubrimiento, diseñada para reconectar con lo que define quién eres.
              </p>
            </div>
          </div>
          <div class="columns">
            <div class="column is-8-desktop is-offset-2-desktop">
              <div class="box-frame">
                <iframe allowfullscreen src="https://ht3.webcoach.cl/"></iframe>    
              </div>
            </div>
          </div>
        </div>
      </section>
      <footer class="modal-card-foot"></footer>
    </div>
  </div>
</template>

<script>

export default {

  methods: {

    closeModal () {this.$emit('clickCloseModal')}

  }
 }

</script>

<style lang="scss" scoped>

  .modal-card-head {
    background-color: #003366;
    border: none;
  }

  .modal-card-title {
    color: #FFF;
  }

  .delete {
    color: #003366;
  }

  .box-frame {
    width: 100%;
    aspect-ratio: 16 / 9;
    border-radius: 10px;
    border: 6px solid #003366;
  }

  iframe {
    width: 100%;
    height: 100%;
  }

  .modal-card-foot {
    background-color: #003366;
    padding: 12px;
  }

</style>