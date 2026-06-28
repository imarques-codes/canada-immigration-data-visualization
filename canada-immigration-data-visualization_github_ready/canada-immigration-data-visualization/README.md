# Canada Immigration Data Visualization

## Sobre o projeto

Este projeto apresenta uma análise visual dos dados de imigração para o Canadá no período de **1980 a 2013**, com foco especial na imigração do **Brasil** e na comparação com outros países da **América do Sul**.

O notebook foi desenvolvido no **Google Colab** e utiliza bibliotecas de análise e visualização de dados para explorar tendências, comparar países e criar gráficos estáticos e interativos.

---

## Objetivo

O objetivo principal é aplicar técnicas de **Análise de Dados** e **Visualização de Dados** para compreender o comportamento da imigração para o Canadá ao longo do tempo.

O projeto busca responder perguntas como:

- Como evoluiu a imigração do Brasil para o Canadá entre 1980 e 2013?
- Como o Brasil se compara a outros países da América do Sul?
- Quais países tiveram maior volume total de imigração para o Canadá?
- Como diferentes bibliotecas podem ser usadas para comunicar dados de forma visual?
- Como transformar dados históricos em gráficos claros, comparativos e interativos?

---

## Como funciona o projeto

O notebook segue um fluxo de análise dividido em etapas:

### 1. Importação e leitura dos dados

O projeto inicia com a leitura do arquivo `imigrantes_canada.csv` usando a biblioteca **Pandas**.

```python
import pandas as pd

df = pd.read_csv('/content/imigrantes_canada.csv')
```

> Observação: no Google Colab, o arquivo CSV precisa ser carregado no ambiente antes da execução. Para rodar localmente, recomenda-se colocar o arquivo dentro da pasta `data/` e ajustar o caminho no notebook.

---

### 2. Preparação da base

A coluna `País` é definida como índice do DataFrame, facilitando a seleção dos países para análise.

Também é criada uma lista com os anos de 1980 a 2013 para filtrar as colunas temporais.

Principais tratamentos realizados:

- Definição do índice por país;
- Seleção das colunas de anos;
- Criação de DataFrames específicos para Brasil e Argentina;
- Organização dos dados para gráficos de linha;
- Transposição de dados da América do Sul para visualizações interativas.

---

### 3. Análise da imigração do Brasil

O projeto isola os dados do Brasil e cria uma série temporal para analisar a evolução da imigração brasileira para o Canadá.

São utilizados gráficos de linha para visualizar a tendência ao longo dos anos.

---

### 4. Comparação com países da América do Sul

O notebook compara o Brasil com países como:

- Argentina
- Colômbia
- Peru

Também é criada uma visualização com os países da América do Sul ordenados pelo total de imigrantes no período.

---

### 5. Visualizações com Matplotlib

O projeto utiliza **Matplotlib** para criar:

- Gráficos de linha;
- Subplots comparativos;
- Boxplot;
- Gráfico de barras horizontais;
- Gráficos exportados em PNG.

Arquivos gerados no notebook:

```text
imigracao_brasil_canada.png
imigracao_america_sul.png
```

---

### 6. Visualizações com Seaborn

Com **Seaborn**, o notebook explora:

- Gráficos de barras;
- Top 10 países com maior imigração para o Canadá;
- Paletas de cores sequenciais, divergentes e categóricas;
- Temas visuais como `dark`, `whitegrid`, `white` e `ticks`;
- Remoção de molduras para gráficos mais limpos.

---

### 7. Visualizações interativas com Plotly

O projeto também utiliza **Plotly** para criar gráficos interativos, incluindo:

- Gráfico de linha interativo da imigração brasileira;
- Gráfico interativo da América do Sul;
- Exportação de gráfico em HTML;
- Animação comparando Brasil e Argentina ao longo dos anos.

Arquivo gerado no notebook:

```text
imigracao_america_sul.html
```

---

## Tecnologias utilizadas

- Python
- Google Colab
- Pandas
- Matplotlib
- Seaborn
- Plotly

---

## Estrutura sugerida do repositório

```text
canada-immigration-data-visualization/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── notebooks/
│   └── data_visualization_immigration_canada.ipynb
│
├── data/
│   └── README.md
│
└── img/
    └── README.md
```

---

## Como executar no Google Colab

1. Abra o notebook no Google Colab.
2. Faça upload do arquivo `imigrantes_canada.csv`.
3. Execute as células na ordem.
4. Analise os gráficos gerados ao longo do notebook.

Depois que o projeto estiver no GitHub, você poderá abrir diretamente no Colab usando um link neste formato:

```text
https://colab.research.google.com/github/imarques-codes/canada-immigration-data-visualization/blob/main/notebooks/data_visualization_immigration_canada.ipynb
```

---

## Como executar localmente

Clone o repositório:

```bash
git clone https://github.com/imarques-codes/canada-immigration-data-visualization.git
```

Acesse a pasta do projeto:

```bash
cd canada-immigration-data-visualization
```

Crie um ambiente virtual:

```bash
python -m venv .venv
```

Ative o ambiente virtual:

```bash
# Windows
.venv\Scripts\activate
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Abra o notebook:

```bash
jupyter notebook notebooks/data_visualization_immigration_canada.ipynb
```

---

## Base de dados

O projeto utiliza o arquivo:

```text
imigrantes_canada.csv
```

Esse arquivo deve conter dados históricos de imigração para o Canadá, organizados por país, região, continente, anos e total acumulado.

Caso a base de dados não esteja no repositório, coloque o arquivo dentro da pasta `data/` e ajuste o caminho de leitura no notebook para:

```python
df = pd.read_csv('data/imigrantes_canada.csv')
```

---

## Principais aprendizados

Este projeto fortalece conhecimentos práticos em:

- Manipulação de dados com Pandas;
- Seleção e transformação de dados;
- Análise temporal;
- Visualização de dados com Matplotlib;
- Criação de gráficos estatísticos e comparativos;
- Customização visual com Seaborn;
- Construção de gráficos interativos com Plotly;
- Organização de projeto para portfólio no GitHub.

---

## Possíveis melhorias futuras

- Adicionar a base de dados na pasta `data/`, caso a licença permita;
- Padronizar os títulos e textos dos gráficos;
- Criar uma seção de insights finais no notebook;
- Adicionar gráficos exportados na pasta `img/`;
- Criar uma versão em inglês do README;
- Transformar a análise em um dashboard interativo com Streamlit;
- Adicionar conclusão executiva com os principais achados da análise.

---

## Autor

**Igor Henrique Marques dos Santos**

- LinkedIn: [linkedin.com/in/igorhmarques](https://www.linkedin.com/in/igorhmarques/)
- GitHub: [github.com/imarques-codes](https://github.com/imarques-codes)
- E-mail: [igorhmsantos@gmail.com](mailto:igorhmsantos@gmail.com)

---

## Status do projeto

Projeto concluído como estudo prático de **Visualização de Dados com Python** e disponível para melhorias contínuas.
