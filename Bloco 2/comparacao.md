# Comparando os desempenhos dos modelos de regressão

Para poder comparar os valores, utilizamos os hiperparâmetros de melhor resultado para cada respectivo modelo.

## Baseline:
* MSE = 0.04
* RMSE = 0.19
* $R^2$ = -0.002

## Modelo #1: Regressão Linear
* MSE = 0.02
* RMSE = 0.16
* $R^2$ = 0.32

## Modelo #2: K Vizinhos Mais Próximos (k-NN)
Hiperparâmetro utilizado: número de vizinhos = 20

* MSE = 0.02
* RMSE = 0.14
* $R^2$ = 0.46

## Modelo #3: Árvore de Decisão
Hiperparâmetros utilizados: número máximo de folhas = 14;
número de profundidade = 8

* MSE = 0.02
* RMSE = 0.14
* $R^2$ = 0.49

## Modelo #4: Floresta Aleatória
Hiperparâmetros utilizados: número de árvores = 300;
número máximo de folhas = 10; número de profundidade = 5
* MSE = 0.02
* RMSE = 0.14
* $R^2$ = 0.42

A partir dos valores acima, concluimos que a Árvore de Decisão é o melhor modelo para este dataset e esta seed específica (61455). É importante frisar que, em outras seeds, os resultados poderiam ser diferentes.

Os critérios de avaliação dos modelos foram RMSE, MSE e $R^2$, sendo que o melhor RMSE é o mais próximo de 0; enquanto o $R^2$ mais ideal é o mais próximo de 1.

De maneira geral, no entanto, os modelos mais recomendados para o nosso dataset são os modelos #2 (k vizinhos mais próximos), #3 (árvore de decisão) e #4 (floresta aleatória). Futuramente, é indicada uma análise estatística mais extensa, de modo a avaliar o desempenho de cada modelo para seeds aleatórias diferentes, assim como a implementação de features com dados categóricos.