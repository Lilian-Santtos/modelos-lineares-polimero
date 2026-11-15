# Modelos Lineares — Modelagem Estatística e Avaliação de Performance

Trabalho da disciplina **Modelos Lineares** do curso de Ciência de Dados e Inteligência Artificial, desenvolvido em Python no Google Colab.

## Objetivo

Analisar o rendimento de um polímero sintético em dois estudos independentes:

- **Estudo 1 — Processo térmico:** regressão polinomial, comparação dos graus e diagnóstico dos resíduos.
- **Estudo 2 — Catalisador e pressão:** experimento fatorial 2 × 3, ANOVA com interação e teste de Tukey.

## Principais resultados

| Estudo | Resultado | Ressalva |
|---|---|---|
| Processo térmico | Modelo cúbico; rendimento máximo estimado de 88,58% a 205,68 °C | Falta de ajuste significativa (p = 0,0217) |
| Catalisador e pressão | Maior média: catalisador B + pressão Alta, 84,55% | Evidência de não normalidade dos resíduos (Shapiro-Wilk: p = 0,0169) |

Os estudos são **independentes**; os resultados não comprovam que as condições produzirão os mesmos rendimentos quando combinadas. Os dados são **sintéticos e fornecidos no enunciado da atividade**.

## Organização

- `Trabalho_Modelos_Lineares_Colab.ipynb`: notebook executável
- `dados/`: duas bases CSV utilizadas
- `resultados/graficos/`: figuras exportadas
- `resultados/tabelas/`: tabelas dos testes
- `Relatorio_Modelos_Lineares.pdf`: relatório escrito sem códigos

## Como executar no Google Colab

1. Baixe os arquivos CSV da pasta `dados/`.
2. No **Meu Drive**, crie a pasta `Modelos_Lineares_IESB` e envie os dois CSV.
3. Abra o notebook no [Google Colab](https://colab.research.google.com/).
4. Execute as células na sequência; os resultados serão salvos na subpasta `resultados`.

## Ferramentas

Python, Google Colab, pandas, NumPy, Matplotlib, SciPy e statsmodels.

## Relatório

O PDF apresenta metodologia, resultados, gráficos e conclusões de acordo com as orientações da atividade.