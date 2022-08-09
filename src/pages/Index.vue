<template>
  <q-page class="bg-dark flex row">
    <div class="col-3">
      <AvatarApp />
      <ListPerfil />
    </div>

    <div class="col-6 q-pa-sm">
      <Publication :openModal='openModal' />
      <ModalApp :show="show" @closed='closeModal' />
    </div>

    <div class="col-3 bg-positive">Hello</div>
  </q-page>
</template>

<script>
import AvatarApp from '../components/Perfil/AvatarPerfil.vue'
import ListPerfil from '../components/Perfil/ListPerfil.vue'
import ModalApp from '../components/Modal/Index.vue'
import Publication from 'src/components/Publication/index.vue'

export default {
  name: 'PageIndex',
  components: { AvatarApp, ListPerfil, ModalApp, Publication },
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
