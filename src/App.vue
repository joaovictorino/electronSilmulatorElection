<template>
  <v-app>
    <v-main>
      <CalculateElection/>
    </v-main>
  </v-app>
</template>

<script>
import CalculateElection from './pages/CalculateElection';

export default {
  name: 'App',

  components: {
    CalculateElection,
  },

  data: () => ({
    //
  }),
};
</script>
