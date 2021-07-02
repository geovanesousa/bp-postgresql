# bp-postgresql
Best practices in PostgreSQL.

PostgreSQL.

Boas práticas. 

----------
2 CAMPOS DE CONTROLE ESSENCIAIS EM UMA TABELA:

/*Este campo informa se o registro está ativo ou não.
Assim ao invés de excluirmos o registro posso desativá-lo. 
Basta alterar o campo ativo para FALSE.*/

ativo BOOLEAN NOT NULL DEFAULT TRUE

/*Armazena a data e a hora em que o registro foi inserido.
Essencial para uma futura auditoria.*/

data_criacao TIMESTAMP NOT NULL DEFAULT CURRENT_TIMESTAMP

----------
