<template>
  <div>
    <v-row>
      <v-col>
        <p>Tipo de eleição</p>
        <v-radio-group
          row
          v-model="typeElection"
        >
          <v-radio
            label="Urna Prodam"
            value="A"
          >Urna Prodam</v-radio>
          <v-radio
            label="Online"
            value="B"
          >Online</v-radio>
          <v-radio
            label="Apuração"
            value="C"
          >Apuração</v-radio>
        </v-radio-group>
      </v-col>
    </v-row>
    <v-row>
      <v-col
        md="12"
        lg="10"
        xl="8"
      >
        <v-text-field
          label="Qtde urnas"
          required
          maxlength="20"
        />
      </v-col>
    </v-row>
    <v-row v-show="expand">
      <v-col
        md="12"
        lg="10"
        xl="8"
      >
        <v-text-field
          label="Qtde eleitores"
          required
          maxlength="20"
        />
      </v-col>
    </v-row>
    <v-row class="add-btn">
      <v-col
        sm="8"
        md="3"
      >
        <v-btn
          tile
          block
          @click="simulate"
        >
          Simular
        </v-btn>
      </v-col>
    </v-row>
  </div>
</template>

<style scoped>
.center {
  width: 50%;
  margin: auto;
}
</style>

<script>
export default {
  name: 'InputElection',
  
  data: () => ({
    expand: false,
    typeElection: ''
  }),
  watch: {
    typeElection: function(val){
      if(val === 'A') {
        this.expand = true
      } else {
        this.expand = false
      }
    }
  },
  methods: {
    simulate: function() {
      alert('teste')
    }
  } 
};
</script>
