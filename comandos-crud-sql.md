# Comandos SQL - Para CRUD (Referência)

## Resumo
C -> Creat
R -> Read
U -> Upload
D -> Delete

<!-- ------------- -->

## Insert
## Fabricantes

```sql
INSERT INTO fabricantes (nome) VALUES ('Asus');
INSERT INTO fabricantes (nome) VALUES ('Asus');
INSERT INTO fabricantes (nome) 
VALUES('Apple'),('LG'),('Samsung'),('Brastemp');

```
<!-- -------------- -->

## Insert
## Produtos
```sql
INSERT INTO produtoss (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Ultrabook', 'Ultrabook Asus Intel Core i9', 
6500.99,
7,
1
);
INSERT INTO produtoss (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Geladeira',
'Frost-Free com acesso a internet',
 8500.99,
10,
6 -- Frost
);
INSERT INTO produtoss (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Tablet Android',
'Tablet 10 Polegadas com 256gb de armazenamento',
 4999,
3,
5 -- Sansumg
);
INSERT INTO produtoss (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Iphone 14 Pro Max',
'Processador Bionic 15 com 512gb de armazenamento',
9999.97,
3,
5 -- Apple
);
INSERT INTO produtoss (nome, descricao, preco, quantidade, fabricante_id)
VALUES('Ipad mini',
'Tablet com tela de retina 4k com 512gb de armazenamento',
5000,
8,
5 -- Apple
);


```

<!-- ------------------- ->

## Insert
## Produtos

```sql