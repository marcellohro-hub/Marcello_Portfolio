# Meu portólio de data science

# [Projeto 1](https://github.com/marcellohro-hub/Rossman_challange)
Este é o projeto final do curso [DS_em_produção](https://datascienceemproducao.kpages.online/como-ser-um-data-scientist?ref=Q40443728O&gclid=CjwKCAiAnIT9BRAmEiwANaoE1eyf2FNWx6xBsxDHqL6oIiIMX4y0Vthvov9dqodrmUdyJc2XvnkZDBoCcxQQAvD_BwE). Tem como objetivo simular um desafio real pedido por uma empresa. Para isso utilizei como base os dados da loja Rossmann do desafio [kaggle](https://www.kaggle.com/c/rossmann-store-sales). No final fiz o deploy do modelo no [Heroku](https://rossmann1-model.herokuapp.com/).

Os dados fornecidos são basicamente uma TimeSeries dos dias mostrando as vendas bem como status de promoções e feriados, e uma outra planilha de dados gerais das lojas.
No próprio notebook o pipeline está bem claro e organizado, passando por featuring engineering, data cleaning, data preparation, etc. Na fase de seleção de variáveis utilizei o método Boruta. Para avaliar o melhor modelo utilizei cross-validation, e no final escolhi o XGBoost. A previsão do modelo foi traduzida em desempenho de negócio.

| ![](https://github.com/marcellohro-hub/Rossman_challange/blob/master/img/whole_scenario.JPG) | 
|:--:| 
| *Previsão de vendas* |

# [Projeto 2](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis)
Este é um projeto de insight com o objetivo de analisar o mercado de engenharia mecânica (minha área original de formação). Fiz um web-scraping de 600 vagas de eng mecanica do linkedin, extraindo todos os textos das vagas (post, industry, applicants, description, etc). Com isso fiz análises estatísticas no pandas e utilizando a bilioteca spaCy de NLP. Pude extrair vários dados muito interessantes como por exemplo as habilidades com mais demanda:
 
| ![](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis/blob/master/img/habilidades.png) | 
|:--:| 
| *Habilidades x Número de vagas que pedem tal habilidade* |

Outras correlações envolvendo local, salário, indústria, palavras-chave do post, etc, estão na própria análise do notebook.

# [Projeto 3](https://github.com/marcellohro-hub/Fraud_detection)

Projeto desafio sobre [fraude de cartão de crédito](https://www.kaggle.com/ntnu-testimon/paysim1) da Comunidade DS. Este projeto usa o dataset [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1) do kaggle. Neste projeto pude testar várias técnicas de balanceamento e modelos de Machine Learning. Surpreendentemente não houve diferença significativa entre o resultado com os dados balanceados e não-balanceados. Em termos de acurácia obtive o seguinte resultado com o modelo final:

* Balanced Accuracy: 0.998765
* F1Score: 0.998764
* KappaScore: 0.998762

Mais informações sobre o desafio e o desempenho de negócio no read-me do projeto.
