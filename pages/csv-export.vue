<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>archive</v-icon>Exportação de CSV</span>
          </v-card-title>
          <v-card-text>
            <span>Utilize esta função para exportar as ocorrências em formato CSV. Você pode filtrar as ocorrências pela data inicial e data final.</span>
            <v-form class="mt-3">
              <v-layout row wrap>
                <v-flex xs12 md6 lg3>
                  <v-text-field prepend-icon="event" label="Data inicial"></v-text-field>
                </v-flex>
                <v-flex xs12 md6 lg3>
                  <v-text-field prepend-icon="event" label="Data final"></v-text-field>
                </v-flex>
                <v-flex xs12 class="mt-3">
                  <v-btn color="blue" class="white--text"><v-icon left>save_alt</v-icon>Exportar</v-btn>
                </v-flex>
              </v-layout>
            </v-form>
          </v-card-text>
        </v-container>
      </v-card>
    </v-flex>
  </v-layout>
</template>

<style scoped>
  .v-card {
    height: 100%;
  }
</style>