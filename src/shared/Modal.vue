<template>
  <div class="modal">
    <div class="modal-background"></div>
    <div class="modal-content">
      <p class="image is-4by4">
        <img :src="modal">
      </p>
    </div>
    <button
      class="modal-close is-large"
      aria-label="close"
      @click="closeModal">
    </button>
  </div>
</template>

<script>

export default {

  props: {
    modal: { type: String, required: true }
  },

  methods: {

    closeModal () {this.$emit('clickCloseModal')}

  }
 }

</script>

<style lang="scss" scoped>

  

</style>
