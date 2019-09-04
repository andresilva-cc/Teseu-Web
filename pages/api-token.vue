<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>vpn_key</v-icon>Token da API</span>
          </v-card-title>
          <v-card-text>
            <span>Digite seu endereço de e-mail abaixo para receber um token para consumo da API.</span>
            <v-form class="mt-3">
              <v-layout row wrap>
                <v-flex xs12 md6>
                  <v-text-field prepend-icon="email" label="E-mail"></v-text-field>
                </v-flex>
                <v-flex xs12 class="mt-3">
                  <v-btn color="blue" class="white--text"><v-icon left>send</v-icon>Enviar</v-btn>
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