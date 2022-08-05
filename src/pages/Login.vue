<template>
  <q-page class="flex flex-center bg-secondary" >
    <q-card class="" style="width:300px ; height:auto ; display: flex; flex-direction: column; align-items: center;">
      <q-card-section>
        <img src="https://cdn.quasar.dev/img/mountains.jpg" ratio='1' width="250px"/>
      </q-card-section>

      <q-card-section class="q-pt-none full-width">
         <q-input filled v-model="login.text" label="E-mail" />
         <q-input class="q-mt-sm" v-model="login.password" filled :type="login.isPwd ? 'password' : 'text' " label="Password">
            <template v-slot:append>
              <q-icon
                :name="login.isPwd ? 'visibility_off' : 'visibility'"
                class="cursor-pointer"
                @click="login.isPwd = !login.isPwd"
              />
            </template>
          </q-input>

          <q-card-actions>
              <q-btn flat color="secondary" label="Login" style="flex:1" @click="$router.push({name:'home'})" />
              <q-btn push color="secondary" label="Cadastro" style="flex:1" />
              <q-btn no-caps class="full-width q-mt-md" flat color="secondary" label="Esqueci minha senha"  @click="$router.push({name:'forgotmypassword'})" />
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
  name: 'Login',
  data () {
    return {
      login: {
        text: '',
        password: '',
        isPwd: true
      }
    }
  }
}
</script>
