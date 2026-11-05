# Ficha4

## 2
## Terminal 1 – Servidor Express:

node server.js

## Terminal 2 – Aplicação React (Client):

npm run dev

## 3

O responsável pelo bloqueio é o browser, através da política CORS (Cross-Origin Resource Sharing).
Se o servidor não enviar o header Access-Control-Allow-Origin, o browser impede o React de aceder à resposta.
Sabemos que é o browser porque o pedido chega ao servidor, como podemos verificar no terminal do server.
O servidor responde, mas o browser não permite que o JavaScript leia a resposta.

## 4
Agora a aplicação React faz apenas 1 request ao abrir, para obter todas as cartas através da API.
Ao filtrar ou pesquisar, não são feitos novos requests, porque os dados já estão guardados no estado do React.
Os dados ficam guardados no estado cards do React, no browser.
O HTML é construído pelo React no lado do cliente (browser).
