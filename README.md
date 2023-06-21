## Funções de agregação

Servem para executar operações aritméticas nos registros de uma coluna 

As principais são: 

MAX(), MIN(), COUNT(), AVG(), SUM()

Exemplos:

-- calcule o preço minimo, maximo e médio dos produtos da tabela products

select min(price), max(price), avg(price)
from sales.products


![image](https://github.com/jucafernando/funcoes-agregacao/assets/21082881/d1194a1c-94e9-4a61-a3ca-f10e9daff3fc)
