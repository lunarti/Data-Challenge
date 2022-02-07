# Data Challenge 20210312 Victor Lunarti Valadão

Desafio Técnico realizado para a oportunidade Data Analyst em DeepESG.

## Parte 1.1

Contida no Jupyter Notebook: 'parte 1.1', exceto as questões de Banco de Dados que está no 'data.xlsx'

## Parte 1.2

Contida no Jupyter Notebook: 'parte 1.2'.

## Parte 2

Imagine que você recebeu uma demanda para gerar indicadores do GPTW para o RH com pelo menos algumas visões como:

- Distribuição de colaboradores por orientação sexual
- Distribuição de colaboradores por escolaridade
- Distribuição de colaboradores por faixa etária

Baseada nessa documentação, quais estruturas de dados você criaria para atender esta demanda?

Desenvolveria Scripts para automatização das consultas na API, logo estabeleceria a coordenação desses scripts utilizando o Apache Airflow resultando no seguinte banco de dados:

|Tabela Colaborador |  | |
--- | --- | ---|
|user_id|int|FK|
|job_titlenb              |int|FK|
|first_name|varchar(50)||
|last_name|varchar(50)||
|birthdate|date|
|gender|int|

Os nomes dos atributos foram retirados da documentação a fim de exibir os requisitos a serem extraídos da API.
O que se entende por Orientação Sexual não é definido por gênero, porém apenas este campo se encontra na documentação.

|Tabela Cargo |  | |
--- | --- | ---|
|job_title|int|PK|
|cbo|code||

A Escolaridade não foi encontrada na documentação, para isso escolhi o CBO para estimar uma possível escolaridade através do cargo exercido pelo Colaborador.

Posteriormente geraria os visuais utilizando Python ou Power BI para gerar os seguintes gráficos:

- Distribuição de colaboradores por orientação sexual: Gráfico de Barras

- Distribuição de colaboradores por escolaridade: Gráfico de Pizza

- Distribuição de colaboradores por faixa etária: Histograma

## Desafio Extra Excell

ARREDMULTB:
Arredonda um número para baixo, aproximando-o de zero, até o múltiplo mais próximo de significância.
ARREDMULTB(número, significância)

ARREDMULTB(DIA(MINUTO(A1/38)/2+56)&"/5"&"/"&A1;7)-34

Arrendonda DIA(MINUTO(A1/38)/2+56)&"/5"&"/"&A1 para baixo até o múltiplo mais próximo de 7.
1. Divide o Ano por 38 e converte em minutos, em sequência divide por 2 e soma 56.
2. Transforma o resultado de (1) em dias e concatena /5 e /Ano, transformando em uma data. 
3. Arredonda a data obtida em (2) para o múltiplo mais próximo de 7 (semana) -> equinócio
4. Subtrai -34 dias e obtém o resultado final -> primeiro domingo depois da lua cheia depois do equinócio vernal.

