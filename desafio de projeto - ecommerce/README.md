## Desfio de Projeto - Ecommerce

### Descrição do Desafio

O desafio de projeto E-commerce consiste na modelagem e refinamento de um esquema de banco de dados para E-commerce, tendo em sua composição pedido, produto, cliente, fornecedor, parceiro, entrega, estoque, pagamento.

O esquema deverá ser adicionado a um repositório do Github para futura avaliação do desafio de projeto. Adicione ao Readme a descrição do projeto conceitual para fornecer o contexto sobre seu esquema.

### Objetivo:
Refine o modelo apresentado acrescentando os seguintes pontos:

- Cliente PJ e PF – Uma conta pode ser PJ ou PF, mas não pode ter as duas informações;
- Pagamento – Pode ter cadastrado mais de uma forma de pagamento;
- Entrega – Possui status e código de rastreio;

Agora é a sua vez de ser o protagonista! Implemente o desafio sugerido pela expert e suba seu projeto para um repositório próprio, com isso, você aumentará ainda mais seu portfólio de projetos no GitHub!

### Resultado de refinamento:
Para a modelagem deste desafio, usei o banco de dados Postgres instalado via docker, também usei o adminer como ferramenta de visualização e manipulação do banco de dados

Para o refinamento de cliente, mantive a tabela cliente e fiz a generalização e especialização do cliente pf e cliente pj.

Para o refinamento da entrega, criei a tabela entrega, vinculada à tabela transportadora. Criei também a tabela entrega_movimento para registrar as movimentações da entrega do produto.

Para o refinamento do sistema de pagamento, crie a tabela pagamento, contendo diversos tipos de pagamento e, para a definição do tipo de pagamento, criei uma tabela intermediária chamada forma_pagamento.