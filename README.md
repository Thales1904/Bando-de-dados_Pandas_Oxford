# Projeto II — Análise de Atividades Policiais em Rhode Island

## Sobre o projeto

A análise utiliza dados do [Stanford Open Policing Project](https://openpolicing.stanford.edu/) para investigar possíveis relações entre o gênero dos motoristas, as infrações de trânsito, os resultados das abordagens, as revistas veiculares, as prisões e as condições meteorológicas.

O trabalho também aborda etapas de preparação e limpeza de dados, análise estatística, visualização de informações, manipulação de séries temporais e integração de diferentes conjuntos de dados utilizando Python.

## Conjuntos de dados

O projeto utiliza dois conjuntos de dados:

| Arquivo | Descrição |
|---|---|
| `police.csv` | Registros de abordagens policiais e informações relacionadas aos motoristas, às infrações e aos resultados das abordagens. |
| `weather.csv` | Dados meteorológicos utilizados para analisar temperaturas e condições climáticas. |

## Etapas da análise

### 1. Preparação e limpeza dos dados

- Importação e inspeção inicial do conjunto `police.csv`.
- Identificação da quantidade de variáveis, registros e valores ausentes.
- Remoção de colunas desnecessárias para a análise.
- Tratamento de registros sem informação sobre o gênero do motorista.
- Verificação e conversão dos tipos de dados.
- Combinação das colunas de data e hora em uma variável do tipo `datetime`.
- Definição da data e hora da abordagem como índice do DataFrame.

### 2. Análise do gênero e das infrações

- Construção de distribuições de frequência das infrações.
- Criação de tabelas de contingência com frequências absolutas e relativas.
- Comparação dos tipos de infrações entre motoristas do sexo masculino e feminino.
- Visualização dos resultados por meio de gráficos de barras agrupadas.
- Comparação dos resultados das abordagens, especialmente notificações (*citations*) e advertências (*warnings*).
- Cálculo das taxas de revista veicular para o conjunto completo e para cada gênero.
- Investigação das taxas de revista considerando simultaneamente o gênero e o tipo de infração.

### 3. Análise exploratória e séries temporais

- Cálculo da taxa geral de prisão e análise de sua variação por hora do dia.
- Construção de gráficos de linha para visualizar as taxas de prisão ao longo das horas.
- Cálculo e visualização da taxa anual de abordagens relacionadas a drogas.
- Comparação das taxas anuais de revista e de ocorrências envolvendo drogas.
- Análise da distribuição das infrações entre os distritos policiais por meio de tabelas de contingência e gráficos de barras agrupadas.

### 4. Análise dos dados meteorológicos

- Exploração das variáveis de temperatura mínima (`TMIN`), média (`TAVG`) e máxima (`TMAX`).
- Cálculo de medidas estatísticas descritivas e construção de boxplots.
- Análise da distribuição da variável `TDIFF` por meio de medidas resumo e histogramas.
- Preparação e integração dos dados policiais e meteorológicos a partir das respectivas datas.
- Investigação de duas questões adicionais utilizando o conjunto de dados integrado.

## Estrutura do repositório

```text
Projeto2/
├── README.md
├── Projeto2.ipynb
└── Tabelas/
    ├── police.csv
    └── weather.csv
```
## **Autor**

**Thales Trajano**

**GitHub**: [@Thales1904](https://github.com/Thales1904)
