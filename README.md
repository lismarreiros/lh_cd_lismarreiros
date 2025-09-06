# Análise de Dados e Modelagem para a PProductions

Este repositório contém o projeto de análise de dados e modelagem preditiva desenvolvido para a PProductions. 
O objetivo principal é extrair insights estratégicos de um dataset de filmes para auxiliar nas decisões sobre o próximo grande lançamento.

### Sumário do Projeto
O projeto foi estruturado em três etapas principais para garantir uma análise completa e aprofundada:

- Análise Exploratória de Dados (EDA): Uma exploração detalhada de variáveis como faturamento, nota do IMDb, gênero e número de votos para identificar padrões, tendências e correlações que podem guiar as decisões de negócio.

- Modelagem de Classificação: Criação de um modelo para inferir o gênero de um filme a partir do texto de sua sinopse (Overview).

- Modelagem de Regressão: Desenvolvimento de um modelo de regressão para prever a nota de um filme no IMDb com base em suas características numéricas, como número de votos e Meta_score.

### Estrutura do Repositório
A estrutura de pastas foi organizada para facilitar a navegação e a compreensão do projeto:

```lh_cd_lismarreiros/
├── data/
│   └── desafio_indicium_imdb.csv
├── models/
│   └── modelo_imdb.pkl
├── notebooks/
│   └── analise_completa.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```
### Como Executar o Projeto

1. Clone o Repositório:
```
git clone https://github.com/lismarreiros/lh_cd_lismarreiros.git
```
2. Instale as Dependências: Navegue até o diretório do projeto e instale todas as bibliotecas listadas no arquivo requirements.txt.

```
pip install -r requirements.txt
```
3. Execute o Notebook:

Abra o arquivo notebooks/analise_completa.ipynb em um ambiente como Jupyter Notebook ou Google Colab e execute todas as células.
O notebook contém o código completo e os resultados de cada etapa da análise.

### Insights e Conclusões Principais
A análise revelou insights importantes para a PProductions:

- Faturamento: Filmes dos gêneros Aventura, Animação e Sci-Fi apresentam a maior mediana de faturamento, tornando-os os gêneros mais lucrativos para investimento.

- Popularidade vs. Crítica: O número de votos no IMDb é o fator mais fortemente correlacionado com o faturamento (Gross), com uma correlação de 0.59. Em contraste, a nota do IMDb tem uma correlação de apenas 0.10 com o faturamento. Isso sugere que a popularidade é um indicador de sucesso financeiro mais forte do que a aprovação da crítica.

- Qualidade: O gênero Drama é o mais popular no dataset e, em geral, recebe as notas mais altas no IMDb.

- Análise da Sinopse (Overview): É possível inferir o gênero de um filme a partir de sua sinopse, pois o texto contém padrões de linguagem distintos. O modelo de classificação binária para o gênero 'Drama' teve um desempenho excelente, identificando todos os filmes de Drama no conjunto de teste com 100% de precisão.
