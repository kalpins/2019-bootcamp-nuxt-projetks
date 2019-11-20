<template>
  <section>
    <v-row>
      <v-col cols="12" sm="6" md="8">
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1293.347517160314!2d24.103184307158827!3d56.96349008977174!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46eecfd2a9833f4b%3A0xda8c700119466379!2sDarbaVieta!5e0!3m2!1slv!2slv!4v1573837291571!5m2!1slv!2slv"
          width="100%"
          height="450"
          frameborder="0"
          style="border:0;"
          allowfullscreen
        ></iframe>
      </v-col>
      <v-col cols="12" sm="6" md="4">
        {{ title }}
        <v-form>
          <v-text-field
            name="name"
            prepend-inner-icon="mdi-account"
            required
            label="Vārds"
            id="id"
          ></v-text-field>
          <v-text-field
            type="email"
            prepend-inner-icon="mdi-email"
            required
            label="E-pasts"
          ></v-text-field>
          <v-select :items="items" label="Tēma"></v-select>
          <v-textarea
            name="question"
            label="Jautājums"
            hint="Hint text"
          ></v-textarea>
          <v-btn block color="primary" dark>
            Nosūtīt
            <v-icon>mdi-send</v-icon>
          </v-btn>
        </v-form>
      </v-col>
    </v-row>
  </section>
</template>

<script>
export default {
  props: {
    title: { defaul: "" }
  },
  data: () => ({
    items: ["Projekts", "Informācija", "Cits"]
  })
};
</script>

<style></style>
