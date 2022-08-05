<template>
  <q-page class="flex flex-center bg-secondary" >
    <q-card class="" style="width:300px ; height:auto ; display: flex; flex-direction: column; align-items: center;">

     <q-card-section class="q-pt-none full-width q-mt-md">
      <div class="text-h5">Esqueci minha senha</div>
      <p class='text-subtitle'>Informe seu email para recuperar senha</p>
     </q-card-section>

      <q-card-section class="q-pt-none full-width q-mt-md">
         <q-input filled v-model="email" label="E-mail" />

          <q-card-actions class="q-mt-md">
              <q-btn push color="secondary" label="Redefinir senha" style="flex:1" @click="$router.push({name:'login'})" />
          </q-card-actions>

      </q-card-section>
    </q-card>

    <q-card class="my-card">
      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class="absolute-bottom text-subtitle2 text-center">
          Title
        </div>
      </q-img>
    </q-card>
  </q-page>
</template>

<script>
export default {
  name: 'ForgotPassword',
  data () {
    return {
      email: ''
    }
  }
}
</script>
