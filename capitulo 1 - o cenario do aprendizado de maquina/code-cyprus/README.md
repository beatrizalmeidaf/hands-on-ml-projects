# Treinamento e Execução de um Modelo Linear com Scikit-Learn

## Objetivo

Este projeto tem como objetivo treinar e executar modelos de regressão linear e KNN (K-Nearest Neighbors) utilizando a biblioteca Scikit-Learn. O foco é prever a satisfação com a vida em função do PIB per capita dos países.

## Ferramentas e Bibliotecas Utilizadas

- **Python**: Linguagem de programação utilizada para o desenvolvimento do código.
- **Pandas**: Biblioteca para manipulação e análise de dados.
- **NumPy**: Biblioteca para operações numéricas e manipulação de arrays.
- **Matplotlib**: Biblioteca para visualização de dados.
- **Scikit-Learn**: Biblioteca de aprendizado de máquina que fornece ferramentas para modelagem e validação.

## Dados

Os dados utilizados neste projeto foram baixados de repositórios online e consistem em dois arquivos CSV:

1. **oecd_bli_2015.csv**: Contém dados sobre a satisfação com a vida de vários países, incluindo indicadores como "Life satisfaction" (satisfação com a vida) e "INEQUALITY" (desigualdade).
2. **gdp_per_capita.csv**: Contém dados sobre o PIB per capita dos países.

### Estrutura dos Dados

- **oecd_bli_2015.csv**:
  - `Country`: Nome do país.
  - `Indicator`: Indicador da satisfação com a vida.
  - `Value`: Valor do indicador.
  - `INEQUALITY`: Categoria de desigualdade (por exemplo, "TOT" para total).

- **gdp_per_capita.csv**:
  - `Country`: Nome do país.
  - `2015`: PIB per capita em 2015.

## Funcionalidades

1. **Preparação dos Dados**: A função `prepare_country_stats` é responsável por preparar e organizar os dados, filtrando por desigualdade total e combinando os dois DataFrames em um único DataFrame que contém o PIB per capita e a satisfação com a vida.

2. **Visualização dos Dados**: Um gráfico de dispersão é gerado para visualizar a relação entre o PIB per capita e a satisfação com a vida.

3. **Modelo de Regressão Linear**: Um modelo de regressão linear é treinado utilizando os dados de PIB per capita como variável independente e satisfação com a vida como variável dependente.

4. **Previsões**: O modelo é utilizado para fazer previsões sobre a satisfação com a vida para um novo valor de PIB per capita (neste caso, 50.587).

5. **Modelo KNN**: Um modelo KNN é treinado e utilizado para prever a satisfação com a vida para o mesmo valor de PIB per capita.

## Como Executar

Para executar o código, siga os passos abaixo:

1. **Instale as bibliotecas necessárias**:
   ```bash
   pip install pandas numpy matplotlib scikit-learn
2. **Baixe os arquivos de dados se necessário**: O código automaticamente baixa os arquivos necessários do repositório online, mas está disponível também na pasta.

3. **Execute o script**: Execute o script em um ambiente Python (recomendado: Jupyter Notebook) para visualizar os resultados e gráficos.
