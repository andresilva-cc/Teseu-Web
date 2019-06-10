<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>map</v-icon>Mapa</span>
          </v-card-title>
          <v-card-text>
            <v-form>
              <v-layout row wrap>
                <v-flex xs12 md6>
                  <v-text-field append-icon="search" label="Pesquisar..."></v-text-field>
                </v-flex>
              </v-layout>
            </v-form>
            <v-layout row wrap class="mt-3">
              <v-flex xs12>
                <img src="/map.jpg">
              </v-flex>
            </v-layout>
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

  img {
    width: 100%;
  }
</style>