# gRPC
RPC (Remote Procedure Call)

## Definição
- É um framework desenvolvido pela google que tem o objetivo facilitar op processo de comunicação entre sistemas de uma forma extremamente rápida, leve, independente de linguagem.
- Faz parte da CNCF (Cloud Native Computing Foundation)

## Quais casos podemos utilizar
- Ideal para microsserviços
- Mobile, Browsers e Backend
- Geração das bibliotecas de forma automática
- Streaming bidirecional utilizando HTTP/2

## Linguagens (Suporte Oficial)
- gRPC-GO
- gRPC-JAVA
- gRPC-C
	* C++
	* Pyton
	* Ruby
	* Objective C
	* PHP
	* C#
	* Node.js
	* Dart
	* Kotlin
	
## Protocol Buffers vs JSON
- Arquivos binários < JSON	
- Processo de serialização é mais leve (CPU)  do que JSON
- Gasta menos recursos de rede
- Processo é mais veloz

## HTTP/2
- Nome original criado pela Google era SPDY
- Lançado em 2015
- Dados trafegados são binários e não texto como no HTTP 1.1
- Utiliza a mesma conexão TCP para enviar e receber dados do cliente e do servidor (Multiplex)
- Server Push
- Headers são comprimidos
- Gasta menos recursos de rede
- Processo é mais veloz

## Formatos de comunicação
- gRPC - API "unary"
- gRPC - API "Server streaming"
- gRPC - API "Client streaming"
- gRPC - API "Bi direcional streaming"

## REST vs gRPC
| REST | gRPC |
|---|---|
| Texto / JSON | Protocol Buffers |
| Unidirecional | Bidirecional e Assíncrono |
| Alta latência | Baixa latência |
| Sem contrato (maior chance de erros) | Contrato definido (.proto) |
| Sem suporte a streaming (Request / Response) | Suporte a streaming |
| Design pré-definido | Design é livre |
| Bibliotecas de terceiros | Geração de código |