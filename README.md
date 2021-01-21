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
├── notebook           <- Colab notebooks do projeto.
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

[Gráficos](https://drive.google.com/drive/folders/1g0EYfwXQz58qNGoQRK2k9ZmvTaa0gvaa?usp=sharing): Todos os gráficos utilizados neste projeto;

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
[Projeto de IT305G](http://bit.ly/youtubeIT305G)

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
Considerando-se uma grande variedade nos valores das variáveis encontradas nos anuários utilizados como fontes de dados, não seria possível uma convergência válida para uma regressão não linear, assim, a metodologia mais adequda foi a normalização de dados, viabilizando o estudo científico e sua aplicação em Machine Learning. A partir disso, as análises seguiram o fluxo investigativo das pergguntas da pesquisa com vistas a uma tomada de decisão prática nas políticas públicas.   
~~~

# Recursos e Métodos

## Bases de Dados

Base de Dados | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
D1A | https://github.com/grnbatera/IT305G/blob/main/D1A.csv | `Dados sem modificação utilizados como base para o projeto`
D1An | https://github.com/grnbatera/IT305G/blob/main/D1An.csv | `Dados normalizados que de fato foram utilizados nos modelos de Machine Learning do projeto`

## Ferramentas

Ferramenta | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Regressão Multivariável | https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html | `Modelo de Regressão Multivariável utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Árvore de Decisão | https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeRegressor.html | `Modelo de Regressão por Árvore de Decisão utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Árvore de Decisão com AdaBoost | https://scikit-learn.org/stable/auto_examples/ensemble/plot_adaboost_regression.html# | `Modelo de Regressão por Árvore de Decisão com AdaBoost utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por AdaBoost | https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostRegressor.html | `Modelo de Regressão por AdaBoost utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por GradientBoosting | https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.GradientBoostingRegressor.html | `Modelo de Regressão por GradientBoosting utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Bagging | https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.BaggingRegressor.html | `Modelo de Regressão por Bagging utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Random Forest | https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html | `Modelo de Regressão por Random Forest utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`
Regressão por Support Vector Regressor | https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVR.html | `Modelo de Regressão por Support Vector Regressor utilizado para determinar as features mais importantes do banco de dados que ajudarão na tomada de decisão em políticas públicas`


# Metodologia
~~~
<Abordagem/metodologia adotada, incluindo especificação de quais técnicas foram exploradas, tais como: aprendizagem de máquina, análise de redes, análise estatística, ou integração de uma ou mais técnicas.>
~~~

## Detalhamento do Projeto
~~~
<Apresente aqui detalhes da análise. Nesta seção ou na seção de Resultados podem aparecer destaques de código como indicado a seguir. Note que foi usada uma técnica de highlight de código, que envolve colocar o nome da linguagem na abertura de um trecho com `~~~`, tal como `~~~python`.

Os destaques de código devem ser trechos pequenos de poucas linhas, que estejam diretamente ligados a alguma explicação. Não utilize trechos extensos de código. Se algum código funcionar online (tal como um Jupyter Notebook), aqui pode haver links. No caso do Jupyter, preferencialmente para o Binder abrindo diretamente o notebook em questão.>
~~~

~~~python
df = pd.read_excel("/content/drive/My Drive/Colab Notebooks/dataset.xlsx");
sns.set(color_codes=True);
sns.distplot(df.Hemoglobin);
plt.show();
~~~

## Evolução do Projeto
~~~
<Relate a evolução do projeto: possíveis problemas enfrentados e possíveis mudanças de trajetória. Relatar o processo para se alcançar os resultados é tão importante quanto os resultados.>
~~~

# Resultados e Discussão
~~~
<Apresente os resultados da forma mais rica possível, com gráficos e tabelas. Mesmo que o seu código rode online em um notebook, copie para esta parte a figura estática. A referência a código e links para execução online pode ser feita aqui ou na seção de detalhamento do projeto (o que for mais pertinente).

A discussão dos resultados também pode ser feita aqui na medida em que os resultados são apresentados ou em seção independente. Aspectos importantes a serem discutidos: É possível tirar conclusões dos resultados? Quais? Há indicações de direções para estudo? São necessários trabalhos mais profundos?>
~~~

# Conclusões
~~~
<Apresente aqui as conclusões finais do trabalho e as lições aprendidas.>
~~~

# Trabalhos Futuros
~~~
<Indique trabalhos futuros a partir do ponto alcançado.>
~~~
