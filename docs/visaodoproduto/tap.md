# Termo de Abertura do Projeto
## Histórico de Revisão
|Data|Versão|Descrição|Autor|
|--|--|--|--|
|23/02/21|0.1|Criação do documento; Adição de introdução, descrição do produto, objetivo do produto, e stakeholders.|Victor Buendia|
|24/02/21|0.2|Criação da justificativa, produto do projeto, requisitos de alto nível, restrições do projeto, cronograma e marcos, e público alvo.|Victor Buendia|
|25/02/21|0.3|Criação dos riscos iniciais, custos estimados e referências|Victor Buendia|

## Introdução
Este documento visa formalizar o início do projeto, agrupando todas as informações necessárias para a execução das atividades envolvidas.

## Descrição do Projeto
O **ComUnidas** é um sistema para moradores de comunidades públicas reportarem problemas em regiões próximas à sua geolocalização a fim de facilitar a comunicação das demandas populacionais com órgãos públicos responsáveis.

## Justificativa
Tendo em vista que o Brasil é um país de tamanho geográfico continental, a ocupação urbana e rural do território nacional trouxe um desafio para o Governo Federal: realizar a manutenção e expansão desses espaços.

Com isso em mente, a articulação dos cidadãos torna-se fundamental para reportar problemas que ocorrem nas comunidades regionais. No entanto, atualmente os meios existentes para a denúncia dessas complicações acabam por ser desconhecidas e, muitas vezes, burocráticas.

Assim, por conta desse desafio, hoje tem-se visto um descaso e negligência por parte do poder público em resolver problemáticas das comunidades urbanas e rurais. Isso deve-se, em parte, pela falta de denúncia da população e, também, pela demora do governo em atuar nesses problemas.

Dessa maneira, o nosso sistema, chamado **ComUnidas** busca estabelecer uma forma de facilitar a reportagem de problemas da comunidade do usuário por meio de uma ponte automatizada entre o governo público. Além disso, o sistema tem por finalidade agrupar as denúncias da comunidade dentro do aplicativo e o seu respectivo andamento de solução. 

## Objetivo do Projeto
O objetivo do aplicativo **ComUnidas** é oferecer um sistema para regiões comunitárias a fim de engajá-la e facilitar na denúncia de problemas públicos com agente responsável sendo o governo. Assim, objetiva-se por *aumentar a visibilidade de problemáticas governamentais que afligem uma população local* com o intuito de catalisar a resolução destas, alertando o Estado diretamente, para melhorar a qualidade de vida dos cidadãos.

## Produto do Projeto
A proposta do projeto é de criar uma ferramenta na qual o usuário precise apenas fazer uma denúncia ou votar em denúncias já realizadas para que o sistema se encarregue de extrair as informações automaticamente e de gerar um relatório que é enviado para o órgão responsável.

O sistema também deverá armazenar essas denúncias para que o usuário possa realizar consultas nas denúncias comunitárias, votar em denúncias existentes, ver o andamento de resolução delas a fim de melhorar a qualidade de vida da comunidade.

## Requisitos de alto nível
Ainda não há dados a respeito.

## Restrições do projeto
As restrições do presente projeto são:

- Aplicação dependente de conexão à internet para ser utilizada;
- Não há garantias de resolução da denúncia pelo Estado;
- A aplicação não faz uma ponte entre o governo e o usuário, mas sim se responsabiliza pela comunicação com o governo a partir da denúncia do usuário.

## Riscos iniciais
Durante a fase de iniciação do projeto, riscos foram levantados e serão rastreados continuamente, de forma que a equipe de gerência consiga prevenir, transferir, mitigar ou aceitá-los, para que o projeto ocorra sem atrasos ou grandes impedimentos que possam comprometê-lo ou até mesmo inviabilizá-lo.

### Riscos internos
- Indefinição de escopo
- Incertezas com relação ao tema do projeto
- Membro faltante nas reuniões semanais
- Divergência de horários dos membros
- Falta de integração entre a equipe
- Baixa produtividade dos integrantes da equipe
- Dificuldade com tecnologias escolhidas
- Requisitos com alto nível de complexidade
- Falta de tempo de integrantes da equipe
- Problemas com ambiente de desenvolvimento
- Falhas de comunicação

### Riscos externos
- Pouca adesão ao uso do produto criado
- Não garantia da resposta do governo às denúncias
- Rejeição pelos órgãos públicos por inconformidade do relatório
- Enviar relatórios para órgãos não responsáveis pela denúncia em questão
- Usabilidade baixa e burocratização da aplicação

O Scrum Master será o responsável por monitorar os riscos internos, e facilitar a adoção de medidas que mitiguem esses riscos, assim como o Product Owner será responsável por gerenciar os riscos externos. O controle é feito através das definições previstas na seção Gerenciamento de Riscos que pode ser encontrada [aqui](../metodologia/gerenciaRisco.md).

## Cronograma e marcos
|Marco|Data|Atividade|
|--|--|--|
|Início do projeto|06/02/21|Início da primeira Sprint do projeto|
|Release 01|21/03/21 - 27/03/21|Primeira entrega de valor do projeto, que aborda os principais artefatos do início de projeto|
|Release 02|16/05/21 - 22/05/21|Segunda entrega de valor, que aborda as funcionalidades definidas no escopo|

## Custo Estimado
Os custos estimados são para 15 sprints de projeto, ou seja, 15 semanas, totalizando 3 meses e 3 semanas de projeto.

### Pessoal
Utilizando como referência o site de busca de empregos **Glassdoor**, verificamos o salário de cada um dos papéis desempenhados pelo time.

|Papel na equipe|Quantidade de membros na função|Transporte e alimentação/dia|Salário/mês|Total|
|--|--|--|--|--|
|Desenvolvedor|6|R$0,00|R$2.772,00|R$16.632,00|
|DevOps|1|R$0,00|R$11.000,00|R$11.000,00|
|Product Owner|1|R$0,00|R$7.549,00|R$7.549,00|
|Scrum Master|1|R$0,00|R$7.945,00|R$7.945,00|
|Arquiteto|1|R$0,00|R$10.000,00|R$10.000,00|
|Total|||||R$53.126,00|

Observações:
- Os valores pagos em transporte e alimentação são nulos porque o trabalho é desenvolvido remotamente de forma integral.

### Aquisições
Para o levantamento de custos foram considerados computadores com a especificação de um processador Intel Core i7, 1 TB de Espaço de Armazenamento, 8 GB de memória RAM e Windows 10, todos os notebooks da marca Lenovo com o [custo até o dia 25/02/2021](https://www.zoom.com.br/notebook/notebook-lenovo-ideapad-s145-intel-core-i7-8565u-15-6-8gb-hd-1-tb-geforce-mx110-windows-10?_lc=11#analise-do-especialista) de R$ 4.299,00.

|Produto|Quantidade|Valor unitário|Valor absoluto|
|--|--|--|--|
|Notebook|10|R$4.299,00|R$42.990,00|
|Total|||R$42.990,00|

## Ferramentas
|Ferramentas|Descrição|Valor|
|--|--|--|
|ZenHub|Ferramenta de gerenciamento de projetos ágeis|R$0,00|
|SonarCloud|Ferramenta de verificação de qualidade de código|R$0,00|
|Draw.io|Ferramenta para elaboração de diagramas|R$0,00|
|Git e GitHub|Ferramenta de versionamento de código|R$0,00|
|Telegram e Discord|Ferramentas de comunicação do time|R$0,00|
|Docker|Ferramenta para criação de administração de ambientes isolados|R$0,00|
|Sistema operacional|Ferramenta de uso para a construção da aplicação|R$0,00|
|Editor de texto para o código|Ferramenta de editor de texto|R$0,00|
|Servidor|Serviço de computação em nuvem|R$0,00|
|Total||R$0,00|

## Total
Fazendo um somatório de todos os gastos categorizados por tipo, chegamos na totalização abaixo:

|Tipo de custo|Valor|
|--|--|
|Equipe|R$53.126,00|
|Aquisições|R$42.990,00|
|Ferramentas|R$0,00|
|Total|R$96.116,00|

## Stakeholders
### Público alvo
O projeto busca contemplar necessidades de comunidades regionais que tenham problemas de responsabilidade do poder público. Além disso, o governo torna-se uma parte interessada ao receber os relatórios com as informações de denúncia dos cidadãos.

### Equipe
|Nome|Papel|Email|
|--|--|--|
|[Guilherme Rosa](https://github.com/guilhesme23)|DevOps|marquesguilherme3@gmail.com|
|[Matheus Blanco](https://github.com/MatheusBlanco)|Product Owner|msallesblanco@gmail.com|
|[Pedro Féo](https://github.com/Phe0)|Scrum Master|pheofo@gmail.com|
|[Saleh Kader](https://github.com/devsalula)|Arquiteto|saleh.nazih.dev@gmail.com|
|[Arthur Matos](https://github.com/Arthur-Matos)|Desenvolvedor|git.arthurmatos@gmail.com|
|[Brian Pina](https://github.com/DLBrianPina)|Desenvolvedor|brian.pina2001@gmail.com|
|[Gabriel Sabanai](https://github.com/Sabanai104)|Desenvolvedor|gabrielsabanaitrindade@gmail.com |
|[Luiz Henrique](https://github.com/luiz-herique)|Desenvolvedor|luizhemrique.fnandes@gmail.com|
|[Nicolas Chagas](https://github.com/nszchagas)|Desenvolvedor|nszchagas@gmail.com|
|[Victor Buendia](https://github.com/Victor-Buendia)|Desenvolvedor|victorbuendia03@gmail.com|

## Referências
Documentação Kalkuli, 2018. Página Termo de Abertura do Projeto. Disponível em: [https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/tap](https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/tap). Acesso em 23 de fevereiro de 2021.

Documentação QR Comer, 2019. Página Termo de Abertura do Projeto. Disponível em: [https://fga-desenho-2019-2.github.io/Wiki/seminario1/tap/](https://fga-desenho-2019-2.github.io/Wiki/seminario1/tap/). Acesso em 25 de fevereiro de 2021.

Glassdoor, © 2021. Página de busca de salários em determinadas regiões. Disponível em: [https://www.glassdoor.com.br/Sal%C3%A1rios/index.htm](https://www.glassdoor.com.br/Sal%C3%A1rios/index.htm). Acesso em 25 de fevereiro de 2021.

Zoom, © 2021. Página de busca de preços de produtos. Disponível em: [https://www.zoom.com.br/](https://www.zoom.com.br/). Acesso em 25 de fevereiro de 2021.