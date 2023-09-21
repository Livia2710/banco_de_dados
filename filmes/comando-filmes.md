# Comandos SQL - Referência 
### Criar banco de dados

```sql 
CREATE DATABASE cinema CHARACTER SET utf8mb4; 

```

### Criar tabela filmes

```sql 
CREATE TABLE filmes (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    titulo VARCHAR(45) NOT NULL,
    lançamento YEAR(4)  
)


```

```sql 
CREATE TABLE genero (
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    genero VARCHAR(45) NOT NULL 
)


```

<!-- h3 -->
### Adicionar campo/coluna em uma tabela

```sql 

ALTER TABLE filmes ADD genero_id INT NOT NULL
AFTER lançamento;

```

<!-- ________________________________ -->

<!-- h3 -->
### Criação da chave estrangeira (relacionamento entre tabelas)

```sql 
ALTER TABLE produtos
ADD CONSTRAINT fk_filmes_genero


FOREIGN KEY(genero_id) REFERENCES generos(id)

```
```sql 

INSERT INTO genero (titulo)
VALUE ('Ação'), ('Comedia'), ('Drama'), ('Romance'), ('Suspense'), ('Terror'), ('Ficção Cientifica');

```


```sql 
INSERT INTO filme(titulo, lançamento, genero_id) 
VALUE('Star Wars: Episodio III - A Vingança dos Sith',
2005, 
7,
);

INSERT INTO filme(titulo, lançamento, genero_id) 
VALUE('A Freira',
2018, 
6,
);

INSERT INTO filme(titulo, lançamento, genero_id) 
VALUE('Para todos garotos que já amei',
2018, 
4,
);

INSERT INTO filme(titulo, lançamento, genero_id) 
VALUE('A Queda',
2022, 
5,
);




```