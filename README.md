## Funções de agregação

### Servem para executar operações aritméticas nos registros de uma coluna 

As principais são: 

MAX(), MIN(), COUNT(), AVG(), SUM()

### Exemplos:

### calcule o preço minimo, maximo e médio dos produtos da tabela products

select min(price), max(price), avg(price)
from sales.products


![image](https://github.com/jucafernando/funcoes-agregacao/assets/21082881/d1194a1c-94e9-4a61-a3ca-f10e9daff3fc)


### Qual o produto mais caro da tabela products


select * from sales.products
where price = (select max(price) 
from sales.products)


![image](https://github.com/jucafernando/funcoes-agregacao/assets/21082881/c9de94de-22b1-451e-84eb-600a79441b4b)

#### Na query acima, utilizei uma subquery para selecionar todas as colunas do produto mais caro da tabela products. 
#### Sem a subquery, a unica informação possível de ser selecionada, seria uma coluna contendo o preço do produto, ou seja, 
#### para verificar outros campos relacionados as colunas dentro de um count(), é necessário realizar uma subquery. 
 
