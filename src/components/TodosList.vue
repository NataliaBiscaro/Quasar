<template>
  <q-list>
    <q-item>
      <q-item-section side>
        <UpdateTodoCheckbox/>
      </q-item-section>
          <q-item-section> Go Shopping </q-item-section>
            <q-item-section side>
              <q-btn size="sm" flat round icon="mdi-delete"></q-btn>
            </q-item-section>
      </q-item>
  </q-list>
</template>

<script>
import UpdateTodoCheckbox from 'src/components/UpdateTodoCheckbox.vue'
export default {
  components: {
    UpdateTodoCheckbox
  }
}
</script>
