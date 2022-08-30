# Reconhecimento_de_Personalidade
Projeto de Machine Learning para o Reconhecimento de Personalidade a partir de um questionário que avalia 5 traços fortes de personalidade. 

Este projeto é baseado na pesquisa de modelo de cinco fatores (FFM) na qual utiliza avaliação de associação entre palavras, sendo capazes de descrever alguém, ou mais especificamente, os traços de personalidade das pessoas, onde tais palavras, são frequentementes aplicadas a mesma pessoa, descrevendo seus aspectos de personalidade.

## O algoritimo

O algoritimo utiliza-se da biblioteca YellowBrick, para efetuar a clusterização dos nossos dados e a biblioteca Sklearn, com o algoritimo KMeans para a modelagem

    from sklearn.cluster import KMeans
  
    from yellowbrick.cluster import KElbowVisualizer

Tendo em vista que o projeto trabalha em cima de 5 traços de personalidade, iremos separar os dados em 5 Clusters para treino e validação.

## Aplicação

No intuito de validar o modelo, ao final do Notebook, há uma interface, criada a partir da biblioteca Gradio, na qual contém as perguntas de modelo de pesquisa, onde é possível responder o questionário, e ao final identificar, através do modelo de aprendizado de máquina, qual a sua personalidade.

## DataBase
A base de dados e as perguntas estão disponibilizadas pela Kaggle, no link:
https://www.kaggle.com/datasets/tunguz/big-five-personality-test
