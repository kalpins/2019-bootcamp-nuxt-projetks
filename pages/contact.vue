<template>
  <v-container>
    <v-row>
      <v-col>
        <h1 class="display-3 mb-4">Saziņa ar mums</h1>
        <p>
          Nam fringilla enim vitae neque pharetra, vel faucibus magna euismod.
          Proin turpis eros, dictum ut cursus eget, dignissim euismod lectus.
          Donec consectetur tellus elit, vel semper tortor tempus eu. Quisque
          pretium lectus ut nisi porta, non pharetra tellus imperdiet. Praesent
          placerat massa eget accumsan venenatis. Cras mattis, dui eget mollis
          tincidunt, neque odio scelerisque libero, ac accumsan tellus sapien
          eget felis. Nunc consequat, sapien eget convallis efficitur, erat urna
          commodo orci, ut imperdiet velit ipsum quis augue. Donec dignissim
          erat sed mollis interdum. Duis pharetra, nunc eget maximus ultricies,
          eros neque interdum odio, ullamcorper egestas quam libero sit amet
          sem. Suspendisse id lorem nisl. Phasellus ultricies neque eget enim
          tristique euismod. Pellentesque pharetra urna eu hendrerit consequat.
        </p>
        <p>
          Etiam eros nisl, fermentum sit amet diam ac, mattis vehicula massa.
          Suspendisse aliquet turpis nisl, sit amet rutrum tortor vestibulum ut.
          Morbi venenatis sodales suscipit. Praesent elementum mauris arcu, ut
          mattis eros bibendum eget. Nunc sit amet sodales risus. Integer
          condimentum dolor at leo interdum, eu hendrerit arcu maximus.
          Phasellus posuere turpis elit. Class aptent taciti sociosqu ad litora
          torquent per conubia nostra, per inceptos himenaeos. Aenean faucibus
          sagittis ullamcorper. Pellentesque vestibulum massa pellentesque nunc
          maximus vestibulum. Aliquam tortor ipsum, molestie sit amet venenatis
          egestas, fringilla in justo. Quisque nunc mauris, venenatis id sapien
          a, auctor volutpat ipsum.
        </p>
      </v-col>
    </v-row>
    <Contact :title="nosaukums"></Contact>
    <v-row>
      <v-col cols="12">
        <iframe
          width="100%"
          height="400"
          src="https://www.youtube.com/embed/Nh9VEkesWfc"
          frameborder="0"
          allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        ></iframe>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import Contact from "~/components/Contact.vue";
export default {
  layout: "contact",
  components: {
    Contact
  },
  data: () => ({
    nosaukums: "From contact page"
  })
};
</script>

<style></style>
