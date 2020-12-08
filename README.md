# Meu portólio de data science

# [Projeto 1](https://github.com/marcellohro-hub/Rossman_challange)
Este projeto tem como objetivo simular um desafio real pedido por uma empresa. Para isso utilizei como base os [dados da loja Rossmann](https://www.kaggle.com/c/rossmann-store-sales) de um desafio kaggle. As principais estapas consistem em:
* Analisar e levar insights sobre as vendas;
* Usar algoritmo de ML capaz de prever as vendas das próximas 6 semanas;
* Fazer [deploy](https://rossmann1-model.herokuapp.com/) do modelo de ML de forma que qualquer pessoa possa acessar as vendas das lojas.

# [Projeto 2](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis)
Este é um projeto de insight com o objetivo de analisar o mercado de engenharia mecânica (minha área original de formação). Fiz um web-scraping de 600 vagas de eng mecanica do linkedin, extraindo todos os textos das vagas (post, industry, applicants, description, etc). Com isso fiz análises estatísticas no pandas e utilizando a bilioteca spaCy de NLP. Pude extrair vários dados muito interessantes como por exemplo as habilidades com mais demanda:
 
| ![](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis/blob/master/img/habilidades.png) | 
|:--:| 
| *Habilidades x Número de vagas que pedem tal habilidade* |

Outras correlações envolvendo local, salário, indústria, palavras-chave do post, etc, estão na própria análise do notebook.

Atualização:

Este projeto foi muito bem recebido quando publiquei no linkedin, um colega da minha rede de conexões se interessou e propos desenvolver um [Guia de Profissões](http://tudosobrecarreira.com.br/guiadeprofissoes/) direcionado para alunos do Ensino Médio que ainda não decidiram o que fazer no vestibular.

# [Projeto 3](https://github.com/marcellohro-hub/Fraud_detection)

Projeto desafio sobre [fraude de cartão de crédito](https://sejaumdatascientist.com/crie-uma-solucao-para-fraudes-em-transacoes-financeiras-usando-machine-learning/) da Comunidade DS. Este projeto usa o dataset [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1) disponível na plataforma Kaggle.

Trata-se de uma empresa de detecção de fraude de cartão de crédito com a seguinte proposta ao seu cliente:

1. A empresa vai **receber 25%** do valor de cada transação detectada verdadeiramente como fraude.
2. A empresa vai **devolver 5%** do valor de cada transação detectada como fraude, porém a transação é verdadeiramente legítima.
3. A empresa vai **devolver 100%** do valor para o cliente, a cada transação detectada como legítima, porém a transação é verdadeiramente uma fraude.

Neste projeto pude testar várias técnicas de balanceamento e modelos de Machine Learning. Surpreendentemente não houve diferença significativa entre o resultado com os dados balanceados e não-balanceados. Em termos de acurácia obtive o seguinte resultado com o modelo final:

* Balanced Accuracy: 0.998765
* F1Score: 0.998764
* KappaScore: 0.998762

Este resultado traduz-se no seguinte resultado em desempenho de negócio:

Com um total de transação de $229,409,295,522.24 por parte do cliente, O valor faturado da companhia seria de $555,956,368.86. Isso equivale a $0.24 faturado a cada $100,00 de transação do cliente.

Mais informações sobre o desafio e o desempenho de negócio no read-me do projeto.

# [Projeto 4](https://gitlab.com/datascience-community/pa003_churn_predict/-/blob/pa003_marcello/churn.ipynb)

Projeto desafio sobre churning da [Comunidade DS](https://sejaumdatascientist.com/predicao-de-churn/). O Objetivo deste projeto é classificar a probabilidade clientes entrarem em churn. Este projeto usa o dataset [ChurnDataset](https://www.kaggle.com/mervetorkan/churndataset) disponível na plataforma Kaggle.


