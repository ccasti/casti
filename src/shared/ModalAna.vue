<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-4-desktop is-size-5-mobile">Análisis de Datos</p>
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
                <img class="img-up" src="../assets/iana.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column has-text-justified info-content">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                <strong>Análisis de Datos y Finanzas</strong><br/>
                Con más de 14 años de experiencia en análisis y control financiero, aplico técnicas avanzadas de análisis de datos para profundizar en información financiera, identificar patrones de comportamiento, detectar anomalías y generar modelos predictivos que apoyan la planificación estratégica y la gestión de riesgos.<br/><br/>
                <strong>Análisis de Datos y Desarrollo Web</strong><br/>
                Diseño entornos web interactivos para visualización y narrativa de datos, integrando múltiples dashboards en una sola plataforma flexible y adaptada a las necesidades de cada usuario. Estas soluciones permiten contextualizar la información, optimizar su interpretación y facilitar la toma de decisiones basada en datos.<br/><br/>
                Revisa un demo de instancia de capacitación digital.<br/>
              </p>
              <button
                id="ana"
                class="button is-rounded"
                @click="go">
                Ir al demo</button>
              <p
                v-show="showTextRedirect"
                class="is-size-5-desktop is-size-5-tablet is-size-6-mobile text-redirect">
                <strong>Estás siendo redirigido al demo</strong>
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

  data () {

    return {

      showTextRedirect: false,
      targetId: '',
      targetUrl: ''
    
    }
  },

  methods: {

    closeModal () {this.$emit('clickCloseModal')},

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

        this.showTextRedirect = true
        
      }, 900);

      setTimeout(() => {
        location.href = this.targetUrl
      }, 2400);
    
    },

    go (ev) {
      this.click(ev)
      
      this.targetUrl = 'https://censo.webcoach.cl/'

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

  .info-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
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

  .delete {
    color: #003366;
  }

  .modal-card-foot {
    background-color: #003366;
    padding: 12px;
  }

  @media screen and (max-width: 768px) {
    
    .button {
      box-shadow: 0px 12px 6px -3px #000033;
      transition: all 300ms;
      -webkit-tap-highlight-color: transparent;
      opacity: 1;
    }
  }

</style>
