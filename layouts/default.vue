<template>
  <v-app class="app">
    <div class="d-flex wrapper">
      <v-navigation-drawer
        v-model="drawer"
        :mini-variant="miniVariant"
        permanent
        class="pa-3"
      >
        <v-list-item class="mb-10" color="#245EE7">
          <v-list-item-content>
            <v-list-item-title class="text-h6">Analize. </v-list-item-title>
            <v-list-item-subtitle> Analytics Platform </v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <div class="mb-3">Main Menu</div>
        <v-list>
          <v-list-item
            v-for="(item, i) in items"
            :key="i"
            :to="item.to"
            router
            exact
          >
            <v-list-item-action>
              <v-icon>{{ item.icon }}</v-icon>
            </v-list-item-action>
            <v-list-item-content>
              <v-list-item-title v-text="item.title" />
            </v-list-item-content>
          </v-list-item>
        </v-list>
        <v-divider></v-divider>
        <div class="mt-10">SUPPORT</div>
        <v-list-item
          v-for="(item, i) in support"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-navigation-drawer>
      <v-main>
        <v-container fluid>
          <Nuxt />
        </v-container>
      </v-main>
    </div>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data() {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Dashboard',
          to: '/',
        },
        {
          icon: 'mdi-account-multiple',
          title: 'Customers',
          to: '/inspire',
        },
      ],
      support: [
        {
          icon: 'mdi-message',
          title: 'Message',
          to: '/message',
        },
        {
          icon: 'mdi-phone',
          title: 'Help',
          to: '/help',
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js',
    }
  },
}
</script>

<style scoped>
.app {
  flex-direction: row !important;
}

.wrapper {
  min-height: 100vh;
}
</style>
