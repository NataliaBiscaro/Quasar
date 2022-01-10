<template>
  <q-btn  @click="handleButtonClicked" size="md" color="secondary" float round icon="mdi-plus"/>
</template>

<script>
export default {
  methods: {
    handleButtonClicked () {
      this.$q.dialog({
        title: 'Create Todo',
        prompt: {
          model: '',
          type: 'text'
        }
      })
        .onOk(this.createTodo)
    },
    createTodo (data) {
      this.$q.notify({
        message: 'Todo Created! :D',
        icon: 'mdi-check',
        color: 'positive'
      })
    }
  }
}
</script>
