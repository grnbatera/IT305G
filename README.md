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

### `external`

[Resultados do Procel](https://drive.google.com/drive/folders/1lXbcbY7AO2QKraQjPi9V74p87YyijNLu?usp=sharing): Fonte de dados contendo o desempenho do Brasil frente a Eficiência Energética e a prestação de contas do Procel;

[Balanço Energético Nacional](https://drive.google.com/drive/folders/1qC8e7uvXWioR11aF4E_RErYfV3_8sFTb?usp=sharing): Fonte de dados com a contabilização relativa à oferta e ao consumo de energia no Brasil, contemplando as atividades de extração de recursos energéticos primários, sua conversão em formas secundárias, importação e exportação, a distribuição e o uso final da energia;

[Anuário Estatítisco de Energia Elétrica](https://drive.google.com/drive/folders/11ri-E-GgCDF2cmAugMsTSBX7PH-5Ingr?usp=sharing): Fonte de dados onde são divulgados os dados detalhados relacionados ao consumo de energia elétrica na rede de distribuição;

[Atlas da Eficiência Energética](https://drive.google.com/drive/folders/1Tht_77lq2VXDvLFrLQJtgIHGYOuwEkG9?usp=sharing): Fonte de dados dos indicadores de Eficiência Energética;

[World Energy Trilemma](https://drive.google.com/drive/folders/1Zy2W9BlIaWLzoALv1s9b2YJpO2MkkIEK?usp=sharing): Fonte de dados com o Ranking Internacional e análise dos países com relação ao trilema de energia e sustentabilidade.

### `processed`

[D1An](https://github.com/grnbatera/IT305G/blob/main/D1An.csv): Dados das fontes externas unificadas e normalizadas para a utilização nos modelos de Regressão não linear em Machine Learning;

[Mapa de Variáveis](https://github.com/grnbatera/IT305G/blob/main/mapadevariaveisdeD1A.csv): Tabela contendo a descrição das variáveis de D1An utilizadas no projeto.

### `raw`

[D1A](https://github.com/grnbatera/IT305G/blob/main/D1An.csv): Dados das fontes externas unificadas com os valores originais para a utilização nos modelos de Regressão não linear em Machine Learning;

[Mapa de Variáveis](https://github.com/grnbatera/IT305G/blob/main/mapadevariaveisdeD1A.csv): Tabela contendo a descrição das variáveis de D1A utilizadas no projeto.


Dados utilizados no projeto respeitadas as possíveis implicações éticas, se você tiver licença para tal e se o volume for suportado pelo Github. Você pode optar por colocar um subconjunto ilustrativo dos dados.

É importante que sejam colocados os dados originais (se for possível) para garantir a reprodutibilidade do processo. Os originais são colocados na subpasta `raw` se forem produzidos pela equipe e na subpasta `external` se forem de terceiros. Também podem ser colocados aqui dados intermediários (por exemplo, dados tratados, resumidos etc.) na pasta `interim`. Finalmente, coloque os dados finais que serviram de entrada para as suas análises na subpasta `processed`.

## `notebooks`

Código do seu projeto que pode ser executado online sem instalação de software, tal como um notebook em Jupyter ou equivalente.

## `src`

Código em alguma linguagem ou projeto em Orange, Weka e similares.

Se for código em linguagem de programação, tente organizá-lo de forma que seja simples a sua execução por terceiros, por exemplo, acrescente as bibliotecas necessárias etc. Acrescente na raiz um arquivo `README.md` com as instruções básicas de instalação e execução.

## `assets`

Qualquer mídia usada no seu projeto: vídeo, ilustrações, arquivos PDF etc.

# Modelo para Apresentação do Projeto

Este é um guia de como produzir documentação em Markdown. Para entender como criar documentos em Markdown no Github, veja o material/vídeo:
[Guia de Uso do Markdown](https://github.com/mc-unicamp/oficinas/tree/master/docs).

Vide detalhes sobre o Markdown em: [Mastering Markdown](https://guides.github.com/features/mastering-markdown/).

E mais especificamente sobre tabelas em: [Organizing information with tables](https://help.github.com/en/articles/organizing-information-with-tables)

O projeto pode ser apresentado em uma das possíveis formas:
1. texto completo no arquivo `README.md`;
2. texto no arquivo `README.md` e seção de Resultados e Discussão dentro de um notebook Jupyter ou equivalente -- nesse caso, deve haver um link para se abrir o notebook na respectiva seção;
3. texto completo dentro de um notebook Jupyter ou equivalente -- nesse caso, o arquivo README.md deve conter pelo menos: o título, os componentes da equipe e um link para o notebook.

Só será aceito o uso de notebook Jupyter (ou equivalente) para apresentação do projeto ou parte dele (formas 2 e 3), se for possível executá-lo online a partir de um link sem instalação local de software.

Para todos os casos, a estrutura Markdown proposta abaixo poderá ser usada, dado que os notebooks aceitam Markdown.

Segue abaixo o modelo de como deve ser apresentado e documentado o projeto. Tudo o que for indicado entre `<...>` indica algo que deve ser substituído pelo indicado. No modelo são colocados exemplos ilustrativos, que serão substituídos pelos do seu projeto.

# Modelo para Apresentação do Projeto

# Projeto `<Título em Português>`
# Project `<Title in English>`

# Descrição Resumida do Projeto
~~~
<Descreva resumidamente o que fará o projeto. O resumo idealmente deve: apresentar o contexto; indicar o problema; apresentar a sua solução para o problema; indicar porque a sua solução é melhor do que os esforços atuais (não obrigatório); concluir com os resultados alcançados.>
~~~

# Abstract in English
~~~
<English version of the abstract.>
~~~

# Equipe
* `<nome completo>` - `<RA>`

# Vídeo do Projeto
`<coloque um link para o vídeo apresentado o projeto.>`

# Introdução e Motivação
~~~
<Descrição do tema do projeto, incluindo motivação, contexto gerador e caracterização do problema. A introdução também pode apresentar iniciativas correlatas para lidar com o problema (não obrigatório) e deve introduzir de forma mais detalhada que o resumo a solução proposta e resultados alcançados. Aqui também são apresentadas as seções do projeto.>
~~~

## Perguntas de Pesquisa
~~~
<Perguntas de pesquisa que o projeto pretende responder ou hipóteses a serem avaliadas, enunciadas de maneira objetiva e verificável.>
~~~

## Objetivos do projeto
~~~
<Como seu projeto propôs abordar o problema apresentado.>
~~~

# Recursos e Métodos

## Bases de Dados
`<Elencar bases de dados utilizadas no projeto preferencialmente no formato da tabela a seguir.>`
Base de Dados | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Base 1 | http://base1.org/ | `<Descrição da Base 1 e para que ela foi usada no projeto.>`
Base 2 | http://base2.org/ | `<Descrição da Base 2 e para que ela foi usada no projeto.>`

## Ferramentas

`<Elencar ferramentas utilizadas no projeto preferencialmente no formato da tabela a seguir.>`
Ferramenta | Endereço na Web | Resumo descritivo e uso
----- | ----- | -----
Ferramenta 1 | http://ferramenta1.org/ | `<Descrição da Ferramenta 1 e para que ela foi usada no projeto.>`
Ferramenta 2 | http://ferramenta2.org/ | `<Descrição da Ferramenta 2 e para que ela foi usada no projeto.>`

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
