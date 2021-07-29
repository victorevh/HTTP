## HTTP MESSAGES

# REQUEST / RESPONSE

# HTTP/1.1

* Legível
* Texto

# HTTP/2

* Estrutura binária
* Otimizações
* Mesma maneira que a versão 1.1

# REQUEST

O pedito é composto por

* Method (A intenção do pedido)
* Protocol Version (versão do protocolo)
* URI
* Body
* Headers 

Para verificar detalhes do pedido você pode usar a DevTools ou o Curl com o comando -v

# RESPONSE

Recebemos na mensagem de resposta por padrão

* Protocol Version
* Status code
* Headers
* Status Message

Para verificar os Headers da resposta você pode usar o comando -i no Curl