# Data Challenge 20210312

Hey tudo bem?
Esse é nosso desafio Hands on, aqui nós vamos ver um pouquinho do seu mão na massa e você terá um gostinho de como será seu dia a dia por aqui :)

### Parte 1.1

Segue em anexo o questionário com a primeira parte.

### Parte 1.2

Baseado na estrutura de dados apresentada, descreva os comandos SQL que você escreveria se a mesma estivesse numa estrutura de banco de dados.

## Parte 2

Imagine que você recebeu uma demanda para gerar indicadores do GPTW para o RH com pelo menos algumas visões como:

1. Distribuição de colaboradores por orientação sexual
2. Distribuição de colaboradores por escolaridade
3. Distribuição de colaboradores por faixa etária 
   
Para a realização desta demanda você recebeu a seguinte documentação: https://documenter.getpostman.com/view/4785048/RWMCvVxN?version=latest

Baseada nessa documentação, quais estruturas de dados você criaria para atender esta demanda?

## Extras

### 1- Desafio extra (plus ++)

Fazer a conexão da API acima (caso GPTW do RH), listando os colaboradores no Power BI, segue um exemplo de como fazer essa conexão https://www.c-sharpcorner.com/blogs/power-bi-report-generation-through-web
   

Para finalizar esse desafio, você precisará:

1. Criar uma conta trial em nosso produto (https://app.pontomaisweb.com.br/) `(Token: $2a$10$FgvbKMpP5PpHG/PBrb8KLOZZLqMIoPCYakT.04lyDJc/7SIKs2sxu)`
2. Acessar o marketplace e ativar a API (menu marketplace / extensões / API)
3. Pegar o token e passar como um dos parâmetros do Header (explicado na
   documentação acima)
   

### 2- Excel extra (plus ++)
   
Para entregar um relatório de SLA (Prazo para entregar/concluir o serviço), era preciso calcular todos os feriados e finais de semana de determinado período. Várias datas são fixas (Natal e Ano-Novo por exemplo) e outras são móveis (Páscoa e Carnaval). 

Para o cálculo do dia em que a Páscoa cairá, podemos utilizar a seguinte fórmula no Excel: `"=ARREDMULTB(DIA(MINUTO(A1/38)/2+56)&"/5"&"/"&A1;7)-34"` (considerando que o ano esteja na célula A1).
Explique a lógica utilizada para o cálculo da Páscoa nessa fórmula, detalhando o que cada função faz no resultado esperado.


## Readme do Repositório

- Deve conter o título do projeto
- Uma descrição de uma frase
- Instruções em geral e arquivos finais do projeto
- Capturas do resultado final do Projeto
- Link para acessar o projeto em caso que tenha sido utilizado um sistema Online.
- Não esqueça o [.gitignore](https://www.toptal.com/developers/gitignore)

## Finalização

Avisar sobre a finalização e enviar para correção em: [https://coodesh.com/review-challenge](https://coodesh.com/review-challenge)
Após essa etapa será marcado a apresentação/correção do projeto.

## Instruções para a Apresentação:

1. Será necessário compartilhar a tela durante a vídeo chamada;
2. Deixe todos os projetos de solução previamente abertos em seu computador antes de iniciar a chamada;
3. Prepara-se pois você será questionado sobre cada etapa e decisão do Challenge;
4. Prepare uma lista de perguntas, dúvidas, sugestões de melhorias e feedbacks (caso tenha).

## Suporte

Use o nosso canal no slack: http://bit.ly/32CuOMy para tirar dúvidas sobre o processo ou envie um e-mail para contato@coodesh.com.
