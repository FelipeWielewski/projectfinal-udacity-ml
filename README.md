# Machine Learning Engineer Nanodegree
# Projeto Final 
# Felipe Wielewski

### Install

Para executar o projeto será necessário as seguintes bibliotecas:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

Todo o código foi escrito e documentado utilizando o [Jupyter Notebook](http://ipython.org/notebook.html)
Desenvolvido em python 2.7 (conda)

## Code
Para desenvolvimento do modelo preditivo foi efetuado pré-processamento dos dados e aplicado algoritmo de GradientBoostingRegressor para treinar a base.
Como métrica foi utilizado o R2 Score, com GridSearchCV para encontrar a melhor combinação de parametros.

### Data

A [base de dados](https://www.kaggle.com/c/instacart-market-basket-analysis) é baseada em um dataset publicado no kaggle, que foi alvo de competição entre os usuários, com mais de 3 milhões de registros. Nesse projeto iremos utilizar uma parte dessa base para processamento e treinamento do modelo.

**Features**
1.  `user_id`: identificador do usuário
2. `order_number`: numeração do pedido
3. `order_dow`: dia da semana da compra
4. `order_hour_of_day`: hora da compra
5. `product_id`: produto do pedido
6. `department_id`: departamento do produto
7. `mean_days_since_order_user`: media de tempo desde a ultima compra

**Target Variable**
4. `days_since_prior_order`: Tempo que irá levar entre as compras