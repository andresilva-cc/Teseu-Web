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
                  <v-text-field 
                    v-model="email"
                    :rules="[rules.required, rules.email]"
                    prepend-icon="email"
                    label="E-mail" />
                </v-flex>

                <v-flex xs12 class="mt-3">
                  <v-btn
                    color="blue"
                    class="white--text"
                    :loading="loading"
                    :disabled="loading"
                    @click="submit">
                      <v-icon left>send</v-icon>
                      Enviar
                    </v-btn>
                </v-flex>

              </v-layout>
            </v-form>
          </v-card-text>

        </v-container>
      </v-card>

      <v-snackbar
        v-model="snackbar"
        color="green"
        bottom
        :timeout="3000"
      >
        O token foi enviado para seu e-mail.
      </v-snackbar>

    </v-flex>
  </v-layout>
</template>

<style scoped>
.v-card {
  height: 100%;
}
</style>

<script>
import axios from '~/plugins/axios'

export default {
  data () {
    return {
      email: '',
      loading: false,
      snackbar: false,

      rules: {
        required: value => !!value || 'Obrigatório.',
        email: value => {
          const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
          return pattern.test(value) || 'E-mail inválido.'
        }
      }
    }
  },

  methods: {
    async submit () {
      try {
        this.loading = true

        await axios.post('/auth/api/token', {
          email: this.email
        })

        this.snackbar = true

        this.loading = false
      } catch (ex) {
        this.loading = false
        throw ex
      }
    }
  }
}
</script>