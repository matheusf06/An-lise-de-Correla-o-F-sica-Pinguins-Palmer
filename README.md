# 🐧 Análise de Correlação Física: Pinguins Palmer

![Badge em Andamento](http://img.shields.io/static/v1?label=STATUS&message=CONCLUIDO&color=GREEN&style=for-the-badge)
![Badge Python](http://img.shields.io/static/v1?label=Tecnologia&message=PYTHON&color=blue&style=for-the-badge)

## 📑 Índice
1. [Introdução e Problema de Negócio](#1-introdução-e-problema-de-negócio)
2. [Tecnologias Utilizadas](#2-tecnologias-utilizadas)
3. [Metodologia (Processo de Análise)](#3-metodologia-processo-de-análise)
4. [Principais Insights e Visualizações](#4-principais-insights-e-visualizações)
5. [Conclusão](#5-conclusão)

---

## 1. Introdução e Problema de Negócio
Este projeto visa analisar as características físicas de três espécies de pinguins do arquipélago Palmer (Adelie, Chinstrap e Gentoo) para identificar padrões de dimorfismo e correlações biológicas.

**A Pergunta de Negócio (Ask):**
> "Existe uma correlação direta entre o comprimento e a profundidade do bico dos pinguins? Essa relação se mantém igual para todas as espécies ou varia individualmente?"

## 2. Tecnologias Utilizadas
O projeto foi desenvolvido em **Python** utilizando o ambiente Jupyter Notebook.
* **Pandas:** Para manipulação e limpeza dos dados (Data Cleaning).
* **Seaborn / Matplotlib:** Para visualização de dados e plotagem estatística.
* **Dataset:** Palmer Penguins (dados brutos contendo medidas de peso, nadadeiras e bicos).

## 3. Metodologia (Processo de Análise)
Seguindo o roteiro de análise de dados do Google:
1.  **Coleta:** Importação do dataset via biblioteca Seaborn.
2.  **Limpeza (Process):** Identificação e remoção de dados nulos (NaN) para garantir a integridade estatística.
3.  **Exploração:** Análise preliminar usando `groupby` para entender as médias por espécie.
4.  **Visualização:** Criação de gráficos de dispersão com regressão linear para validar hipóteses.

## 4. Principais Insights e Visualizações

### Hipótese: Pinguins com bicos mais compridos têm bicos mais profundos?

Ao plotar os dados gerais, percebemos um fenômeno estatístico interessante (Paradoxo de Simpson). Se olharmos os dados misturados, a correlação parece fraca. Porém, ao segmentar por espécie, a tendência fica clara.

![Insira aqui a imagem do seu gráfico salvo](grafico.png)


**Descobertas:**
* **Correlação Positiva:** Dentro de cada espécie, existe uma relação linear positiva. Quanto maior o comprimento do bico, maior tende a ser sua profundidade.
* **Diferenciação de Espécies:**
    * Os pinguins **Gentoo** (verde) possuem bicos menos profundos, mas com grande variação de comprimento.
    * Os pinguins **Adelie** (azul) tendem a ter bicos mais curtos e profundos.

## 5. Conclusão
A análise confirma que as dimensões do bico são características distintivas fortes entre as espécies e mantêm uma proporção de crescimento previsível. Para futuros estudos, sugere-se cruzar esses dados com o sexo dos animais para verificar se há dimorfismo sexual impactando essas medidas.

---
*Autor: Matheus Feijão Oliveira*
*Conecte-se comigo no [LinkedIn](https://www.linkedin.com/in/matheusfeijao/)*
