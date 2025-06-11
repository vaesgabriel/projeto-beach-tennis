# Projeto Ciência de Dados – Beach Tennis

## Tema do Projeto

Análise e modelagem preditiva de dados relacionados ao beach tennis, visando extrair insights relevantes sobre o desempenho dos jogadores e prever resultados das partidas, utilizando técnicas de ciência de dados e aprendizado de máquina.

## Repositório no GitHub

O projeto está hospedado no seguinte repositório GitHub:

[https://github.com/vaesgabriel/projeto-beach-tennis.git](https://github.com/vaesgabriel/projeto-beach-tennis.git)

*(Substitua pelo link correto do seu repositório.)*

## Dataset Utilizado

### Origem

O dataset foi coletado a partir de fontes públicas e oficiais de torneios de beach tennis, contendo dados históricos de partidas, jogadores e condições associadas.

### Variáveis Principais

- **data**: Data da partida
- **jogador_1** e **jogador_2**: Identificação dos jogadores participantes
- **pontos_jogador_1** e **pontos_jogador_2**: Pontuação final de cada jogador
- **local**: Local onde a partida foi realizada
- **condicoes_climaticas**: Informações meteorológicas do dia da partida
- **categoria_partida**: Categoria ou tipo do torneio
- **outros atributos técnicos e estatísticos**

### Transformações Realizadas

- Limpeza e padronização dos nomes dos jogadores para evitar duplicidades
- Conversão da coluna de datas para formato datetime
- Tratamento de valores ausentes e inconsistentes, com exclusão ou imputação conforme o contexto
- Criação de variáveis derivadas, como diferença de pontos, categorização de condições climáticas e indicadores de desempenho prévio
- Normalização e escalonamento das variáveis numéricas para alimentar os modelos preditivos
- Divisão do dataset em conjuntos de treino e teste para validação dos modelos

## Modelos Utilizados ou Desenvolvidos

- **Regressão Linear Múltipla** para prever a pontuação total dos jogadores em partidas futuras, utilizando variáveis preditoras como condições climáticas, local e desempenho anterior
- **Árvore de Decisão** para classificar o vencedor da partida com base nas variáveis técnicas e ambientais
- **Random Forest** para otimizar a classificação do vencedor, combinando várias árvores de decisão e melhorando a robustez do modelo

## Resultados Obtidos

- A regressão linear atingiu um erro médio quadrático (MSE) de aproximadamente 447.27, com um coeficiente de determinação (R²) de 0.35, indicando que o modelo explica cerca de 35% da variância da pontuação
- A árvore de decisão apresentou uma acurácia satisfatória na previsão do vencedor, com limitações em partidas muito equilibradas
- O modelo Random Forest melhorou a precisão, apresentando maior capacidade de generalização nos dados de teste
- Análises exploratórias indicaram que fatores como condições climáticas e local da partida influenciam diretamente o desempenho dos jogadores
- O workflow adotado permite a atualização contínua com novos dados e aprimoramento dos modelos

---

*Este relatório foi gerado a partir do workflow desenvolvido no notebook do projeto, contemplando desde a coleta dos dados até a modelagem preditiva.*

