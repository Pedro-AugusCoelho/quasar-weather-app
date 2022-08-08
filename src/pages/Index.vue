<template>
  <q-page class="bg-dark flex row">
    <div class="col-3">
      <AvatarApp />
      <ListPerfil />
    </div>

    <div class="col-5 q-pa-sm bg-accent">
      <q-card class="my-card">
        <q-item clickable v-ripple  @click='openModal'>
          <q-item-section avatar>
            <q-icon color="primary" name="description" />
          </q-item-section>
          <q-item-section class="text-h6">No que você está pensando</q-item-section>
        </q-item>
      </q-card>
      <ModalApp :show="show" @closed='closeModal' />
    </div>
    <div class="col-4 bg-positive"></div>
  </q-page>
</template>

<script>
import AvatarApp from '../components/Perfil/AvatarPerfil.vue'
import ListPerfil from '../components/Perfil/ListPerfil.vue'
import ModalApp from '../components/Modal/Index.vue'

export default {
  name: 'PageIndex',
  components: { AvatarApp, ListPerfil, ModalApp },
  data () {
    return {
      text: '',
      show: false
    }
  },
  methods: {
    openModal () {
      this.show = true
    },
    closeModal () {
      this.show = false
    }
  }
}
</script>
