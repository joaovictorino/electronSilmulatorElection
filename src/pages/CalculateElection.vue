<template>
  <v-container>
    <v-row class="text-center">
      <v-col class="mb-4">
        <h1 class="display-2 font-weight-bold mb-3">
          Simulador de eleições
        </h1>
        <InputElection></InputElection>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import InputElection from '@/components/InputElection';

export default {
  name: 'CalculateElection',

  components: {
    InputElection,
  },

  data: () => ({
    //
  }),
};
</script>
