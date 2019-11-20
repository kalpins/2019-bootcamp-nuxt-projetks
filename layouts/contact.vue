<template>
  <v-app>
    <v-app-bar fixed app>
      <v-toolbar-title v-text="title" />
      <v-spacer />
      <v-toolbar-items>
        <v-btn text to="/">Sākums</v-btn>
        <v-btn text>Link 2</v-btn>
        <v-btn text to="/contact">Kontakti</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-content>
      <nuxt />
    </v-content>

    <v-footer>
      <span>Šis ir mans kontaktu lapas footeris, jo gribēju citu layout</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      title: "Mans RCS gala darbs"
    };
  }
};
</script>
