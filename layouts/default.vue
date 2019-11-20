<template>
  <v-app>
    <v-app-bar fixed app class="title">
      <v-toolbar-title class="appbar--text" v-text="title" />
      <v-spacer />
      <v-toolbar-items>
        <v-btn text to="/">Sākums</v-btn>
        <v-btn text to="/posts">Posts</v-btn>
        <v-btn text to="/contact">Kontakti</v-btn>
      </v-toolbar-items>
    </v-app-bar>
    <v-content>
      <nuxt />
    </v-content>

    <v-footer>
      <span>&copy; 2019</span>
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
