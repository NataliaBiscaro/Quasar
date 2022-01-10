<template>
<q-page class="flex flex-center" padding>
    <div class="full-width" style="max-width: 418px;">
        <h5 class="q-my-md text-center"> Login </h5>
    <q-card>
      <q-card-section>
        <q-form>
          <q-input filled label="E-mail" placeholder="email@example.com" class="q-my-md"/>
          <q-input filled label="Password" type="password" class="q-my-sm"/>
          <q-checkbox :model-value="true" label="Remember me"/>
      </q-form>
      </q-card-section>
      <q-btn label="login" class="full-width" color="primary"/>
    </q-card>

    </div>

  </q-page>
</template>

<script>
export default {
  // name: 'PageName',
}
</script>
