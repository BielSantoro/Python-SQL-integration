# Integração Python-SQL

Para integrar Python ao SQL (Disponivel: https://www.postgresql.org/) será primeiro necessario se certificar da disponibilidade de uma database, no caso do exemplo foi utilizado o PostgreSQL com uma database 'aula' já criada. Em seguida será necessario um compilador python e a adição da biblioteca externa Psycopg (Disponivel: https://www.psycopg.org/)

## Explicação do codigo:

Veja que o código é responsável por criar rotinas de conexão, tabelas, inserção de dados e transações. Na linha 1 importamos a biblioteca PSYCOPG para que seus recursos possam ser utilizados durante a programação do módulo. Nas linhas 2 e 3 configuramos a conexão local ao banco de dados 'aula'. Já a linha 4 recupera o objeto 'cur' para acesso ao banco. Em seguida montamos um SQL para criar a tabela, que é executado a seguir. Na linha 7 criamos um SQL para inserir uma linha na tabela e a executamos em seguida. A linha 9 força a execução das transações pendentes e na linha 10 executamos um SQL de consulta. Da linha 11 até a 13 recuperamos e exibimos os resultados e ao final fechamos a conexão. 
