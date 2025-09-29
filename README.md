⚠️ Análise dos Erros do Projeto CRUD JWT JSON

Este documento apresenta os pontos que não estão de acordo com o enunciado da tarefa e que precisam ser corrigidos.

1. Proteção da rota GET /users/:id

O enunciado determina que todas as rotas de /users sejam protegidas.
No código atual, a rota GET /users/:id não está protegida.

2. Campos do usuário

O enunciado pede que os usuários sejam cadastrados com os campos nome, email e senha.
No código atual, está sendo utilizado nome, idade e senha, o que não segue as instruções.

3. Login

A autenticação deve ser feita utilizando email e senha.
No código atual, o login foi implementado utilizando nome e senha, o que está em desacordo com o pedido.

4. IDs dos usuários

O enunciado sugere o uso de UUID para identificar os usuários de forma única.
No código atual, os IDs são numéricos incrementais (1, 2, 3...), o que pode causar conflitos e não segue a recomendação.

5. Retorno de dados sensíveis

As rotas de listagem e busca de usuários ainda retornam o campo senha.
Isso expõe informações sensíveis e fere boas práticas de segurança.