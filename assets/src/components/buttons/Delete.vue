<template>
  <button @click="show" aria-label="Delete"  title="Delete" class="action" id="delete-button">
    <i class="material-icons">delete</i>
    <span>Delete</span>
  </button>
</template>

<script>
export default {
  name: 'delete-button',
  methods: {
    show: function (event) {
      this.$store.commit('showHover', 'delete')
    }
  }
}
</script>
