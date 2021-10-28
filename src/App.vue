<template>
  <v-app>

    <v-app-bar
      app
      color=""
      light
    >
      <v-container>
        <div class="d-flex  align-center">
          <v-img
            alt="Vuetify Logo"
            class="shrink mr-2"
            contain
            src="./assets/logo.png"
            transition="scale-transition"
            width="32"
          />
          <v-btn text class="text-none">Home</v-btn>
          <v-btn text class="text-none">About</v-btn>
          <v-btn text class="text-none">Projects</v-btn>
          <v-btn text class="text-none">Contact</v-btn>
          <v-spacer/>
          <v-btn icon>
            <v-icon v-icon>mdi-account</v-icon>
          </v-btn>
        </div>
      </v-container>
    </v-app-bar>

    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>

<script>
export default {
  name: 'App',

  data: () => ({
    //
  })
}
</script>
<style lang="scss">
@import '@/assets/variables';

$brandColor: #0273d7;

</style>
