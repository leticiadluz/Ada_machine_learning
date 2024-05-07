# Projetos Machine Learning ADA Tech

**No repositório, você encontrará os projetos dos módulos Machine Learning I e Machine Learning II do curso de Data Science da AdaTech do programa Santander Coders.**

### Machine Learning I
O primeiro projeto tem como objetivo desenvolver um modelo preditivo capaz de antecipar o risco de um indivíduo sofrer um ataque cardíaco. 
Para o desenvolvimento do projeto, utilizamos o dataset Heart Attack Risk Prediction, disponível no site do [Kaggle](https://www.kaggle.com/datasets/iamsouravbanerjee/heart-attack-prediction-dataset). 
Este dataset foi criado a partir de dados sintéticos gerados por inteligência artificial. Inicialmente, realizamos uma análise exploratória dos dados e, 
à medida que avançamos na análise, percebemos que variáveis bem estabelecidas na literatura médica, como obesidade, diabetes e tabagismo, não tinham relação com o target. 
Isso representa um problema significativo na construção de modelos na área da saúde. Devido ao tempo limitado para o projeto, optamos por continuar utilizando o 
mesmo dataset para desenvolver os modelos de machine learning. Para as variáveis que não mostraram relação clara, realizamos testes de hipóteses e, ao final, selecionamos as 
variáveis mais relevantes para o modelo com base na literatura médica e nos testes realizados.  

**O notebook com a Análise exploratória de dados pode ser acessado [aqui]**(https://github.com/leticiadluz/Ada_machine_learning/blob/main/EDA.ipynb)

**O dataset limpo após a análise exploratória e remoção de variáveis não importantes, pode ser acessado [aqui]**(https://github.com/leticiadluz/Ada_machine_learning/blob/main/df_IAM_risco_final.csv)  

Construímos seis modelos de Machine Learning utilizando três estimadores diferentes: regressão logística, KNN e Random Forest. Realizamos pré-processamento das variáveis, escolhendo as mais adequadas para cada estimador, além de otimização de hiperparâmetros e seleção de variáveis. A métrica escolhida para a avaliação do modelo foi o recall, pois em um problema como o risco de ataque cardíaco, priorizamos identificar todos os verdadeiros positivos e minimizar os falsos negativos.
Em nenhum dos modelos gerados conseguimos um recall superior a 0.60, mesmo após várias tentativas de otimização. 
Ao revisitar a seção de discussão no Kaggle, outros usuários relataram o mesmo problema, indicando que não é possível gerar um bom modelo com um dataset que não reflete a realidade.  

**O notebook com os modelos de Machine Learning pode ser acessado [aqui]**(https://github.com/leticiadluz/Ada_machine_learning/blob/main/ML.ipynb)

### Devido a uma falha de atenção inicial, selecionamos um conjunto de dados que não representa a realidade e não demonstra correlação entre as variáveis preditoras e o target, uma vez que o dataset é sintético. Isso inviabiliza a implementação do modelo em produção. Portanto, seria necessário recomeçar a modelagem utilizando dados mais robustos e confiáveis.

