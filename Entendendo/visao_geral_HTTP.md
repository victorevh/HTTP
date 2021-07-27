# HyperText Transfer Protocol 

Protocolo de Transferência do HyperTexto


## Visão Geral

  * Permite troca de informações e dados na internet
  * Uma troca de mensagens
  * HTML, CSS, Scripts, Imagens, Vídeo
  * Uma chamada para cada um desses recursos

## Como ocorre a troca de mensagens

O Browser faz um Request (pedido) para o servidor que efetua uma Response (Resposta), com isso temos um fluxo de mensagens.

* As Mensagens podem ser divididas em três tipos

  * Pedido (Request)
  * Resposta (Response)
  * Request/Response

## Pedido (Request)

Quando começamos um pedido, precisamos entender qual ação vamos executar que são os Metodos

* GET (Pegar um Recurso) (Acessar um endereço)
* POST (Criar um Recurso) (Postar algo na internet)

## Resposta (Response)

A Resposta do pedido é feita em ordem

* 1º Status code: 

Resposta do servidor sobre o estado do pedido/resposta.

Exemplo:
200: a solicitação foi respondida com sucesso
301: pedido de redirecionamento
404: o servidor não encontra a pagina
500: erro interno do servidor

## Request/Response

* Exemplos de Request Message e Response Message

  * REQUEST MESSAGE

    * GET/index.html HTTP/1.1
    * User-Agent: Mozilla/4.0
    * Accept: text/html

  * RESPONSE MESSAGE

    * HTTP/1.1 200 OK
    * Server: Express
    * Content-Type: text/html

      <html>....</html>

* Headers 
  
    São campos informativos, do tipo propriedade: valor propety/value

    * Exemplo 
        
         * Contenty-Type: application/json 
         * User-Agent: Chrome
         * Request URL: www.google.com

* Body

    Posso estar enviando e recebendo ao mesmo tempo, enviando um JSON e recebendo HTML ao mesmo tempo.