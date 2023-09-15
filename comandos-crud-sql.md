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
VALUE ('Apple'), ('LG'),('Samsung'), ('Brastemp');
INSERT INTO fabricantes (nome)
VALUE ('Positivo'), ('Microsoft');

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

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Geladeira',
'Frost-Free com acesso a internet',
8500.99, 
10,
6
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Tablet',
'Tablet 10 polegadas com 256GB de armazenamento',
4999, 
3,
5
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Iphone 14 Pro Max',
'Processador Bionic 15 com 512GB de armazenamento',
9999.97, 
3,
3
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Ipad mini',
'Tablet com tela de resina 4k com 512GB de armazenamento',
5000, 
8,
3
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Xbox',
'Console de ultima geração',
2500, 
6,
8
);

INSERT INTO produtos(nome, descricao, preco, quantidade, fabricante_id) 
VALUE('Ultrabook',
'AMD Ryzen 5 160BG RAM...',
4500.97, 
12,
7
);






```


