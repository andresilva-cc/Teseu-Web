<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>widgets</v-icon>Documentação da API</span>
          </v-card-title>
          <v-card-text>
            <p>A API pública do Teseu permite que você consuma os dados do aplicativo, incluindo os dados gerados pelos usuários. Você pode consumir as ocorrências, categorias e exportar os dados no formato CSV.</p>
            <div class="title pt-4 pb-3">URL Base</div>
            <p>Todos os <i>endpoints</i> referenciados nesta documentação possuem a seguinte URL base:</p>
            <code>https://api.teseu.app/</code>
            <div class="title pt-5 pb-3">Identificação</div>
            <p>Em cada <i>request</i> à API, você deve incluir o <i>header</i> <code>User-Agent</code> com o seu nome e seu e-mail, ou o nome de sua aplicação e o e-mail de contato. Como por exemplo:</p>
            <code>User-Agent: João Silva (joao.silva@email.com)</code>
            <div class="title pt-5 pb-3">Formato de dados</div>
            <p>Todos os dados são enviados e recebidos em JSON (<i>JavaScript Object Notation</i>). Isto significa que você deve enviar o <i>header</i> <code>Content-Type: application/json</code> quando realizando requisições POST, PUT ou PATCH.</p>
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