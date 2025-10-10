**Clusterização de Clientes** 

**1\. Introdução**

Este projeto tem como objetivo aplicar técnicas de aprendizado de máquina não supervisionado para realizar a segmentação de clientes. A análise busca identificar padrões de comportamento no consumo e apoiar estratégias de marketing mais assertivas.

**2\. Problema resolvido**

Empresas muitas vezes não têm clareza sobre quem são seus melhores clientes, quais apresentam maior engajamento e quais possuem baixo potencial de consumo. Isso dificulta a definição de campanhas de marketing direcionadas e aumenta o custo de aquisição de clientes.

O problema abordado neste projeto foi justamente a identificação de diferentes perfis de clientes a partir de dados demográficos e de comportamento de consumo.

**3\. Modo de Resolução do Problema**

Foi realizada uma análise exploratória de dados (EDA) para compreender a distribuição das variáveis e identificar possíveis padrões. Após isso, foi aplicado o K-Means, um modelo estatístico amplamente utilizado em processos de segmentação de clientes. O problema em questão pertence à categoria de aprendizado não supervisionado, em que o modelo identifica automaticamente semelhanças entre os clientes e os agrupa em clusters.

A clusterização consiste em agrupar um conjunto de indivíduos de tal forma que aqueles que pertencem ao mesmo grupo apresentem maior similaridade entre si em comparação com os que estão em grupos diferentes. No caso deste projeto, a aplicação do K-Means tem como objetivo identificar a qual segmento cada cliente pertence, permitindo caracterizar diferentes perfis de comportamento.

Além disso, foi necessário definir o número ideal de clusters para representar os dados de forma significativa para o negócio. Para isso, foram utilizadas métricas e técnicas de validação de modelos, em especial a análise do Elbow Graph e a Silhouette Analysis, que auxiliaram na escolha da segmentação mais adequada.

**4\. Estrutura do projeto**

A estrutura do projeto foi organizada de acordo com o framework CRISP-DM (Cross Industry Standard Process for Data Mining), amplamente utilizado em projetos de ciência de dados. Dessa forma, a resolução do problema segue uma sequência de etapas bem definidas. Inicialmente, realizou-se a exploração dos dados, com o intuito de compreender a base disponível, identificar padrões e possíveis inconsistências. Em seguida, foi feita a preparação dos dados, aplicando os ajustes necessários para tornar o conjunto adequado ao treinamento dos modelos.

Na etapa seguinte ocorreu a construção do modelo, em que técnicas de clusterização, com destaque para o algoritmo K-Means, foram aplicadas para segmentar os clientes em grupos de interesse. Posteriormente, realizou-se a avaliação dos resultados, utilizando métricas e análises visuais, como o Elbow Graph e a Silhouette Analysis, para validar a quantidade de clusters mais apropriada e a qualidade da segmentação obtida. Por fim, a fase de deploy e conclusão concentrou-se na interpretação dos perfis de clientes gerados, bem como na definição de recomendações práticas que podem apoiar estratégias de marketing e tomada de decisão no negócio.

**5\. Tecnologias Utilizadas** 

As principais tecnologias utilizadas foram: 

* Pandas → usado para manipulação, limpeza e transformação dos dados em formato de tabelas (DataFrames).

* Numpy → utilizado para cálculos numéricos, operações vetoriais e matriciais de forma eficiente.

* Matplotlib / Pyplot → empregados na criação de gráficos básicos e personalizáveis   
* para análise de dados.

* Seaborn → usado para visualizações estatísticas mais elaboradas e intuitivas, facilitando a interpretação.

* Scipy → aplicado em operações estatísticas, funções matemáticas avançadas e suporte ao pré-processamento.

* Scikit-learn (Sklearn) → biblioteca principal para machine learning, aplicada aqui nos algoritmos de clusterização (K-Means, clusterização hierárquica) e métricas de avaliação.

* Yellowbrick → utilizado para gerar visualizações gráficas específicas de avaliação de modelos, como Elbow Method e Silhouette Analysis.

  

**6\. Resultados obtidos**

A partir das análises do Elbow Graph e Silhouette Analysis foi identificado que o melhor número de clusters é de 5 segmentos de clientes. 

Além disso, foi possível identificar características distintas e, com isso, chegar às seguintes conclusões sobre os diferentes segmentos de clientes da loja:

* Cluster 0 (40,5%): formado majoritariamente por mulheres, com idade média de 42 anos, renda média de 55k e score em torno de 49\. Representa o grupo regular, ou seja, clientes que compõem a maior parte da base.

* Cluster 1 (19,5%): composto em sua maioria por mulheres, com idade média de 32 anos, renda média elevada de 86k e score alto (82). É considerado um grupo de clientes estratégicos, com alto poder aquisitivo e forte engajamento.

* Cluster 2 (11,0%): também predominantemente feminino, formado por clientes mais jovens (25 anos), com renda baixa (26k), mas score elevado (79). Esse segmento reúne clientes em potencial, pois, apesar da baixa renda atual, demonstram grande propensão ao consumo.

* Cluster 3 (17,5%): grupo formado principalmente por homens, com idade média de 41 anos, renda média elevada (88k), porém score muito baixo (17). Apesar do poder de compra, o baixo engajamento torna esse segmento de baixa prioridade estratégica.

* Cluster 4 (11,5%): composto em sua maioria por mulheres mais velhas (45 anos), com renda média reduzida (28k) e score baixo (20). Esse perfil é pouco atrativo para estratégias de marketing, dado o baixo engajamento e a baixa capacidade de consumo.

