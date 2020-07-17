<template>
  <v-container>
    <v-app-bar color="indigo">
      <v-toolbar-title class="white--text">
        {{ title }}
      </v-toolbar-title>
    </v-app-bar>

    <v-form class="pt-11">
      <v-system-bar>
        Dane osobowe
      </v-system-bar>
      <v-combobox label="Imię i nazwisko"> </v-combobox>
      <v-text-field label="Dział"> </v-text-field>
      <v-text-field label="Stanowisko"> </v-text-field>
      <v-system-bar>
        Informacje o szkoleniu 
      </v-system-bar>

      <v-text-field label="Nazwa"> </v-text-field>
      <v-text-field label="Lokalizacja"> </v-text-field>
      <v-text-field label="Cena" type="number"> </v-text-field>

      <v-row>
        <v-date-picker color="indigo"> </v-date-picker>
        <v-date-picker color="indigo"> </v-date-picker>
      </v-row>
      <v-textarea label="Uzasadnienie"> </v-textarea>
      <v-btn color="indigo">Wyślij </v-btn>
    </v-form>
  </v-container>
</template>

<script>
import Vue from "vue";
export default Vue.extend({
  name: "SubmissionForm",

  data: () => ({
    title: "Wniosek o dofinansowanie do szkolenia",
  }),
});
</script>
