# Comandos SQL - Referência
<!-- -------------------------- -->
## Modelagem física

### Criar banco de dados
```sql
CREATE DATABASE vendas CHARACTER SET utf8mb4;

```


<!-- -------------------------------- -->

### Criar a tabela fabricantes

```sql
CREATE TABLE fabricantes(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL
)


```
<!-- -------------- -->


```sql
CREATE TABLE fabricantes(
    id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    nome VARCHAR(45) NOT NULL,
    descricao TEXT (1000) NOT NULL,
    preco DECIMAL (6,2) NOT NULL,
    quantidade TINYINT (4) NOT NULL
)


```
<!-- -------------------- -->


### Adicionar campo/coluna em uma tabela

```sql
ALTER TABLE produtos ADD fabricantes_id INT NOT NULL
AFTER quantidade;

```
<!-- -------------------- -->


### Criação da chave estrangeira (relacionamento entre tabelas)

```sql
ALTER TABLE produtos
    # CONTRAINT é uma restrição definida no relacionamento
    ADD CONSTRAINT fk_produtos_fabricantes

    # A chave estrangeira deve fazer referência da chave primaria
    FOREIGN KEY(fabricantes_id) REFERENCES fabricantes(id)

```