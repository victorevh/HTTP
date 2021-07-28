# Conceitos HTTP

## O HTTP foi feito pra ser simples e legivel para qualquer pessoa

* Cliente / Servidor : Requisição / Resposta

* Stateless
   * Não guarda informações (Estado)
   * Não existe relação entre conexões
   * É como jogar uma moeda pro ar, as vezes pode ser cara, ou coroa

* Sessões (Loguin e senha, podem ser armazendos em)
    * Cookies
    * Storages

* É extensível porque através do cabeçalho, podemos fazer diversas trocas de informações entre o cliente-servidor, conforme a necessidade.
    * Headers: informações para a comunicação
    * Body: corpo do pedido ou da resposta

## Cliente

* Quem é o cliente? 

É o User Agent, que na maioria das vezes é o Browser, no caso do meu estudo o cliente é o cURL

* User Agent
   * Browser
   * cURL

* Quais são os pedidos realizados pelo Cliente?

O Pedido do cliente é intreseco a ação que o mesmo quer tomar

* Ações do Cliente
   * GET        (Pedir dados)
   * POST       (Enviar dados)
   * PUT        (Atualizar dados)
   * DELETE     (Deletar dados)

## Servidor

* Quem é o servidor?

O servidor se apresenta como uma máquina no mundo que está preparada para ouvir e processar. Podem existir varios servidores em um computador, e varios computadores para um servidor.

* Ações do servidor (Resposta)
   * headers 
      * Status code
         * 404
         * 500
    * Body
        * Corpo da resposta


## Proxies

* Quem são os Proxies? 

Podemos entender os Proxies como representantes que ficam entre o cliente e o servidor, e ajudam a fazer o transporte dos dados (Roteadores, switch).

* Funções do Proxies
   * Cache 
   * Filtro (tipo um antivírus, ou controle parental)
   * Load balancing (distribuição da carga) 
   * Autenticação
   * Autorização