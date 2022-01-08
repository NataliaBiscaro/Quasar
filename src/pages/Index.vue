<template>

  <q-page class="row">

    <q-card class="col-xs-9">
      <q-toolbar>
        <q-input dense placeholder="Search" borderless class="full-width" :model-value="search" >
          <template #append> <q-icon name = "mdi-magnify"/></template>
        </q-input>
      </q-toolbar>
          <q-list bordered>
            <q-item>
              <q-item-section side>
                <q-checkbox :model-value="true"></q-checkbox>
              </q-item-section>
                <q-item-section> Go Shopping </q-item-section>
                <q-item-section side>
                  <q-btn size="sm" flat round icon="mdi-delete"></q-btn>
                </q-item-section>
            </q-item>
          </q-list>
        </q-card>
        <div class='col-xs-3'>
          <q-toolbar class="bg-primary">
            <q-btn
              fab style="margin-bottom: -45px;"
              class="q-ml-md"
              color = 'green-4'
              icon="mdi-plus"/>
          </q-toolbar>
        </div>
    </q-page>

</template>

<script>
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'PageIndex',

  data () {
    return {
      selected: null
    }
  }
})
</script >
