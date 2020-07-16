<template>
  <v-app>
    <v-content>
      <SubmissionForm />
    </v-content>
  </v-app>
</template>

<script>
import SubmissionForm from "./components/SubmissionForm";

export default {
  name: "App",

  components: {
    SubmissionForm,
  },

  data: () => ({
    //
  }),
};
</script>
