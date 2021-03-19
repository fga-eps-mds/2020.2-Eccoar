# Rastro do Processo de Construção da Arquitetura

## Histórico de Revisão

|Autor|Mudanças|Data|Versão|
|--|--|--|--|
|[Saleh Kader](https://github.com/devsalula)| Tópicos: 1.0, 2.0, 3.0, 4.0 |19/03/2021|0.1|

## 1. Introdução

O presente documento, tem por finalidade apresentar todo o conteúdo e referências coletadas para a construção da Arquitetura do Projeto Eccoar. Esse documento não é a mesma coisa que o [documento de arquitetura](./documento-arquitetura.md), sendo apenas responsável por rastrear o processo anterior a construção da Arquitetura do Projeto Eccoar.

## 2. Pré-Construção e Critérios

Para a definição arquitetural do projeto foram levadas em consideração 3 principais stakeholders:

* Professor e Interessados da Disciplina de MDS/EPS.
* Desenvolvedores do Projeto Eccoar;
* Possíveis Clientes/Usuários do Projeto Eccoar;

Tendo isso em vista, foram retirados de cada stakeholder critérios de aceitação da arquitetura e a partir delas foram criadas regras para poder atender as necessidades de cada um. Os critérios retirados de cada stakeholder foram:

|Stakeholder|Critério|
|-----------|--------|
|Professor e Interessados da Disciplina|Utilizar de uma Arquitetura que <br />permita a independência do desenvolvimento de funcionalidades do projeto.
|Desenvolvedores do Projeto Eccoar|Ter contato com desenvolvimento de software, aprendendo novas tecnologias e padrões de desenvolvimento.
|Possíveis Clientes/Usuário do Projeto|Conseguir denunciar os problemas em sua região com o objetivo que elas alcancem as instâncias governamentais.

Com esses critérios levantados, analisamos o [Lean Inception](../lean-inception.md) de onde retiramos o nosso *backlog* do produto e listamos as nossas funcionalidades. Isso aconteceu devido a importância da preocupação da arquitetura a nível empresarial aliada a arquitetura técnica, afim de alinhar toda camada técnica com a camada de negócios do projeto.

## 3. Processo de Levantamento de Referências

Tendo os critérios levantados e *backlog* levantados, iniciou-se uma processo massivo de levantamento de referências e pesquisas para compreender qual é o melhor padrão arquitetural para a construção do projeto. O melhor estilo não vai ser discutido nesse documento, já que possuímos um [documento de arquitetura](./documento-arquitetura.md) para discutir esse assunto. O objetivo aqui é apenas apresentar as referências consultadas.

Como dentro da disciplina temos como critérios criar uma arquitetura que possibilite o desenvolvimento de funcionalidades de maneira independente e consequentemente não criando gargalos para a entrega contínua, foi consultado o professor sobre referências na área de modularização de projetos de software. O Professor prontamente compartilhou conosco um *paper* do autor David Parnas.

O Parnas em seu artigo ele demonstra que as tomadas de decisões para modularização baseadas no *design* do sistema são muito mais eficazes que as decisões orientadas a um fluxograma. Tendo isso em vista enxergamos que a modelagem dos dados do projeto seriam uma decisão baseada diretamente no nosso design e então partimos para essa construção.

A modelagem de dados nos forneceu a possibilidade de enxergar alguns módulos que consequentemente nos levou a aceitar na arquitetura de microsserviços dentro do *Backend*. Olhando para o livro Engenharia de Software Moderna do Marcos Tulio Valente, começamos a modelar os nossos microsserviços separando dois bancos de dados principais um para um serviço de Usuários e outro para o serviço de Denúncias. Não ficamos restritos apenas a esses dois serviços e partir de um artigo de Guia de Microsserviços do Martin Fowler utilizamos do nosso *backlog* para levantar mais alguns serviços dentro do projeto.

No final, observamos a necessidade de alinhar tudo isso a entrega contínua onde enxergamos que o *Front* estava com características monolíticas. Por isso, no *Frontend* começamos a pesquisar formas de modularizar a sua arquitetura e a partir dessas pesquisas encontramos um artigo do Pete Hodgson no blog do Martin Fowler, sobre *Feature Toggles*, que é uma técnica muito poderosa para poder modificar sistemas sem ter a necessidade de modificar o código e oferecendo a possibilidade de realizar *Canary Releases* e também realizar Testes A/B. 


## 4. Referências
> Fowler, M. Software Architecture Guide. MartinFowler. Agosto de 2019. Disponível em: [https://martinfowler.com/architecture/](https://martinfowler.com/architecture/). Acesso em: 19 de Março de 2021

> Parnas, D. L. On the Criteria To Be Used in Decomposing Systems into Modules. Comm. ACM (Dec., 1972) 1053-1056

> Valente, M. Engenharia de Software Moderna. Disponível em: [https://engsoftmoderna.info/cap7.html](https://engsoftmoderna.info/cap7.html). Acesso em: 19 de Março de 2021

> Hodgson, Pete. Feature Toggles. MartinFowler. Outubro de 2017. Disponível em: [https://martinfowler.com/articles/feature-toggles.html](https://martinfowler.com/articles/feature-toggles.html). Acesso em: 19 de Março de 2021