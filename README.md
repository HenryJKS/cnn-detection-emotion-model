# Detecção de emoção por faces

- Dataset: https://www.kaggle.com/datasets/ananthu017/emotion-detection-fer

Classes: **Feliz**, **Triste**, **Surpreso**

## Dados
São identificados 3 classes, com diferenças significaticas de quantidades de imagens em cada dados, assim foi utilizado o aumento de dados, e a penalização para erros cometidos na classes com menores quantidades de imagens.

## Modelo
Conforme o modelo criado, foram usados:
- 1 camada de entrada, 6 camadas ocultas e 1 camada de saída

Nas camadas ocultas é realizada a `normalização` para diminuir a distância dos dados, e o `Dropout` para evitar o `overfitting`. Na camada de saída foi utilizado a função de ativação `softmax` para classificação de multiclasse
- treinado com 25 épocas

## Avaliação do algoritmo
Após o treinamento, o modelo atingiu uma acurácia de 0.81 com loss de 0.4

## Modelo Final

modelo salvo como `.keras`.