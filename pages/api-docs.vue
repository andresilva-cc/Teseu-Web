<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>widgets</v-icon>Documentação da API</span>
          </v-card-title>
          <v-card-text>
            <p>A API pública do Teseu permite que você consuma os dados do aplicativo, incluindo os dados gerados pelos usuários. Você pode consumir as ocorrências, categorias e exportar os dados no formato CSV*.</p>
            
            <div class="title pt-4 pb-3">URL Base</div>
            <p>Todos os <i>endpoints</i> referenciados nesta documentação possuem a seguinte URL base:</p>
            <code>https://api.teseu.app/</code>
            
            <div class="title pt-5 pb-3">Identificação</div>
            <p>Em cada <i>request</i> à API, você deve incluir o <i>header</i> <code>User-Agent</code> com o seu nome e seu e-mail, ou o nome de sua aplicação e o e-mail de contato. Como por exemplo:</p>
            <code>User-Agent: João Silva (joao.silva@email.com)</code>
            
            <div class="title pt-5 pb-3">Autorização</div>
            <p>Para ter acesso à API, você deve possuir um <i>token</i> de autorização, o qual pode ser solicitado na página <b><nuxt-link to="/api-token">Token da API</nuxt-link></b>. Em cada <i>request</i> à API, você deve incluir o <i>header</i> <code>Authorization</code>, onde seu valor deve ser composto de <code>Bearer</code> + espaço + <i>token</i>, como por exemplo:</p>
            <code>Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJlbWFpbCI6ImV4YW1wbGVAZXhhbXBsZS5jb20ifQ.NszkdPsAJIKOYrt9cNGBsvFRevkCS64Xxo_zRI4C0K4</code>

            <div class="title pt-5 pb-3">Formato de dados</div>
            <p>Todos os dados são enviados e recebidos em JSON (<i>JavaScript Object Notation</i>). Isto significa que você deve enviar o <i>header</i> <code>Content-Type: application/json</code> quando realizando requisições POST, PUT ou PATCH.</p>

            <div class="title pt-5 pb-3">Rotas</div>
            <p>Atualmente estão disponíveis 3 rotas para serem consumidas:</p>
            <ul>
              <li><code>/occurrences</code></li>
              <li><code>/occurrences/{id}</code></li>
              <li><code>/category</code></li>
            </ul>

            <div class="subheading pt-5 pb-3"><code>/occurrences</code></div>
            <p>Esta rota retorna todas ocorrências cadastradas.</p>
            

            <div class="subheading pt-3 pb-3"><code>/occurrences/{id}</code></div>
            <p>Esta rota retorna os detalhes da ocorrência com o <code>id</code> específicado.</p>

            <div class="subheading pt-3 pb-3"><code>/category</code></div>
            <p>Esta rota retorna todas as categorias de ocorrências.</p>

            <hr class="mt-5 mb-3">

            <div class="caption mb-3">* Em breve</div>

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

  a {
    text-decoration: none;
  }
</style>