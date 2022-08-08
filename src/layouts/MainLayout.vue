<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-btn
          flat
          dense
          round
          icon="menu"
          aria-label="Menu"
          @click="leftDrawerOpen = !leftDrawerOpen"
        />

        <q-toolbar-title>
          Facebook
        </q-toolbar-title>
      </q-toolbar>
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      show-if-above
      bordered
      content-class="bg-dark"
    >
      <q-list>
        <q-item-label header class="text-grey-8 text-h6">
          Menu
        </q-item-label>
        <q-item clickable @click="$router.push({name:'login'})">

            <q-item-section avatar>
              <q-icon name='exit_to_app' color="white" size="25px" />
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-weight-bold text-white">Logout</q-item-label>
            </q-item-section>

        </q-item>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

export default {
  name: 'MainLayout',
  data () {
    return {
      leftDrawerOpen: false
    }
  }
}
</script>
