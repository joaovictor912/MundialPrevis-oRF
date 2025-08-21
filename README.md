# MundialPrevis-oRF
# Simulador Preditivo do Mundial de Clubes FIFA 2025

##  Objetivo do Projeto

Este projeto é um simulador computacional criado para estimar as probabilidades de cada um dos 32 times participantes vencer o Mundial de Clubes da FIFA de 2025. O objetivo não é prever um único campeão com certeza, mas sim quantificar as chances de cada clube com base em uma série de dados e estatísticas, reconhecendo a natureza imprevisível do futebol.

## Lógica e Algoritmos

A lógica central do projeto é a **Simulação de Monte Carlo**, onde o torneio completo é simulado 1.000 vezes para identificar os resultados mais frequentes.

Cada partida individual dentro da simulação é prevista por um algoritmo de Machine Learning, o **`Random Forest Classifier`** da biblioteca `scikit-learn`. Este algoritmo calcula as probabilidades de vitória, empate ou derrota com base em um "Power Score" de cada time, que leva em conta:

-   Ranking histórico dos últimos 5 anos (com pesos para anos recentes).
-   Valor de mercado do elenco.
-   Média de gols marcados e sofridos, ajustada pela força da liga continental de cada clube.

## Como Executar

1.  Clique no botão "Open in Colab" no topo deste notebook.
2.  No ambiente do Colab, execute todas as células em ordem (`Ambiente de execução -> Executar tudo`).
3.  O resultado final, com a tabela de probabilidades e o gráfico, será exibido ao final da execução.
