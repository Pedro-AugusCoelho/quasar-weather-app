<template>
    <div class="q-pa-md">
          <q-list>
             <q-item clickable v-ripple>
              <q-item-section avatar  class="gt-sm">
                <q-icon color="white" name="group" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Amigos</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="diversity_3" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Grupos</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="store" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Marketplace</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="campaign" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6 text-white">Central de anúncios</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="videogame_asset" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Jogos</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="live_tv" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Watch</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="person" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Minha conta</q-item-label>
              </q-item-section>
            </q-item>

            <q-item clickable v-ripple>
              <q-item-section avatar class="gt-sm">
                <q-icon color="white" name="settings" />
              </q-item-section>

              <q-item-section>
                <q-item-label class="text-h6  text-white">Configurações</q-item-label>
              </q-item-section>
            </q-item>

          </q-list>
      </div>
</template>

<script>
export default {
  name: 'ListPerfil'
}
</script>
