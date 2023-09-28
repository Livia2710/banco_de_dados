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

<!-- ________________________________ -->

<!-- h3 -->
### Adicionar campo/coluna em uma tabela

```sql 

ALTER TABLE produtos ADD fabricante_id INT NOT NULL
AFTER quantidade;

```

<!-- ________________________________ -->

<!-- h3 -->
### Criação da chave estrangeira (relacionamento entre tabelas)

```sql 
ALTER TABLE produtos
# CONSTRAINT é uma restrição definifida no relacionamento
ADD CONSTRAINT fk_produtos_fabricantes

#A chave estrangeira deve fazer referencia a chave primaria
FOREIGN KEY(fabricante_id) REFERENCES fabricantes(id)

```