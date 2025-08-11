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
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-centered">
                <strong>Se complementa con:</strong><br/>
              </p>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-4-desktop is-offset-4-desktop is-4-tablet is-offset-4-tablet is-6-mobile is-offset-3-mobile">
              <figure class="image">
                <img class="img-up" src="../assets/ifin.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-justified">
                Con más de 14 años de trayectoria en la industria financiera, he desarrollado un profundo conocimiento en análisis y control financiero aplicado a empresas.<br/><br/>
                Además, complemento esta experiencia con habilidades avanzadas en análisis de datos para potenciar la precisión y profundidad en la interpretación financiera y la toma de decisiones.<br/><br/>
                Mis habilidades en finanzas:
              </p>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Evaluación de posición financiera.
              </p>
              <progress class="progress is-link" value="96" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Análisis de capacidades de pago.
              </p>
              <progress class="progress is-link" value="96" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Presupuesto y Forecasting
              </p>
              <progress class="progress is-link" value="85" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Gestión de Costos
              </p>
              <progress class="progress is-link" value="90" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Gestión de flujos y desfases de caja.
              </p>
              <progress class="progress is-link" value="96" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Optimización de estructuras de financiamiento.
              </p>
              <progress class="progress is-link" value="90" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Mitigación estratégica de riesgos cambiarios.
              </p>
              <progress class="progress is-link" value="85" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2 last">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Conocimiento Tributario Básico
              </p>
              <progress class="progress is-link" value="87" max="100"></progress>
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

  .last {
    margin-bottom: 2.4rem;
  }

  .modal-card-foot {
    background-color: #003366;
    padding: 12px;
  }

</style>
