<template>
  <v-container>
    <v-row>
      <v-col
        md="5"
        lg="4"
        xl="3"
      >
        <h1>
          Simulador de eleições
        </h1>
        <br>
        <div>
          <InputElection></InputElection>
        </div>
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
