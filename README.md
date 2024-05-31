<h1 align="center">Modelo de Classificação de Churn</h1>

<p align="center">
 <a href="#entendimento-do-negócio">Entendimento do negócio</a> •
 <a href="#tecnologias-utilizadas">Tecnologias utilizadas</a> •
 <a href="#tratamento-dos-dados">Tratamento dos dados</a> • 
 <a href="#entendimento-dos-dados">Entendimento dos dados</a> • 
 <a href="#perguntas-de-negócio">Perguntas de negócios</a
</p>

## Entendimento do negócio
<p align="justify">
Esta é uma proposta de resolução para um desafio da Formação em Dados da Escola DNC. Trata-se da criação de um modelo de classificação para mapear qual perfil de usuário tem mais chance de deixar uma plataforma de streaming. 

<p align="justify">
Os dados fornecidos possuem informações sobre as contas dos clientes na plataforma de streaming, como código de identificação, idade, gênero, dias de assinatura ativa, tipo de conta, avaliação média dos conteúdos da plataforma, número de perfis ativos, quantidade de serviços de streaming que o cliente possui, quantidade de dispositivos conectados à conta e a indicação se o cliente cancelou o serviço ou não.


## Tecnologias utilizadas
- Google Colab
- Python
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn

## Tratamento dos dados
<p align="justify">
Para utilizarmos as informações de maneira ideal, foi necessário remover linhas duplicadas, linhas com valores nulos em variáveis de interesse, substituir valores Nan e transformar os tipos de variáveis.

## Entendimento dos dados
<p align="justify">
Foi feita uma análise univariada para visualizar a distribuição dos dados afim de procurar por padrões ou tendências relevantes para o negócio, assim como uma análise multivariada, para entender a relação existente entre as variáveis.

<p align="justify">
Para a fazer a modelagem dos dados, foram utilizados o LabelEncoder, o MinMaxScaler e a função get_dummies do Pandas. O modelo escolhido foi o Random Forest Classifier, que foi implementado e tunado utilizando o scikit-learn.

## Perguntas de negócio
<p align="justify">
O modelo criado apresentou uma acurácia de 0.53. As métricas foram consideradas satisfatórias levando em conta que a distribuição da variável alvo era bastante desbalanceada. O tunning dos hiperparâmetros foi feito principalmente para reduzir o overfitting do modelo inicial, que apresentou uma perfomance muito discrepante entre treino e teste.



