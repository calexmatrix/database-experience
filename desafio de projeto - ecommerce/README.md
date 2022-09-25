## Desfio de Projeto - Ecommerce

O desafio de projeto E-commerce consiste na modelagem e refinamento de um esquema de banco de dados para E-commerce, tendo em sua composição pedido, produto, cliente, fornecedor, parceiro, entrega, estoque, pagamento.

Como desafio, foi solicitado os refinamento das entidades de cliente, pagamento e entrega.

Para a modelagem deste desafio, usei o banco de dados Postgres instalado via docker, também usei o adminer como ferramenta de visualização e manipulação do banco de dados

Para o refinamento de cliente, mantive a tabela cliente e fiz a generalização e especialização do cliente pf e cliente pj.

Para o refinamento da entrega, criei a tabela entrega, vinculada à tabela transportadora. Criei também a tabela entrega_movimento para registrar as movimentações da entrega do produto.

Para o refinamento do sistema de pagamento, crie a tabela pagamento, contendo diversos tipos de pagamento e, para a definição do tipo de pagamento, criei uma tabela intermediária chamada forma_pagamento.