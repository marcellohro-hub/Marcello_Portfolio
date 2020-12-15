# Meu portólio de data science

# [Projeto 1](https://github.com/marcellohro-hub/Rossman_challange)
**Tema: Regressão para previsão de vendas de uma time-series. Modelo final: XGBoost.**

Este projeto tem como objetivo simular um pedido de previsão de vendas por uma empresa. Foi utilizado os [dados da loja Rossmann](https://www.kaggle.com/c/rossmann-store-sales) de um desafio kaggle. As principais estapas consistem em:
* Analisar e levar insights sobre as vendas (efeito de promoções, feriados, distância ao concorrente, etc);
* Usar algoritmo de regressão capaz de prever as vendas das próximas 6 semanas;
* Fazer [deploy](https://rossmann1-model.herokuapp.com/) do modelo de ML de forma que qualquer pessoa possa acessar as vendas das lojas.

# [Projeto 2](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis)
**Tema: Insights sobre carreira. Principais técnicas utilizadas: Web-scraping e NLP.**

Este é um projeto de insight com o objetivo de analisar o mercado de engenharia mecânica (minha área original de formação). Fiz um web-scraping de 600 vagas de eng mecanica do linkedin, extraindo todos os textos das vagas (post, industry, applicants, description, etc). Com isso fiz análises estatísticas no pandas e utilizando a bilioteca spaCy de NLP. Pude extrair vários dados muito interessantes como por exemplo as habilidades com mais demanda:
 
| ![](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis/blob/master/img/habilidades.png) | 
|:--:| 
| *Habilidades x Número de vagas que pedem tal habilidade* |

Outras correlações envolvendo local, salário, indústria, palavras-chave do post, etc, estão na própria análise do notebook.

Atualização:

Este projeto foi muito bem recebido quando publiquei no linkedin, um colega da minha rede de conexões se interessou e propos desenvolver um [Guia de Profissões](http://tudosobrecarreira.com.br/guiadeprofissoes/) direcionado para alunos do Ensino Médio que ainda não decidiram o que fazer no vestibular.

# [Projeto 3](https://github.com/marcellohro-hub/Fraud_detection)
**Tema: Detecção de fraudes. Modelo final: random forest para classificação**

Projeto que visa simular o modelo de negócio de uma empresa fictícia de combate a fraude de cartão de crédito. Este projeto usa o dataset [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1) disponível na plataforma Kaggle.

A empresa de detecção de fraude de cartão de crédito tem a seguinte proposta ao seu cliente:

1. A empresa vai **receber 25%** do valor de cada transação detectada verdadeiramente como fraude.
2. A empresa vai **devolver 5%** do valor de cada transação detectada como fraude, porém a transação é verdadeiramente legítima.
3. A empresa vai **devolver 100%** do valor para o cliente, a cada transação detectada como legítima, porém a transação é verdadeiramente uma fraude.

Neste projeto pude testar várias técnicas de balanceamento e modelos de Machine Learning. Surpreendentemente não houve diferença significativa entre o resultado com os dados balanceados e não-balanceados. Em termos de acurácia obtive o seguinte resultado com o modelo final (random forest otimizado com fine-tuning):

* Balanced Accuracy: 0.998765
* F1Score: 0.998764
* KappaScore: 0.998762

Este resultado traduz-se no seguinte resultado em desempenho de negócio:

Com um total de transação de $229,409,295,522.24 por parte do cliente, O valor faturado da companhia seria de $555,956,368.86. Isso equivale a $0.24 faturado a cada $100,00 de transação do cliente.

Mais informações sobre o desafio e o desempenho de negócio no read-me do projeto.

# [Projeto 4](https://github.com/marcellohro-hub/Churn_prediction)
**Tema: Previsão de evasão de clientes. Modelo final: redes neurais para classificação**

Este projeto visa simular a produção de um plano de ações para uma empresa de serviços bancários sofrendo alta taxa de evasão de clientes. Essa evasão é chamada de **churn** nas métricas de negócio. Foi utilizado o dataset [ChurnDataset](https://www.kaggle.com/mervetorkan/churndataset) disponível no site de competições kaggle.

Após testar vários modelos, escolhi redes neurais como modelo final. Utilizei um fine-tuning para calibrar o número de neurônios em cada cadamada, drop-out rate, batch-size e otimizador, obtendo o seguinte score final:

* Recall: 0.72
* Ballanced Accuracy: 0.77
* F1 Score: 0.60
* Kappa Score: 0.48

Por fim, seguindo a proposta do desafio, arbitrei condições de incentivos para evitar a evasão de clientes. Esses incentivos são baseados na probabilidade de churning dada pelo modelo final para cada cliente:

Para clientes com probabilidade de churning maior que 50%:
* Investir 10% * retorno_do_cliente * probabilida_de_churning, com um teto de $10,000

Para clientes com probabilidade de churning menor que 50%:
* Investir valor igual ao retorno dado pelo cliente com um teto de $500,00

Se esse investimento tiver 100% de eficácia, isto é, fizer com que mais nenhum cliente entre em churning, equivaleria a um ROI de $23,00 a cada $1,00 investido.

