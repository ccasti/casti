<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-4-desktop is-size-5-mobile">Capacitación</p>
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
                <img class="img-up" src="../assets/icap.png">
              </figure>
            </div>
          </div>
          <div class="columns">
            <div class="column has-text-justified info-content">
              <p class="is-size-5-desktop is-size-5-tablet is-size-6-mobile">
                Experiencia diseñando y ejecutando programas de capacitación que generan resultados tangibles en personas y equipos.<br/>
                Combino metodologías de aprendizaje activo con herramientas digitales interactivas, logrando experiencias formativas dinámicas y adaptadas a las necesidades de cada organización.<br/><br/>
                Mi especialidad son las instancias digitales, que facilitan el acceso, la personalización y el seguimiento del aprendizaje.<br/><br/>
                Integro el modelo de Coaching en cada proyecto cuando es pertinente, promoviendo la reflexión, el autoconocimiento y el desarrollo continuo, para que la capacitación no sea solo un evento, sino un proceso transformador con impacto real en el desempeño y el clima laboral.<br/><br/>
                Revisa un demo de instancia de capacitación digital.<br/>
              </p>
              <button
                id="cap"
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
      
      this.targetUrl = 'https://cap.webcoach.cl/'

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
