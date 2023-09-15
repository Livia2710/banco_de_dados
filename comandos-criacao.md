<!-- MD = Mark Down  -->

<!-- h1 -->
# Comandos SQL - Referência 

<!--h2--->
## Modelagem física

<!-- h3 -->
### Criar banco de dados

```sql 
CREATE DATABASE vendas CHARACTER SET utf8mb4; 

```
<!-- _____________FABRICANTES________________ -->

<!-- h3 -->
### Criar tabela fabricantes

```sql 
CREATE TABLE fabricantes (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)

```
<!-- _____________PRODUTO___________________ -->

<!-- h3 -->
### Criar tabela produtos

```sql 
CREATE TABLE produtos (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT(1000) NOT NULL,
    preco DECIMAL(6,2) NOT NULL,
    quantidade TINYINT(4) NOT NULL
)

```