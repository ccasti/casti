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
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-centered">
                <strong>Se complementa con:</strong><br/>
              </p>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-4-desktop is-offset-4-desktop is-4-tablet is-offset-4-tablet is-6-mobile is-offset-3-mobile">
              <figure class="image">
                <img class="img-up" src="../assets/iweb.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-justified">
                Pulsa en cada barra para ver el detalle y un demo interactivo.
              </p>
             </div>
          </div>
          <div class="columns">
            <div class="column is-full">
              <div class="card-option">
                <header @click="toggleOption2" class="card-header">
                  <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                    Análisis de datos
                  </p>
                </header>
                <transition name="expand">
                  <div v-show="showOption2" class="card-content has-text-justified">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Entornos web personalizados para la presentación enriquecida de datos<br/>
                      Desarrollo entornos web a medida que integran múltiples dashboards, ofreciendo una experiencia mucho más rica y dinámica que una presentación tradicional o un dashboard individual. Estas interfaces se diseñan según las necesidades específicas de los usuarios, permitiendo organizar, contextualizar y narrar los datos con interacción y flexibilidad.<br/><br/>
                      Revisa un demo preparado con los datos del censo nacional del año 2024.<br/>
                    </p>
                    <button
                      id="ad"
                      class="button is-rounded"
                      @click="go">
                      Ir al demo</button>
                    <p
                      v-show="showTextRedirectAD"
                      class="is-size-5-desktop is-size-5-tablet is-size-6-mobile text-redirect">
                      <strong>Estás siendo redirigido al demo</strong>
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
                  <p class="card-header-title is-paddingless is-size-4-desktop is-size-5-tablet is-size-6-mobile">
                    Capacitación
                  </p>
                </header>
                <transition name="expand">
                  <div v-show="showOption3" class="card-content has-text-justified">
                    <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                      Diseño y desarrollo de entornos digitales interactivos para capacitación, optimizados para maximizar la participación y el aprendizaje.<br/>
                      Creación de evaluaciones en línea para medir conocimientos y actitudes, orientadas a procesos de desarrollo de talento, reclutamiento y selección. Estas soluciones permiten automatizar la recopilación y análisis de información, optimizando recursos y mejorando la eficiencia de los procesos de Recursos Humanos.<br/><br/>
                      Revisa un demo de instancia de capacitación digital.<br/>
                    </p>
                    <button
                      id="c"
                      class="button is-rounded"
                      @click="go">
                      Ir al demo</button>
                    <p
                      v-show="showTextRedirectC"
                      class="is-size-5-desktop is-size-5-tablet is-size-6-mobile text-redirect">
                      <strong>Estás siendo redirigido al demo</strong>
                    </p>
                  </div>   
                </transition>
              </div>
            </div>
          </div>
          <div class="columns">
            <div class="column">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile has-text-justified">
                <strong>Todas las interfaces de este sitio web fueron programadas por mí</strong>, para realizarlo utilicé mis habilidades de maquetación en HTML, estilos, transiciones y animaciones con CSS e interacciones y dinamismo del sitio con JavaScript, además del framework Vue2.<br/><br/>
                Otras Habilidades en el desarrollo web:
              </p>
             </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Consumo de API´s
              </p>
              <progress class="progress is-link" value="95" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Vue
              </p>
              <progress class="progress is-link" value="75" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Python
              </p>
              <progress class="progress is-link" value="40" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                SQL
              </p>
              <progress class="progress is-link" value="50" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                HTML
              </p>
              <progress class="progress is-link" value="95" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                CSS
              </p>
              <progress class="progress is-link" value="90" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                JavaScript
              </p>
              <progress class="progress is-link" value="85" max="100"></progress>
            </div>
          </div>
          <div class="columns is-mobile">
            <div class="column is-8 is-offset-2 last">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
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
      showTextRedirectAD: false,
      showTextRedirectC: false,
      targetId: '',
      targetUrl: ''
    
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
    },

    click (ev) {
      ev.preventDefault()
      this.targetId = ev.target.id
      
      document.getElementById(this.targetId).style.boxShadow = "0px 6px 6px 0px #000033";
      setTimeout(() => {
        document.getElementById(this.targetId).style.boxShadow = "0px 12px 6px -3px #000033";
      }, 300)

      setTimeout(() => {
        document.getElementById(this.targetId).classList.add('is-loading')
      }, 600);
    },

    redirecting () {

      setTimeout(() => {
        if (this.targetId == 'ad') {
          this.showTextRedirectAD = true  
        }
        if (this.targetId == 'c') {
          this.showTextRedirectC = true
        }
      }, 900);

      setTimeout(() => {
        location.href = this.targetUrl
      }, 2400);
    
    },

    go (ev) {
      this.click(ev)
      
      if (this.targetId == 'ad') {
        this.targetUrl = 'https://censo.webcoach.cl/'
      }
      if (this.targetId == 'c') {
        this.targetUrl = 'https://cap.webcoach.cl/'
      }

      this.redirecting()
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

  .card-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
  }

  .last {
    margin-bottom: 2.4rem;
  }

  .button {
    margin: 3rem auto;
    background-color: #003366;
    border-color: #003366 !important;
    color: #fff;
    box-shadow: 0px 6px 6px 0px #000033;
    transition: all 300ms;
    -webkit-tap-highlight-color: transparent;
    opacity: .9;
  }

  .button:hover {
    box-shadow: 0px 12px 6px -3px #000033;
    color: #fff !important;
    opacity: 1;
  }

  .text-redirect {
    align-self: center ;
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

    .button {
      box-shadow: 0px 12px 6px -3px #000033;
      transition: all 300ms;
      -webkit-tap-highlight-color: transparent;
      opacity: 1;
    }
  }

</style>
