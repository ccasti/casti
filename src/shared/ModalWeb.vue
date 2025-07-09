<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-card">
      <header class="modal-card-head">
        <p class="modal-card-title is-size-3-desktop is-size-5-mobile">Desarrollo de Entornos Web</p>
        <button @click="closeModal" class="delete" aria-label="close"></button>
      </header>
      <section class="modal-card-body">
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
        <p>listado de algo <br/></p>
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
