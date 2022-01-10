<template>

  <q-page class="row page-bg" >

    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input dense placeholder="Search" borderless class="full-width" :model-value="search" >
          <template #append> <q-icon name = "mdi-magnify"/></template>
        </q-input>
      </q-toolbar>
          <TodosList bordered/>
        </q-card>
        <div class='col-xs-3'>
          <q-toolbar class="bg-primary">
            <CreateTodoButton/>
          </q-toolbar>
        </div>
    </q-page>

</template>

<script>
import CreateTodoButton from 'src/components/CreateTodoListButton.vue'
import TodosList from 'src/components/TodosList.vue'
import { defineComponent } from 'vue'
export default defineComponent({

  name: 'PageIndex',
  components: {
    CreateTodoButton,
    TodosList
  },

  data () {
    return {
      selected: null
    }
  }
})
</script >

<style lang="scss">
.page-bg{
  background: $blue-1;
}

</style>
