## URI

* Uniform Resource Identifier

* Conceito

É um identificador de recursos que trabalha de forma unica. A exemplo da minha pessoa, eu sou um recurso, onde tenho meu nome e minha localização, então se preciso me achar (recurso) tenho que saber desses itens.

# Resource

* O que é o Recurso?

É o Alvo do pedido Ex:. https://www.google.com

Se podemos identificar, nomear, endereçar ou manipular, estamos falando de um recurso.

* Esse recurso pode ser qualquer coisa identificável ou entidade
* Entidade Digital (acessar o Email através to protocolo mailto:email@dominio.com)
* Entidade Abstrata (Para iniciar uma sessão no google por exemplo, precisamos passar pelo processo de autenticação, tudo isso são endereços locais que precisamos chegar)
* Entidade Fisica (Produtos, Usuarios)


# Locator

* O que é o Localizador?

É por onde podemos procurar o recurso usando a URL (endereço)

* URL (Uniform Resource Locator)

A URL trabalha com componentes, são eles obrigatórios e opcionais

* Obrigatorios
   * Protocolos (https://, http://, mailto:)
   * Dominios google.com
Dominios podem ser escritos em forma de ip 

* Protocolo + dominio = URL

* Opcionais (Fazem a diferença para encontrar determinado recurso)
   * Subdonínio (O que vem antes do Domnínio)
   * Path (Exemplo www....com.br/blog)
   * Parametros (Não consigo chegar a determinado video do youtube se o parametro dele não estiver inserido na url (?v=vpYct2npKD8))
   * Porta (Exemplo http://127.0.0.1:3333/index.html) a porta é :3333
      * Quando utilizo o http:// sem inserir a porta, implicitamente atribuo a porta :80 ao dominio
      * Quando utilizo o https:// implicitamente eu tenho a porta :443
   * Âncora (quando tenho uma ancora # tenho um local dentro do documento. exemplo: wwww.ok.com.br/index.html#algumlugar)

# Name

é quando encontro o recurso pelo nome, mas não pelo local (não sei onde está o recurso)

* URN (Uniform Resource Name)

Exemplos: urn:isbn:044534233242 sabemos que existe um livro com esse isbn mas não sabemos onde ele está, mas sabemos que a identificação do mesmo é essa.