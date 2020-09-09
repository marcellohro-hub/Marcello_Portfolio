# Meu portólio de data science

# [Projeto 1](https://github.com/marcellohro-hub/Rossman_challange)
Este projeto tem como objetivo simular um desafio real pedido por uma empresa. Para isso utilizei como base os dados da loja Rossmann do desafio [kaggle](https://www.kaggle.com/c/rossmann-store-sales). No final foi feito o deploy do modelo no [Heroku](https://rossmann1-model.herokuapp.com/).

Os dados fornecidos são basicamente uma TimeSeries dos dias mostrando as vendas bem como status de promoções e feriados, e uma outra planilha de dados gerais das lojas.
No próprio notebook o pipeline está bem claro e organizado, passando por featuring engineering, data cleaning, data preparation, etc. Na fase de seleção de variáveis utilizei o método Boruta. Para avaliar o melhor modelo utilizei cross-validation, e no final escolhi o XGBoost. A previsão do modelo foi traduzida em desempenho de negócio.

| ![](https://github.com/marcellohro-hub/Rossman_challange/blob/master/img/Capture.JPG) | 
|:--:| 
| *Desempenho dos modelos* |

| ![](https://github.com/marcellohro-hub/Rossman_challange/blob/master/img/whole_scenario.JPG) | 
|:--:| 
| *Previsão de vendas* |
