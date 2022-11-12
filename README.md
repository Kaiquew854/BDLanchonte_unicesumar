# BDLanchonte_unicesumar

Um cliente solicitou sua empresa a criação de um banco de dados para armazenar os pedidos de uma lanchonete. A solicitação engloba o cadastro produtos, seus respectivos preços e tipos, além do cadastro dos clientes e a forma de pagamento de cada pedido. Após a reunião da equipe de analistas o seguinte DER (diagrama de entidade e relacionamento) foi elaborado como representação dos requisitos obtidos com o cliente:

![image](https://user-images.githubusercontent.com/80990220/201476629-848b5df3-8a07-4b08-98f1-99b27d76bf5a.png)


As tabelas a seguir contêm os dados dos pedidos:

![image](https://user-images.githubusercontent.com/80990220/201476654-d7708493-f225-481b-bea6-378a3cdb9d4d.png)


Chaves e Referências:

 

Tabela TIPO_PRODUTO:
- ID é chave primária.
 

Tabela TIPO_PAGTO:
- ID é chave primária.
 

Tabela PRODUTOS:
- ID é chave primária.
- ID_TIPO_PRODUTO é chave estrangeira e referencia ID da tabela TIPO_PRODUTO.

Tabela PEDIDOS:
- ID é chave primária.
- ID_TIPO_PAGTO é chave estrangeira e referencia ID da tabela TIPO_PAGTO.
 

Tabela PEDIDOS_PRODUTOS:
- ID é chave primária.
- ID_PEDIDO é chave estrangeira e referencia ID da tabela PEDIDOS.
- ID_PRODUTO é chave estrangeira e referencia ID da tabela PRODUTOS.

Com base nas informações descritas no DER e tabelas apresentadas, realize as seguintes atividades:

1) Crie um script contendo os comandos de criação das tabelas (CREATE TABLE), lembrando que os tipos dos campos poderá ser ao seu critério, porém, não fugindo da necessidade do campo.
2) Crie um script contendo os comandos de inserção de dados (INSERT), onde seja feita a inserção dos dados descritos nas tabelas acima.
3) Crie os comandos para apagar o conteúdos das tabelas (DELETE).
