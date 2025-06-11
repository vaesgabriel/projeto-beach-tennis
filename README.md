# Projeto de Data Science – Análise e Modelagem de Vendas

## Tema do Projeto

Análise exploratória e modelagem preditiva de dados de vendas, com o objetivo de compreender o comportamento das vendas por região, segmento e subcategoria, além de prever a quantidade de itens vendidos utilizando técnicas de aprendizado de máquina.

## Repositório no GitHub

O projeto está hospedado no seguinte repositório do GitHub:

[https://github.com/vaesgabriel/projeto-beach-tennis.git](https://github.com/vaesgabriel/projeto-beach-tennis.git)

## Dataset Utilizado

Neste projeto, utilizamos um conjunto de dados que reúne informações mensais de vendas, distribuídas por região, segmento, estado e subcategoria de produtos. Os dados foram organizados para possibilitar análises detalhadas do desempenho comercial e servir como base para modelos preditivos.

A seguir, apresentamos a origem dos dados, as principais variáveis consideradas e as transformações aplicadas para adequação às técnicas de análise e modelagem.

### Origem

O dataset utilizado é fictício, criado para fins didáticos e de desenvolvimento do projeto. Os dados simulam registros de vendas mensais por região, segmento e subcategoria, permitindo a aplicação das técnicas de análise exploratória e modelagem preditiva abordadas. Apesar de simulados, os dados foram estruturados para refletir padrões plausíveis do mercado, garantindo relevância nas análises e resultados apresentados.

### Variáveis Principais

- **Ano**: Ano da venda (ex: 2023)  
- **Mês**: Mês da venda (1 a 12)  
- **Regiao**: Região geográfica da venda (ex: Sul, Sudeste)  
- **Estado**: Unidade federativa da venda (ex: RS, SP)  
- **Segmento**: Segmento de mercado do produto (ex: Insumos, Equipamentos)  
- **IDSubcategoriaProduto**: Código identificador da subcategoria do produto  
- **QuantidadeItens**: Quantidade total de itens vendidos em cada combinação das variáveis acima

### Transformações Realizadas

- Tratamento e limpeza dos dados, eliminando registros com valores faltantes ou inconsistentes  
- Agrupamento e sumarização dos dados para obtenção de vendas mensais por região, segmento e subcategoria  
- Criação de tabelas pivô para visualizações mais intuitivas, como mapas de calor por Estado e Mês  
- Codificação das variáveis categóricas por meio de OneHotEncoder para alimentar os modelos preditivos  
- Divisão dos dados em conjuntos de treino (80%) e teste (20%) para validação robusta dos modelos

## Modelos Utilizados ou Desenvolvidos

- **Regressão Linear**: Modelo preliminar para estabelecer relações lineares simples entre variáveis e quantidade vendida  
- **Random Forest Regressor**: Modelo principal utilizado para previsão da quantidade de itens vendidos, por sua capacidade de lidar com dados categóricos e capturar interações complexas  
- Pré-processamento automatizado via pipeline, integrando codificação e modelagem

## Resultados Obtidos

- O modelo Random Forest apresentou um **Erro Quadrático Médio (MSE)** de aproximadamente **447.27**, indicando que, em média, a diferença quadrática entre as previsões e valores reais é baixa  
- O **Coeficiente de Determinação (R²)** alcançou **0.35**, o que demonstra que o modelo explica cerca de 35% da variabilidade total das vendas, um desempenho razoável considerando a complexidade e variabilidade dos dados  
- As análises exploratórias mostraram que as vendas possuem forte variação por região, com as regiões Sul e Sudeste apresentando os maiores volumes  
- O segmento de equipamentos se destacou como principal responsável pelo volume de vendas, seguido pelos insumos  
- Visualizações como gráficos de barras e mapas de calor foram essenciais para identificar padrões sazonais e regionais, auxiliando na tomada de decisões estratégicas  
- O workflow construído permite atualizações contínuas com novos dados, facilitando o re-treinamento e melhoria progressiva dos modelos

---

*Este relatório foi elaborado com base no notebook e dados fornecidos, abrangendo desde a importação e limpeza dos dados até a análise exploratória, modelagem preditiva e visualização dos resultados.*
