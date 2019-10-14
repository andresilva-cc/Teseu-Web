<template>
  <v-layout justify-center fill-height>
    <v-flex xs12>
      <v-card>
        <v-container>
          <v-card-title>
            <span class="headline"><v-icon medium left>description</v-icon>Termos de Uso</span>
          </v-card-title>
          <v-card-text>
            <p>Estes Termos de Uso regem seus direitos e obrigações referentes ao uso do aplicativo Teseu. Estes termos constituem um contrato totalmente vinculativo entre a aplicação Teseu e você. Portanto, é recomendável que você leia atentamente estes termos.</p>
  
            <p>Ao utilizar o aplicativo Teseu, você concorda com este referido termo e a Política de Privacidade. Se você não concorda com estes termos ou qualquer de suas partes, então você está proibido e deve abster-se de usar este aplicativo. Se você infringir estes termos ou qualquer de suas partes, sua conta estará sujeita a suspensão e exclusão, e caso necessário, processos judiciais.</p>

            <p>Os termos de uso são definidos a seguir:</p>

            <ol>
              <li><b>Compartilhamento de conta:</b> a sua conta de usuário é de uso exclusivo por você e não deve ser compartilhada com nenhuma outra pessoa.</li>
              <li><b>Segurança do usuário:</b> nós não encorajamos você em nenhum momento a visitar áreas perigosas reportadas pelos outros usuários. Nossa principal preocupação é sua segurança, por isso ao receber uma notificação de uma área perigosa, evite a mesma.</li>
              <li><b>Mal-uso das ocorrências:</b> em nenhum momento você deve registrar ocorrências baseadas em atividades meramente suspeitas ou baseadas somente em características físicas de um indivíduo, como por exemplo a cor da pele e vestimentas.</li>
              <li><b>Vigilantismo:</b> qualquer tipo de vigilantismo ou autojustiça é expressamente proibida. A proposta da aplicação é notificar ocorrências criminais, enquanto o trabalho de investigação, julgamento e aplicação de penas é de responsabilidade dos devidos órgãos.</li>
              <li><b>Conexão de internet:</b> é necessária uma conexão com a internet para utilizar este aplicativo, e quaisquer cobranças associadas incorridas pelo seu uso do serviço, são de sua exclusiva responsabilidade e feitas exclusivamente por sua conta.</li>
              <li><b>Idade:</b> este aplicativo é destinado ao uso por usuários que tenham atingido a maioridade, no caso do Brasil, 18 anos.</li>
            </ol>

            <div class="title mt-5 mb-4">Política de Privacidade</div>

            <p>A aplicação Teseu respeita sua privacidade. Oferecemos serviços baseados em comunidade, localização e push notifications. Ao utilizar nossos serviços, você confia suas informações a nós. Esta política de privacidade é incorporada como parte dos Termos de Uso do Teseu. Seu uso dos serviços está sujeito aos Termos de Uso e a esta Política de Privacidade e implica na aceitação desses documentos. A política de privacidade é detalhada abaixo:</p>

            <ol>
              <li>Ao registrar sua conta, armazenamos em nosso banco de dados o seu nome de usuário e seu número de telefone celular.
                <ol type="a">
                  <li>A autenticação é realizada através de código de confirmação via SMS, portanto, somente quem tem acesso a seu número de telefone celular (você mesmo) pode utilizar sua conta.</li>
                  <li>O seu número de telefone nunca é mostrado a nenhum outro usuário, apenas o seu nome de usuário.</li>
                  <li>É recomendado que você utilize um nome de usuário fictício para não expor sua identidade.
                    <ol type="i">
                      <li>Para sua conveniência, ao cadastrar sua conta, o aplicativo irá gerar um nome de usuário aleatório para você utilizar.</li>
                    </ol>
                  </li>
                  <li>Caso você deseja desativar sua conta, entre em contato com o suporte.</li>
                </ol>
              </li>
              <li>Para utilizar a funcionalidade de notificações em tempo real com base em sua localização, precisamos do acesso aos serviços de localização do seu dispositivo, os quais serão solicitados na primeira inicialização do aplicativo.
                <ol type="a">
                  <li>A sua localização será enviada ao servidor de tempo em tempo, porém não será armazenada em nosso banco de dados, servindo apenas para obter as ocorrências próximas de sua localização.</li>
                  <li>A sua localização não é compartilhada com nenhum usuário ou terceiro.</li>
                  <li>Caso você queira desativar esta funcionalidade, desative os alertas nas configurações do aplicativo.</li>
                </ol>
              </li>
              <li>Para utilizar a funcionalidade de locais de interesse, você concorda em compartilhar conosco o nome e localização do seu local, os quais serão armazenados em nosso banco de dados.
                <ol type="a">
                  <li>Nenhum usuário ou terceiro terá acesso aos seus locais de interesse.</li>
                  <li>Caso você queira desativar esta funcionalidade, remova todos os seus locais de interesse nas configurações do aplicativo.</li>
                </ol>
              </li>
              <li>Para utilizar a funcionalidade de contatos de confiança, você concorda em compartilhar conosco o nome e número de telefone celular de seu contato, os quais serão armazenados em nosso banco de dados.
                <ol type="a">
                  <li>O aplicativo necessita de acesso à sua lista de contatos (agenda) para importar os contatos desejados.</li>
                  <li>Nenhum usuário ou terceiro terá acesso aos seus contatos de confiança.</li>
                  <li>Ao adicionar um novo contato de confiança, o seu contato será avisado por SMS, e caso ele queira, poderá cancelar esta ação.</li>
                  <li>Caso você queira desativar esta funcionalidade, remova todos os seus contatos de confiança nas configurações do aplicativo.</li>
                </ol>
              </li>
              <li>Ao cadastrar uma ocorrência, você concorda em compartilhar conosco os dados de sua ocorrência, além da sua localização ou localização informada durante o cadastro. Todas estas informações serão armazenadas em nosso banco de dados.
                <ol type="a">
                  <li>Os usuários do aplicativo próximos a sua localização terão acesso a estas informações enquanto a ocorrência estiver visível. Seu número de telefone celular não será visível para os outros usuários (apenas o seu nome de usuário)</li>
                  <li>Terceiros poderão ter acesso a estas informações através de nossa API pública ou através da exportação de arquivos CSV, porém sua identidade não será revelada, apenas os dados da ocorrência (incluindo a localização).</li>
                </ol>
              </li>
              <li>Toda conexão que você faz no aplicativo é registrada, armazenando no banco de dados a data/hora de conexão e seu endereço IP.</li>
              <li>Todas a comunicação entre o aplicativo e o servidor é feita através de uma conexão segura (HTTPS), isto significa que os dados não podem ser visualizados por terceiros, ainda que ocorra interceptação da conexão.</li>
            </ol>
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

  p {
    text-indent: 30px;
  }

  ol {
    margin-left: 25px;
    margin-top: 5px;
  }

  li {
    margin-bottom: 10px;
  }
</style>