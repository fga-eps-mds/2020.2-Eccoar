# Template Análise de dados

## Histórico de revisão

| Autor                                | Mudanças            | Data       | Versão |
| ------------------------------------ | ------------------- | ---------- | ------ |
| [Pedro Féo](https://github.com/phe0) | Criação do template | 07/05/2021 | 1.0    |

## Decisões tomadas

Esse é um espaço dedicado a explicar por que e quais decisões foram tomadas a partir das análises em cima das métricas de código.

## Aspectos de qualidade

Essa é a lista de aspectos de qualidade que serão avaliados pelo time. Esses aspectos foram selecionados com base nas métricas disponíveis para coleta da equipe.

### Manutenabilidade

O conjunto de métricas abaixo será coletado para avaliar a manutenabilidade do código do projeto. Tal aspecto é importante por nos permitir avaliar o quão fácil será para que manutenção seja feita no código.

#### Qualidade de código

##### Complexidade

- Pode ser obtido através do Sonarcloud e depois passar pela função disponível nesse [jupyter notebook](https://github.com/fga-eps-mds/Analytics/blob/main/analytics.ipynb);
- Ele é obtido pela quantidade de arquivos não complexos dividido pelo número total de arquivos;
- Um arquivo é considerado complexo se a complexidade ciclomática por função for maior qu 10;

##### Comentários

- Pode ser obtido através do Sonarcloud e depois passar pela função disponível nesse [jupyter notebook](https://github.com/fga-eps-mds/Analytics/blob/main/analytics.ipynb);
- É obtido pela quantidade de arquivos comentados dividido pelo número total de arquivos;
- Um arquivo é considerado comentado se a quantidade de linhas comentadas do arquivo estiver entre 10% e 30%;

##### Duplicações

- Pode ser obtido através do Sonarcloud e depois passar pela função disponível nesse [jupyter notebook](https://github.com/fga-eps-mds/Analytics/blob/main/analytics.ipynb);
- Pode ser calculado pelo número de arquivos com duplicação dividido pelo número total de arquivos;
- Um arquivo é considerado com duplicação se possuir mais de 5% de linhas duplicadas;

#### Blocking Code

##### Non-Blocking Files

- Pode ser obtido através do Sonarcloud e depois passar pela função disponível nesse [jupyter notebook](https://github.com/fga-eps-mds/Analytics/blob/main/analytics.ipynb);
- Pode ser calculado pela quantidade de arquivos com problemas de segurança dividido pelo número total e arquivos;

### Confiabilidade

A métrica abaixo será utilizada para calcular a confiabilidade do projeto. Esse aspecto é importante para avaliar o quão confiável o código é em realizar aquilo que propõe.

##### Sucesso nos testes

- Pode ser obtido através do Sonarcloud e depois passar pela função disponível nesse [jupyter notebook](https://github.com/fga-eps-mds/Analytics/blob/main/analytics.ipynb);
- Pode ser calculado com a quantidade de testes menos a quantidade de testes que falharam dividido pelo total de testes;

### Produtividade

Esse aspecto é responsável por avaliar a produtividade da equipe em realizar as tarefas propostas para concluir o projeto de software. Esse aspecto é avaliado principalmente nos documentos de review da sprint, como explica o [template](./review.md). Porém alguns dados tabém serão avaliados nesse documento.

##### THROUGHPUT

- Pode ser obtido através do zenhub do grupo;
- Pode ser calculdo pelo número de issues resolvidas dividido pelo número de issues em uma sprint;

##### ISSUE TYPE IN A TIMEFRAME

- Pode ser obtido através das issues do github e do zenhub;
- Os tipos de issues são classificadas através das tags de issue no github;
- Para calcular esse métrica se divide o número de issues de um tipo pela quantidade total de issues na sprint;

##### BUGS RATIO

- Pode ser obtido através das issues do github e do zenhub;
- Um bug é representado por uma issue que possua a tag bug;
- Para calcular essa métrica se divide o número de issues que são bugs pela quantidade de total de issues em uma sprint

## Referências

- Metric Definitions. Sonarqube. Disponível em <https://docs.sonarqube.org/latest/user-guide/metric-definitions/>. Acesso em 8 de maio de 2021.
- ISO 25000: software and data quality. Disponível em <https://iso25000.com/index.php/en/iso-25000-standards/iso-25010?start=0>. Acesso em 8 de maio de 2021.
- Choma, J. Guerra, E.M. and Silva, T.S. 2017. Patterns for Implementing Software Analytics in Development Teams. HILLSIDE Proc. of Conf. on Pattern Lang. of Prog. 24 de out. de 2017, 12 páginas.
- Silverio Martínez-Fernández, Anna Maria Vollmer, Andreas Jedlitschka, Xavier Franch, Lidia López, Prabhat Ram, Pilar Rodríguez Marín, Sanja Aaramaa, Alessandra Bagnato, Michal Choras, Jari Partanen: Continuously Assessing and Improving Software Quality With Software Analytics Tools: A Case Study. Acesso em 8 de maio de 2021.
