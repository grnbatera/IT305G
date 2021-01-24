# IT305G
Repositório do Projeto da Disciplina de Gestão de Energia Eficiência Energética.

# Estrutura de Arquivos e Pastas

A estrutura [Cookiecutter Data Science](https://drivendata.github.io/cookiecutter-data-science/) simplificada do projeto: 

~~~
├── README.md          <- apresentação do projeto.
│
├── data
│   ├── external       <- dados dos anuários utilizados no projeto.
│   ├── processed      <- dados normalizados usados nos modelos de regressão não lineares.
│   └── raw            <- dados originais sem modificações.
│
├── notebook           <- Google Colaboratory notebook do projeto.
│
├── Python 3.0         <- Linguagem de programação do projeto.
│
└── assets             <- Gráficos, Apresentação PDF e Pitch do projeto.
~~~

## `data`

Neste projeto foram utilizados dados externos de fonte aberta para o estudo de regressão não linear, a saber:

#### `external`

[Resultados do Procel](https://drive.google.com/drive/folders/1lXbcbY7AO2QKraQjPi9V74p87YyijNLu?usp=sharing): Fonte de dados contendo o desempenho do Brasil frente a Eficiência Energética e a prestação de contas do Procel;

[Balanço Energético Nacional](https://drive.google.com/drive/folders/1qC8e7uvXWioR11aF4E_RErYfV3_8sFTb?usp=sharing): Fonte de dados com a contabilização relativa à oferta e ao consumo de energia no Brasil, contemplando as atividades de extração de recursos energéticos primários, sua conversão em formas secundárias, importação e exportação, a distribuição e o uso final da energia;

[Anuário Estatítisco de Energia Elétrica](https://drive.google.com/drive/folders/11ri-E-GgCDF2cmAugMsTSBX7PH-5Ingr?usp=sharing): Fonte de dados onde são divulgados os dados detalhados relacionados ao consumo de energia elétrica na rede de distribuição;

[Atlas da Eficiência Energética](https://drive.google.com/drive/folders/1Tht_77lq2VXDvLFrLQJtgIHGYOuwEkG9?usp=sharing): Fonte de dados dos indicadores de Eficiência Energética;

[World Energy Trilemma](https://drive.google.com/drive/folders/1Zy2W9BlIaWLzoALv1s9b2YJpO2MkkIEK?usp=sharing): Fonte de dados com o Ranking Internacional e análise dos países com relação ao trilema de energia e sustentabilidade.

#### `processed`

[D1An](https://github.com/grnbatera/IT305G/blob/main/D1An.csv): Dados das fontes externas unificadas e normalizadas para a utilização nos modelos de Regressão não linear em Machine Learning;

[Mapa de Variáveis](https://github.com/grnbatera/IT305G/blob/main/mapadevariaveisdeD1A.csv): Tabela contendo a descrição das variáveis de D1An utilizadas no projeto.

#### `raw`

[D1A](https://github.com/grnbatera/IT305G/blob/main/D1An.csv): Dados das fontes externas unificadas com os valores originais para a utilização nos modelos de Regressão não linear em Machine Learning;

[Mapa de Variáveis](https://github.com/grnbatera/IT305G/blob/main/mapadevariaveisdeD1A.csv): Tabela contendo a descrição das variáveis de D1A utilizadas no projeto.

## `notebook`

[Projeto IT305G](https://github.com/grnbatera/IT305G/blob/main/Projeto_IT305G.ipynb): Notebook em Google Colaboratory do projeto.

## `src`

Todo o projeto foi realizado em um único notebook em Google Colaboratory em Python 3.0

## `assets`

[Gráficos](https://github.com/grnbatera/IT305G/tree/main/Mídias): Todos os gráficos utilizados neste projeto;

[Apresentação](https://github.com/grnbatera/IT305G/blob/main/Apresentação%20IT305G%20-%20Gleyson(043801).pdf): PDF contendo uma versão simplificada do projeto;

[Pitch](http://bit.ly/youtubeIT305G): Vídeo curto de apresentação do projeto.

# Apresentação do Projeto:

## `Regressão de Dados dos Anuários de Energia e Eficiência Energética para Tomada de Decisão em Políticas Públicas Utilizando Machine Learning`
### `Data Regression from Energy and Energy Efficiency Yearbooks for Decision Making in Public Policies Using Machine Learning`

# Descrição:
~~~
Este projeto visa unificar fontes de dados livres relativas ao uso de energia e eficiência energética com o objetivo de obter um modelo de regressão não linear por Machine Learning e, através deste modelo, propor políticas públicas que ajudem o Brasil a melhorar sua posição com relação ao World Energy Trilemma. 

Assim, após a unificação dos dados e sua normalização (uma vez que as variáveis envolvidas possuem valores muito distintos entre si), os dados foram submetidos aos processos de regressão não linear por machine learning o modelo com o melhor desempenho de score de treino, score de teste e RMSE foi a regressão por Gradient Boosting.

A regressão por Gradient Boosting trouxe 5 variáveis mais importantes para o modelo e, a partir disso, foram elaboradas 3 propostas de políticas públicas visando melhorar estas variáveis e consequentemente o posicionamento do Brasil com relação ao Trilemma.
~~~

# Abstract:
~~~
This project aims to unify free data sources related to the use of energy and energy efficiency in order to obtain a non-linear regression model by Machine Learning and, through this model, to propose public policies that help Brazil to improve its position in relation to the World Energy Trilemma.

Thus, after the data was unified and normalized (since the variables involved have very different values), the data were submitted to non-linear regression processes by machine learning, the model with the best performance of training score, score test and RMSE was regression by Gradient Boosting.

The regression by Gradient Boosting brought 5 most important variables to the model and, based on that, 3 public policy proposals were elaborated in order to improve these variables and consequently Brazil's position in relation to Trilemma.
~~~

# Equipe
* `Gleyson Roberto do Nascimento` - `043801`

# Vídeo do Projeto
[![Projeto IT305G](https://github.com/grnbatera/IT305G/blob/main/Mídias/thumb.jpg)](http://bit.ly/youtubeIT305G)


# Introdução e Motivação
~~~
Na atualidade, a análise de dados está se tornando cada vez mais importante dada a sua capacidade de encontrar padrões e possibilidades antes não cogitadas e, assim, auxiliar em tomadas de decisão. Desta forma, através de metodologias de Machine Learning, serão analisados dados unificados de cinco tipos de anuários complementares visando uma tomada de decisão que resulte em políticas públicas que melhorem o posicionamento do Brasil com relação ao seu posicionamento no World Energy Trilemma.
~~~

## Perguntas de Pesquisa
~~~
Tentaremos verificar aqui se:

1) Considerando-se as variáveis existentes nos anuários, existe alguma correlação de forma a validar uma regressão não linear?

2) Se existe uma regressão não linear possível, existe uma metodologia simples em Machine Learning ou será necessário o uso do Deep Learning?

3) Escolhida uma metodologia, os resultados de score e RMSE são aceitáveis ou teve overfitting/underfitting?

4) Supondo que a metodologia possui resultados aceitáveis, ela consegue indicar a importância das features (variáveis)?

5) Uma vez conhecidas as importâncias das features (variáveis), é possível fazer uma tomada de decisão para implementar políticas públicas?

6) Uma vez sugeridas as políticas públicas, estas surgem para alterar alguma já existente ou são completamente novas? Além disso, são simples ou muito complexas para implementar? 
~~~

## Objetivos do projeto
~~~
Considerando-se uma grande variedade nos valores das variáveis encontradas nos anuários utilizados como fontes de dados, não seria possível uma convergência válida para uma regressão não linear, assim, a metodologia mais adequda foi a normalização de dados, viabilizando o estudo científico e sua aplicação em Machine Learning. A partir disso, as análises seguiram o fluxo investigativo das pergguntas da pesquisa com vistas a uma tomada de decisão prática nas políticas públicas. Como pode ser visto no Diagrama 01.
~~~
![Diagrama 01](https://github.com/grnbatera/IT305G/blob/main/Mídias/diag01.jpg)

# Recursos e Métodos

## Bases de Dados

Base de Dados | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
D1A | https://github.com/grnbatera/IT305G/blob/main/D1A.csv | `Dados sem modificação utilizados como base para o projeto`
D1An | https://github.com/grnbatera/IT305G/blob/main/D1An.csv | `Dados normalizados que de fato foram utilizados nos modelos de Machine Learning do projeto`

## Ferramentas

Ferramenta | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Regressão Multivariável | http://bit.ly/39Q5zuR | `Modelo de Regressão Multivariável utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Árvore de Decisão | http://bit.ly/2LJxjti | `Modelo de Regressão por Árvore de Decisão utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Árvore de Decisão com AdaBoost | http://bit.ly/398eWHn | `Modelo de Regressão por Árvore de Decisão com AdaBoost utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por AdaBoost | http://bit.ly/3ivTT4v | `Modelo de Regressão por AdaBoost utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por GradientBoosting | http://bit.ly/2LRmhlE | `Modelo de Regressão por GradientBoosting utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Bagging | http://bit.ly/3phELud | `Modelo de Regressão por Bagging utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Random Forest | http://bit.ly/3o4lmv5 | `Modelo de Regressão por Random Forest utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Support Vector Regressor | http://bit.ly/2NoD8g6 | `Modelo de Regressão por Support Vector Regressor utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`


# Metodologia
~~~
De forma simplificada, o banco de dados unificado possuía 59 variáveis diferentes, de forma que para encontrar alguma correlação entre elas optou-se pelo método clássico da regressão não linear, ou seja, buscou-se entender como 58 variáveis independentes se relacionavam para chegar a uma variável dependente, que no caso é o posicionamento do Brasil no ranking do World Energy Trilemma. Como existe um número significativo de variáveis optou-se pelos 10 principais métodos de regressão não linear por Machine Learning disponíveis para o Python 3.0. Conforme o Diagrama 02 abaixo: 
~~~
![Diagrama 02](https://github.com/grnbatera/IT305G/blob/main/Mídias/diag02.jpg)

## Detalhamento do Projeto
~~~
Uma vez que os dados brutos foram normalizados, devido a grande disparidade de grandezas entre as variáveis existentes, estes passaram pelos 10 principais algorítmos de regressão não linear por Machine Learning disponíveis no Python 3.0. Para a análise destas saídas foram considerados 3 principais parâmetros: o score de treino, o score de teste e o RMSE. De forma que as respostas puderam ser compiladas conforme a tabela abaixo:
~~~

Posição | Método | Score de Treino | Score de teste | RMSE - Raiz do Erro Quadrático Médio
----- | ----- | ----- | ----- | -----
1 | Regressão com GradientBoosting | 0.9999999060685 | 0.930055664679408 | 0.154478588479773
2 | Regressão por Árvore de Decisão com AdaBoost | 0.889162561576354 | 0.948979591836734 | 0.131936203536836
3 | Regressão por AdaBoost | 0.889162561576354 | 0.948979591836734 | 0.131936203536836
4 | Regressão por Support Vector Regressor - Kernel Polynomial | 0.99018307556021 | 0.733055286436736 | 0.301788496308552
5 | Regressão Multivariável | 1 | 0.657599492165343 | 0.341789895132097
6 | Regressão por Bagging | 0.809579182630907 | 0.466085600907028 | 0.426803365676911
7 | Regressão por Support Vector Regressor - Kernel Linear | 0.990168652051838 | 0.612689391992557 | 0.363514479861328
8 | Regressão por Random Forrest | 0.783752287732621 | 0.400043845663265 | 0.452430396339587
9 | Regressão por Support Vector Regressor - Kernel RBF | 0.990157176414034 | 0.144717519805832 | 0.540190331461215
10 | Regressão por Árvore de Decisão | 0.997263273125342 | -0.0306122448979591 | 0.592979483991658

~~~
Após a análise desta resposta, chegou-se a conclusão que o melhor método de regressão não linear foi a rgressão por Gradient Boosting e, a partir disso, foi feita a análise das principais features fornecidas por este modelo para então haver uma tomada de decisão para elaboração de políticas públicas.
~~~

## Evolução do Projeto
~~~
Os principais desafios enfrentados durante o andamento deste projeto se concentraram nas seguintes áreas:

a) Fontes de dados: infelizmente os dados possuem periodicidade anual, de forma que seriam poucas as observações possíveis na série e isto poderia comprometer o modelo de regressão não linear e até mesmo não ser possível encontrar um modelo válido. Além disto, não existe uma padronização na elaboração dos anuários, ou seja, a cada governo existem distintas formas de apresentação de dados e isto contribuiu para que existissem apenas 59 variáveis confiáveis e constantes em todos as fontes consultadas. Outro ponto muito relevante é que não há garantias de uniformidade de metodologia entre as fontes, de forma que temos apenas que assumir essa similaridade para continuar o projeto;

b) Valores dos dados: as ordens de grandeza existentes entre váriaveis eram muito grandes, de forma que isso comprometeu os testes inciais dos modelos de regressão, sendo muito comum o overfitting e grandes valores de RMSE, contudo ao adotar a estratégia de padronização dos dados, este deixou de ser um problema, a partir daí, a obtenção de modelos com valores aceitáveis de score de treino, score de teste e RMSE foi mais comum.

c) Aleatoriedade em modelos de regressão por Machine Learning: um dos pontos positivos e, também, negativos dos métodos de regressão por Machine Learning é que muitos deles utilizam raízes randômicas, de forma que o lado positivo é que o método não se limita, podendo encontrar uma solução mudando sua raiz, contudo o lado negativo é que podem ser necessárias várias tentativas até que se chegue a um resultado plausível e, sem garantias de que este mesmo resultado volte a ocorrer se o programa rodar novamente, de forma que uma vez que o resultado foi positivo, se deve verificar as features imediatamente. 
~~~

# Resultados e Discussão
~~~
Com base na aplicação dos dados padronizados nos modelos de regressão não lineares por Machine Learning foram obtidos os seguintes resultados:
~~~
Comparativo entre os dados reais e os regredidos | Comparativo entre os dados reais e os regredidos
----- | -----
![Gráfico 01](https://github.com/grnbatera/IT305G/blob/main/Mídias/g01.png) | ![Gráfico 02](https://github.com/grnbatera/IT305G/blob/main/Mídias/g02.png)
![Gráfico 03](https://github.com/grnbatera/IT305G/blob/main/Mídias/g03.png) | ![Gráfico 04](https://github.com/grnbatera/IT305G/blob/main/Mídias/g04.png)
![Gráfico 05](https://github.com/grnbatera/IT305G/blob/main/Mídias/g05.png) | ![Gráfico 06](https://github.com/grnbatera/IT305G/blob/main/Mídias/g06.png)
![Gráfico 07](https://github.com/grnbatera/IT305G/blob/main/Mídias/g07.png) | ![Gráfico 08](https://github.com/grnbatera/IT305G/blob/main/Mídias/g08.png)
![Gráfico 09](https://github.com/grnbatera/IT305G/blob/main/Mídias/g09.png) | ![Gráfico 10](https://github.com/grnbatera/IT305G/blob/main/Mídias/g10.png)
~~~
Desta maneira, ao analisarmos os dados e gráficos podemos concluir que o melhor método de regressão não linear por Machine Learning para os dados normalizados foi a a regressão por Gradient Boosting, de forma que este modelo trouxe as seguintes features (variáveis) mais relevantes:
~~~

Feature | Importância | Descrição
----- | ----- | -----
v29 | 1 | Geração Distribuída - Gás Natural(%)
v46 | 2 | Consumo Médio Tensão A2 - 88 a 138 kV (GWh)
v37 | 3 | Tarifa Média Tensão A1 - 230kV ou mais(R$/MWh)
v47 | 4 | Consumo Médio Tensão A3 - 69kV(GWh)
v49 | 5 | Consumo Médio Tensão A4- 2,3 a 25 kV(GWh)

~~~
Uma vez que as features (variáveis) mais relevantes foram determinadas, cabe a análise destas na série de dados, como segue:
~~~

Comportamento das features na série de dados | Comportamento das features na série de dados
----- | -----
![Gráfico 11](https://github.com/grnbatera/IT305G/blob/main/Mídias/g11.png) | ![Gráfico 12](https://github.com/grnbatera/IT305G/blob/main/Mídias/g12.png)
![Gráfico 13](https://github.com/grnbatera/IT305G/blob/main/Mídias/g13.png) | 

~~~
Assim, considerando o comportamento das features, podemos estabelecer 3 sugestões de políticas públicas:

a) Para o Gás Natural na Geração Distribuída:  Incentivo fiscal para uso do Biogás, de forma que a unidade consumidora que consiga fazer o manejo dos resíduos e utilizá-lo como Biogás de forma adequada e sustentável tenha redução dos principais impostos pagos para cada nível (IPTU, ISS, ICMS, etc). Além disso, para que exista a possibilidade de que cada grupo possa ter acesso aos meios para se criar o Biogás,  medidas como treinamentos e linhas de crédito de baixo custo são importantíssimos. Desta forma, além de aumentar participação do Gás Natural na Geração Distribuída, melhorando o índice mais importante do modelo de regressão de Machine Learning, estaremos de fato melhorando a atual solução de manejo de resíduos e dando valor à uma fonte de energia subutilizada;

b) Para o Consumo nas Tensões A2, A3 e A4:  Este é um item mais complicado, uma vez que demanda uma adequação da rede para aumento do fornecimento de uma dada tensão ou uma adequação da unidade consumidora à uma nova tensão de entrada. Assim, a proposta seria mais de estudos para uma melhor distribuição entre as faixas de tensões, de forma que as faixas de tensão tenham um consumo mais equilibrado entre si, deslocando unidades consumidoras de faixa quando isto for viável segundo estudo prévio e dando incentivos fiscais e linhas de crédito para adequação de equipamentos para a nova faixa de tensão; 

c) Para a Tarifa Média na Tensão A1: A proposta para este caso é mais simples, de forma que a unidade consumidora que conseguir melhorar sua Eficiência Energética, na forma de redução de MWh em sua conta, tenha a tarifa reduzida proporcionalmente a redução de energia durante o ano, ou seja, se em 1 ano houver uma economia de 5%, a tarifa será reduzida em 5% e assim por diante, incentivando a Eficiência Energética e melhorando um índice importante no modelo de Machine Learning, o que levará a uma posição melhor no trilemma.
~~~

# Conclusões
~~~
Primeiramente, podemos responder os questionamentos iniciais deste projeto:

1) Considerando-se as variáveis existentes nos anuários, existe alguma correlação de forma a validar uma regressão não linear?
R- Sim, existem correlações e foi possível validar uma regressão não linear por Gradient Boosting.

2) Se existe uma regressão não linear possível, existe uma metodologia simples em Machine Learning ou será necessário o uso do Deep Learning?
R- O Gradient Boosting é uma metodologia simplificada de Machine Learning, de forma que não houve a necessidade do uso do Deep Learning.

3) Escolhida uma metodologia, os resultados de score e RMSE são aceitáveis ou teve overfitting/underfitting?
R- Algumas das metodologias testadas nesse projeto apresentaram overfitting e underfiting, contudo, isso não foi observado no caso do Gradient Boosting, ele manteve-se em bom desempenho e com RMSE entre os mais baixos testados. 

4) Supondo que a metodologia possui resultados aceitáveis, ela consegue indicar a importância das features (variáveis)?
R- O modelo de regressão por Gradient Boosting encontrado mostrou 5 features mais significatvas, de forma que foi possível analisar o comportamento de cada uma na série de dados.

5) Uma vez conhecidas as importâncias das features (variáveis), é possível fazer uma tomada de decisão para implementar políticas públicas?
R - Sim, foi possível fazer uma tomada de decisão e sugerir 3 políticas públicas distintas.

6) Uma vez sugeridas as políticas públicas, estas surgem para alterar alguma já existente ou são completamente novas? Além disso, são simples ou muito complexas para implementar? 
R- Numa busca simples, não foram encontradas políticas públicas de âmbito nacional, algumas vezes foram encontradas em âmbitos mais locais, de forma que as medidas parecem possuir viés diferente das econtradas localmente. Considerando as 3 propostas, 2 são de implementação mais simples e uma demanda estudo de viabilidade.

Após isto, podemos concluir então que sim, os métodos de Machine Learning foram extremamente úteis na busca de regredir os dados apresentados nas fontes de dados  utilizadas e o modelo encontrado nos trouxe features para serem analisadas e, com isto, foi possível uma tomada de decisão e sugestão de 3 distintas políticas públicas que visam melhorar a posição do Brasil no ranking do World Energy Trilemma.
~~~

# Trabalhos Futuros
~~~
Os trabalhos futuros podem se concentrar nos pontos críticos deste problema, de forma que poderiam incluir:

a) Análises com séries mensais e mais fontes de dados, que embora sejam mais difíceis de se conseguir,  trariam um banco de dados mais complexo e que consolidaria melhor o modelo de machine learning;

b) Comparativos com dados internacionais para uma análise de confiabilidade dos modelos de regressão;

c) Aplicação de técnicas de Deep Learning, para uma análise mais robusta de variáveis.
~~~

# Referências

[1] [Resultados do Procel:](http://www.procelinfo.com.br/main.asp?View={EC4300F8-43FE-4406-8281-08DDF478F35B}) (acesso em janeiro/2021);

[2] [Balanço Energético Nacional:](https://www.epe.gov.br/pt/publicacoes-dados-abertos/publicacoes/balanco-energetico-nacional-ben) (acesso em janeiro/2021);

[3] [Atlas da Eficiência Energética:](https://www.epe.gov.br/pt/publicacoes-dados-abertos/publicacoes/atlas-da-eficiencia-energetica-brasil-2019) (acesso em janeiro/2021);

[4] [Anuário Estatístico de Energia Elétrica:](https://www.epe.gov.br/pt/publicacoes-dados-abertos/publicacoes/anuario-estatistico-de-energia-eletrica) (acesso em janeiro/2021);

[5] [World Energy Trilemma Index:](https://www.worldenergy.org/publications?cat=69) (acesso em janeiro/2021);
