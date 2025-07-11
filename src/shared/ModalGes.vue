<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-4-desktop is-size-5-mobile">Finanzas</p>
        <button @click="closeModal" class="delete" aria-label="close"></button>
      </header>
      <section class="modal-card-body">
        <div class="container">
          <div class="columns">
            <div class="column is-paddingless">
              <p class="is-size-5-desktop is-size-6-mobile has-text-centered">
                <strong>Se complementa con:</strong><br/>
              </p>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-4-desktop is-offset-4-desktop is-6-mobile is-offset-3-mobile">
              <figure class="image">
                <img class="img-up" src="../assets/ifin.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-6-mobile has-text-justified">
                Durante mis 14 años de experiencia en la industria financiera, trabajando siempre con empresas, he cultivado un sólido conocimiento de análisis y control financiero, tales como:<br/><br/>
                <strong>- Determinación de posición financiera.</strong><br/>
                <strong>- Análisis de capacidades de Pago.</strong><br/>
                <strong>- Análisis de flujos y desfaces de caja.</strong><br/>
                <strong>- Estructuras de financiamiento.</strong><br/>
                <strong>- Mitigación riesgos tipo de cambio.</strong><br/><br/>
                El Coaching está presente en todas mis gestiones como profesional, principalmente en las interacciones con personas, facilitando espacios de trabajo productivos.<br/><br/>
                Todas las instancias de <strong>Capacitación </strong>que diseño y desarrollo tienen incorporados los conceptos del Coaching para el potenciamiento de las personas, siendo parte integral de una estrategia de gestión de personas.<br/>
                El <strong>Desarrollo Web</strong> me permite implementar instancias digitales de autoconocimiento y reflexión, que aportan información importante a los procesos de desarrollo de las personas.<br/><br/>
                <strong>Conoce mi trabajo en la ventana de más abajo</strong>, se trata de una dinámica llamada "Carta a mi niñez", una poderosa y emotiva instancia de reflexión y autodescubrimiento diseñada para conectarte con todo aquello que define a la persona que eres.
              </p>
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

  .modal-card-foot {
    background-color: #003366;
    padding: 12px;
  }

</style>
