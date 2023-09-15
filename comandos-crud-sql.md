<!-- MD = Mark Down  -->

<!-- h1 -->
# Comandos SQL - Para CRUD Referência 

<!--h2--->
## Resumo

C -> Create (Insere dados)
R ->Read (Ler dados)
U ->Update (Atualizar)
D -> Delete (Deletar)

<!-- ___________________________________________ -->

## insert
## Fabricantes

```sql 
INSERT INTO fabricantes (nome) VALUE('Asus');
INSERT INTO fabricantes (nome) VALUE('Dell');
INSERT INTO fabricantes (nome)
VALUE ('Apple'), ('LG'),('Samsung'), ('Brastemp')

```

<!-- ___________________________________________ -->

## insert
## Produtos

```sql 
INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Ultrabook','Ultrabook Asus Intel Core 19',
6500.99, 
7,
1
);



```


