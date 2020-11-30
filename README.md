# Meu portólio de data science

# [Projeto 1](https://github.com/marcellohro-hub/Rossman_challange)
Este é o projeto final do curso [DS_em_produção](https://datascienceemproducao.kpages.online/como-ser-um-data-scientist?ref=Q40443728O&gclid=CjwKCAiAnIT9BRAmEiwANaoE1eyf2FNWx6xBsxDHqL6oIiIMX4y0Vthvov9dqodrmUdyJc2XvnkZDBoCcxQQAvD_BwE). Tem como objetivo simular um desafio real pedido por uma empresa. Para isso utilizei como base os dados da loja Rossmann do desafio [kaggle](https://www.kaggle.com/c/rossmann-store-sales). No final fiz o deploy do modelo no [Heroku](https://rossmann1-model.herokuapp.com/).

# [Projeto 2](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis)
Este é um projeto de insight com o objetivo de analisar o mercado de engenharia mecânica (minha área original de formação). Fiz um web-scraping de 600 vagas de eng mecanica do linkedin, extraindo todos os textos das vagas (post, industry, applicants, description, etc). Com isso fiz análises estatísticas no pandas e utilizando a bilioteca spaCy de NLP. Pude extrair vários dados muito interessantes como por exemplo as habilidades com mais demanda:
 
| ![](https://github.com/marcellohro-hub/Linkedin_scraping-and-analysis/blob/master/img/habilidades.png) | 
|:--:| 
| *Habilidades x Número de vagas que pedem tal habilidade* |

Outras correlações envolvendo local, salário, indústria, palavras-chave do post, etc, estão na própria análise do notebook.

Atualização:

Este projeto foi muito bem recebido quando publiquei no linkedin, um colega da minha rede de conexões se interessou e propos desenvolver um [Guia de Profissões](http://tudosobrecarreira.com.br/guiadeprofissoes/) direcionado para alunos do Ensino Médio que ainda não decidiram o que fazer no vestibular.

# [Projeto 3](https://github.com/marcellohro-hub/Fraud_detection)

Projeto desafio sobre [fraude de cartão de crédito](https://sejaumdatascientist.com/crie-uma-solucao-para-fraudes-em-transacoes-financeiras-usando-machine-learning/) da Comunidade DS. Este projeto usa o dataset [Synthetic Financial Datasets For Fraud Detection](https://www.kaggle.com/ntnu-testimon/paysim1) do kaggle.

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
