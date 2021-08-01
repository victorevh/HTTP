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

## OPTIONS

Vai servir para dar informações sobre a disponibilidade da requisição (Quais metodos estão disponiveis para mim)

* no curl você pode usar (curl -X OPTIONS http://localhost:3000/post -i) para receber o cabeçalho e ver os Metodos permitidos de acesso

## GET

Serve para pegar um recurso / somente recebe dados
* curl -v ou --get

### Caracteristicas do GET

* Seguro: SIM (Não faz alteração no servidor)
* Idempotente: SIM (sempre que eu pedir a pagina vai ser entregue da mesma maneira)
* BODY
    * REQUEST: NÃO
    * RESPONSE: SIM
* Cacheable: SIM
* Uso em formulários HTML: SIM

no curl você pode usar o -v para obsevar informações do escopo desejado 

* curl http://localhost:3000/posts\ ?q \ =json    \ ?q \ =..... é um filtro de pesquisa.



## HEAD

Semelhante ao GET, porém recebemos somente o cabeçalho HEAD / posts

* para ver os cabeçalhos de resposta no curl -I ou --head

### Caracteristicas do HEAD

* Seguro: SIM (Não faz alteração no servidor)
* Idempotente: SIM (sempre que eu pedir a pagina vai ser entregue da mesma maneira)
* BODY
    * REQUEST: NÃO
    * RESPONSE: NÃO
* Cacheable: SIM
* Uso em formulários HTML: NÃO

## POST

Publicar / Cadastra um Recurso em algum lugar

* para enviar dados usar comando curl -d '{ dados aqui }' 
* -H é o cabecario EX:/ "Content-type: application/json" avisando que o conteudo que estou enviando é um json e por fim a rota com o -X POST http://localhost:3000/posts
* usar o comando cat no curl para visualizar o texto de determinado arquivo

### Caracteristicas do POST

* Seguro: NÃO (vai alterar algo no servidor)
* Idempotente: NÃO (cada vez que eu fazer a rota de cadastro ele faz retornos diferentes (por conta dos cadastros diferentes) )
* BODY
    * Request
    * Response
* Uso em formulários HTML: SIM (Posso cadastrar um usario no meu sistema usando esse metódo)
* Poderá ser cacheable

## PUT

A diferença entre o POST e o PUT é que o PUT é indepotente ()

Serve para criar um novo ou Atualizar um recurso (o uso definitivo do PUT é para atualizar um recurso)

* Criação Status code 201
* Atualização Status code 204 ou 401

* para enviar dados usar comando curl -d '{ dados aqui }' 
* -H é o cabecario EX:/ "Content-type: application/json" avisando que o conteudo que estou enviando é um json e por fim a rota com o -X PUT http://localhost:3000/profile

### Caracteristicas do PUT

* Seguro: NÃO (vai alterar algo no servidor)
* Idempotente: SIM (Sempre a resposta é a mesma)
* BODY
    * Request: SIM
    * Response: NÃO
* Uso em formulários HTML: NÃO
* Cacheable: NÃO