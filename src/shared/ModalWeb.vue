<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-4-desktop is-size-5-mobile">Desarrollo de Entornos Web</p>
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
                <img class="img-up" src="../assets/iweb.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <div class="card-option">
                <header @click="toggleOption2" class="card-header">
                  <p class="card-header-title is-paddingless is-size-4-desktop is-size-6-mobile">
                    Análisis de datos
                  </p>
                </header>
                <transition name="expand">
                  <div v-show="showOption2" class="card-content has-text-justified">
                    <p class="is-size-5-desktop is-size-6-mobile has-text-justified">
                      Desarrollo de dashboards interactivos para la visualización de datos, customizados según el consumidor de la información, esto permite múltiples opciones de organización y configuracion, al implementarse en una instancia web, cada usuario autorizado con el link podrá realizar una revisión independiente respecto de la información y datos, además de obtener una interfaz amigable, permite incorporar contexto, comentarios, etc. Ideal para presentaciones corporativas y directorios.<br/>
                      <strong>Revisar instancia de Análisis de Datos en Expertises.</strong>
                    </p>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <div class="card-option">
                <header @click="toggleOption3" class="card-header">
                  <p class="card-header-title is-paddingless is-size-4-desktop is-size-6-mobile">
                    Capacitación
                  </p>
                </header>
                <transition name="expand">
                  <div v-show="showOption3" class="card-content has-text-justified">
                    <p class="is-size-5-desktop is-size-6-mobile has-text-justified">
                      Desarrollo de instancias digitales interactivas de capacitación.<br/>
                      Desarrollo de test digitales de evaluación de actitudes y conocimientos para uso de recursos humanos en el desarrollo de personas además de los procesos de selección y reclutamiento, permitiendo un ahorro en recursos al automatizar el levantamiento de información y evaluación.
                      <strong>Revisar demo en instancia de Capacitación en Expertises.</strong>
                    </p>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-6-mobile has-text-justified">
                <strong>Todas las instancias de este sitio web fueron programadas por mí</strong>, para realizarlo utilicé mis habilidades de maquetación en HTML, estilos, transiciones y animaciones con CSS e interacciones y dinamismo del sitio con JavaScript, además del framework Vue2.<br/><br/>
                Otras Habilidades en el desarrollo web:
              </p>
             </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                Consumo de API´s
              </p>
              <progress class="progress is-link" value="95" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                Vue
              </p>
              <progress class="progress is-link" value="75" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                Python
              </p>
              <progress class="progress is-link" value="40" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                SQL
              </p>
              <progress class="progress is-link" value="50" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                HTML
              </p>
              <progress class="progress is-link" value="95" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                CSS
              </p>
              <progress class="progress is-link" value="90" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-6-mobile">
                JavaScript
              </p>
              <progress class="progress is-link" value="85" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2 last">
              <p class="is-size-5-desktop is-size-6-mobile">
                Git y GitHub
              </p>
              <progress class="progress is-link" value="75" max="100"></progress>
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

  data () {

    return {

      showOption2: false,
      showOption3: false,
    
    }
  },

  methods: {

    closeModal () {this.$emit('clickCloseModal')},

    toggleOption2 (ev) {
      ev.preventDefault()
      if (this.showOption2) {
        this.showOption2 = false
      } else {
        this.showOption2 = true
      }
    },

    toggleOption3 (ev) {
      ev.preventDefault()
      if (this.showOption3) {
        this.showOption3 = false
      } else {
        this.showOption3 = true
      }
    }

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

  .card-option {
    background-color: #fff;
    border: 3px solid #003366;
    border-radius: 9px;
    margin-bottom: .3rem;
  }

  .card-option:hover {
    box-shadow: 0px 6px 6px 0px #003366;
  }

  .last {
    margin-bottom: 2.4rem;
  }

  .modal-card-foot {
    background-color: #003366;
    padding: 12px;
  }

  @media screen and (max-width: 768px) {
    .card-option {
      box-shadow: 0px 3px 3px 0px #003366;
      margin-bottom: 0;
    }
  }

</style>
