# JSON Server

https://github.com/typicode/json-server

instalar json-server através do Curl: npm install -g json-server  (-g instala de uma maneira global na maquina)

* mkdir (cria novo diretorio)
* cd (entrar no diretorio)
* vim db.json (criar json dentro do diretorio e colar o script conforme o tutorial do git. esc + :wp +enter)
* json-server --watch db.json (para iniciar o JSON server)



# METHODS

* OPTIONS
* GET
* HEAD
* POST
* PUT
* PATCH
* DELETE

## HTTP Methods

* Define um conjunto de métodos HTTP
* Indica a ação que o cliente deseja operar
* Podem ser chamados de Verbos HTTP
* Cada um possui a sua semântica
* Características
  
  * Seguro  (Somente leitura)
     * Não altera o estado do servidor
     * Somente leitura
     * Cliente não solicita alterações
     * Não há carga extra para o servidor
     * O servidor é responsável em manter o método seguro
     * Quais são os métodos?
         * GET
         * HEAD
         * OPTIONS
  
  * Idempotente
     * Ao executar o método, a resposta deverá ser sempre a mesma
     * Quais são?
         * Todos os seguros são idempotentes
         * PUT
         * DELETE

     * Status code poderá ser diferente
     * O servidor tem a responsabilidade de retornar dados da mesma maneira
     * Essa especificação não é garantia de que todos os servidores irão aplicar o conceito corretamente (mas deveria)

HTTP METHOD

* GET: IDEMPOTENCE/SAFETY
* HEAD: IDEMPOTENCE/SAFETY
* PUT: IDEMPOTENCE
* DELETE: IDEMPOTENCE
* POST: NO
* PATCH: NO
