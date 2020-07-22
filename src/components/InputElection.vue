<template>
  <v-row>
    <v-col
      md="7"
      xg="9"
    >
      <v-row>
        <v-col md="12">
          <v-form
            ref="form"
            lazy-validation
          >
            <v-row>
              <v-col md="12">
                <p>Tipo de eleição</p>
                <v-radio-group
                  row
                  required
                >
                  <v-radio
                    label="Urna Prodam"
                    value="True"
                  >Urna Prodam</v-radio>
                  <v-radio
                    label="Online"
                    value="False"
                  >Online</v-radio>
                  <v-radio
                    label="Apuração"
                    value="True"
                  >Apuração</v-radio>
                </v-radio-group>
              </v-col>
            </v-row>
            <v-row>
              <v-col
                sm="12"
                md="6"
              >
                <v-text-field
                  ref="idTextField"
                  label="Quantidade de urnas"
                  required
                  maxlength="100"
                />
              </v-col>
            </v-row>
            <v-row>
              <v-col
                sm="12"
                md="6"
              >
                <v-text-field
                  label="Quantidade média de eleitores"
                  required
                  maxlength="100"
                />
              </v-col>
            </v-row>
            <v-row>
              <v-col
                sm="12"
                md="6"
              >
                <v-text-field
                  class="mr-4"
                  type="date"
                  label="Data de início eleição"
                  required
                />
              </v-col>
            </v-row>
            <v-row>
              <v-col
                sm="12"
                md="6"
              >
                <v-text-field
                  class="mr-4"
                  type="date"
                  label="Data de fim eleição"
                  required
                />
              </v-col>
            </v-row>
            
            <v-row class="add-btn">
              <v-col
                sm="8"
                md="3"
              >
                <v-btn
                  color="green"
                  tile
                  block
                >
                  Calcular
                </v-btn>
              </v-col>
            </v-row>
          </v-form>
        </v-col>
      </v-row>
    </v-col>
  </v-row>
</template>

<script>

export default {
  name: 'InputElection'
};
</script>s