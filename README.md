# Meu portólio de data science

# Projeto 1
Este projeto tem como objetivo simular um desafio real pedido por uma empresa. Para isso utilizei como base os dados da loja Rossmann do desafio [kaggle](https://www.kaggle.com/c/rossmann-store-sales). 

## Contexto
* Reunião mensal de resultados para definição de orçamento;
* CFO pediu uma previsão de vendas das próximas 6 semanas de cada loja;

## Proposta
* Análisar e levar insights sobre as vendas;
* Usar algoritmo de ML capaz de prever as vendas das próximas 6 semanas;
* Fazer deploy do modelo de ML de forma que qualquer pessoa possa acessar as vendas das lojas;

## Detalhes do Pipeline

1. DESCRICAO DOS DADOS
* Preenchimento de NANs
  * Distância de competidores (competition_distance): foi suposto que a competição fica muito distance, logo substituido por 200000;
  * Data de abertura dos competitodes (competition_open_since_month e competition_open_since_year): foi suposto que a competição foi fundada há muito tempo, logo substituido pela data 01/1900;
  * Início da promoção 2 (promo2): foi suposto que a promo 2 terá início em 01/2018 (no futuro);
* Estatística descritiva dos dados numéricos e categóricos
1. FEATURE ENGINEERING
* Criação de hipóteses
** Nesta etapa foi criado um mapa mental de hipóteses sobre o negócio;
** Utilização de gráficos para 
   1. Criacao das Hipoteses
   1. Lista Final de Hipóteses
   1. Feature Engineering
1. PASSO 03 - FILTRAGEM DE VARIÁVEIS
3.1. Filtragem das Linhas
3.2. Selecao das Colunas
4.0. PASSO 04 - ANALISE EXPLORATORIA DOS DADOS
4.1. Analise Univariada
4.1.1. Response Variable
4.1.2. Numerical Variable
4.1.3. Categorical Variable
4.2. Analise Bivariada
H1. Lojas com maior sortimentos deveriam vender mais.
H2. Lojas com competidores mais próximos deveriam vender menos.
H3. Lojas com competidores à mais tempo deveriam vendem mais.
H4. Lojas com promoções ativas por mais tempo deveriam vender mais.
H5. Lojas com mais dias de promoção deveriam vender mais.
H7. Lojas com mais promoções consecutivas deveriam vender mais.
H8. Lojas abertas durante o feriado de Natal deveriam vender mais.
H9. Lojas deveriam vender mais ao longo dos anos.
H10. Lojas deveriam vender mais no segundo semestre do ano.
H11. Lojas deveriam vender mais depois do dia 10 de cada mês.
H12. Lojas deveriam vender menos aos finais de semana.
H13. Lojas deveriam vender menos durante os feriados escolares.
4.2.1. Resumo das Hipoteses
4.3. Analise Multivariada
4.3.1. Numerical Attributes
4.3.2. Categorical Attributes
5.0. PASSO 05 - DATA PREPARATION
5.1. Normalizacao
5.2. Rescaling
5.3. Transformacao
5.3.1. Encoding
5.3.2. Response Variable Transformation
5.3.3. Nature Transformation
6.0. PASSO 06 - FEATURE SELECTION
6.1. Split dataframe into training and test dataset
6.2. Boruta as Feature Selector
6.2.1. Best Features from Boruta
6.3. Manual Feature Selection
7.0. PASSO 07 - MACHINE LEARNING MODELLING
7.1. Average Model
7.2. Linear Regression Model
7.2.1. Linear Regression Model - Cross Validation
7.3. Linear Regression Regularized Model - Lasso
7.3.1. Lasso - Cross Validation
7.4. Random Forest Regressor
7.4.1. Random Forest Regressor - Cross Validation
7.5. XGBoost Regressor
7.5.1. XGBoost Regressor - Cross Validation
7.6. Compare Model's Performance
7.6.1. Single Performance
7.6.2. Real Performance - Cross Validation
8.0. PASSO 08 - HYPERPARAMETER FINE TUNING
8.1. Random Search
8.2. Final Model
9.0. PASSO 09 - TRADUCAO E INTERPRETACAO DO ERRO
9.1. Business Performance
9.2. Total Performance
9.3. Machine Learning Performance
10.0. PASSO 10 - DEPLOY MODEL TO PRODUCTION
10.1. Train model for deployment
10.2. Rossmann Class
10.3. Testing Rossman Class on a Kaggle submission
10.4. API Handler
10.5. API Tester
