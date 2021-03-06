# Documento de Arquitetura de Software

## Histórico de Revisão

|Autor|Mudanças|Data|Versão|
|--|--|--|--|
|[Brian Pina](https://github.com/DLBrianPina) e [Arthur Matos](https://github.com/Arthur-Matos)| Tópicos: 1.1, 1.2, 1.3 e 1.4 |03/03/2021|0.1|
|[Brian Pina](https://github.com/DLBrianPina), [Arthur Matos](https://github.com/Arthur-Matos) e <br/> [Gabriel Sabanai](https://github.com/Sabanai104)|Tópicos: 2.1 |03/03/2021|0.2|
|[Arthur Matos](https://github.com/Arthur-Matos), [Brian Pina](https://github.com/DLBrianPina) e <br/> [Gabriel Sabanai](https://github.com/Sabanai104)|Tópicos: 3, 4.1 |03/03/2021|0.3|
|[Brian Pina](https://github.com/DLBrianPina), [Arthur Matos](https://github.com/Arthur-Matos), <br/>[Gabriel Sabanai](https://github.com/Sabanai104) e [Saleh Kader](https://github.com/devsalula)|Tópicos: 3, 4.2 |05/03/2021|0.4|
|[Saleh Kader](https://github.com/devsalula)| Tópicos: 1.4, 4.2, 4.3 | 05/03/2021 | 05

## 1. Introdução

### 1.1 Finalidade

Este documento oferece uma visão geral arquitetural abrangente do sistema, usando diversas visões arquiteturais para representar os diferentes aspectos do sistema. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas em relação ao sistema.

### 1.2 Escopo

O Eccoar é um *Progressive Web App* (PWA)  que tem por objetivo ser a voz do cidadão em comunicar para as instituições governamentais sobre problemas em suas cidades.

Esse documento tem como objetivo representar as decisões arquiteturais do Eccoar, levando em conta as restrições impostas devido o contexto e visão da aplicação. Estão descritos neste documento especificações de tecnologia como linguagens, *frameworks* e padrões de projeto.

### 1.3 Definições, Acrônimos e Abreviações

* API: Application Programming Interface ou Interface de Programação de Aplicações é conjunto de definições e protocolos usado no desenvolvimento e na integração de software de aplicações.
* API Gateway: O *gateway* de API é uma ferramenta de gerenciamento de APIs que fica entre o cliente e uma coleção de serviços de *back end*.
* PWA: *Progressive Web App* são aplicações desenvolvidas para web que dão acesso a funcionalidades nativas, tendo como três pilares instabilidade, confiabilidade e capacidade.

### 1.4 Referências
> Parnas, D. L. On the Criteria To Be Used in Decomposing Systems into Modules. Comm. ACM (Dec., 1972) 1053-1056

> Documento de Arquitetura. Kalkuli, Brasília, Novembro de 2018. Disponível em: [https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/docArquitetura](https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/docArquitetura). Acesso em: 03 de Março de 2021

> Documento de Arquitetura. HubCare, Brasília, Abril de 2019. Disponível em: [https://cjjcastro.gitlab.io/2019-1-hubcare-docs/project/architecture-document/](https://cjjcastro.gitlab.io/2019-1-hubcare-docs/project/architecture-document/). Acesso em: 03 de Março de 2021

> O que é API? Red Hat. Disponível em: [https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces](https://www.redhat.com/pt-br/topics/api/what-are-application-programming-interfaces). Acesso em: 03 de Março de 2021

> Qual é a função de um gateway de API? Red Hat. Disponível em: [https://www.redhat.com/pt-br/topics/api/what-does-an-api-gateway-do](https://www.redhat.com/pt-br/topics/api/what-does-an-api-gateway-do). Acesso em: 03 de Março de 2021

> What Is React? ReactJs. Disponível em: [https://reactjs.org/tutorial/tutorial.html#what-is-react](https://reactjs.org/tutorial/tutorial.html#what-is-react). Acesso em: 03 de Março de 2021.

> Richard, S. LePage, P. What are Progressive Web Apps? web.dev. Janeiro de 2020. Disponível em: [https://web.dev/what-are-pwas/](https://web.dev/what-are-pwas/). Acesso em: 03 de Março de 2021.

> Naik, V. Architecting for Continuous Delivery. ThoughtWorks. Janeiro de 2016. Disponível em: [https://www.thoughtworks.com/pt/insights/blog/architecting-continuous-delivery](https://www.thoughtworks.com/pt/insights/blog/architecting-continuous-delivery). Acesso em: 03 de Março de 2021

> Valente, M. Engenharia de Software Moderna. Disponível em: [https://engsoftmoderna.info/cap7.html](https://engsoftmoderna.info/cap7.html). Acesso em: 03 de Março de 2021

> Fowler, M. Software Architecture Guide. MartinFowler. Agosto de 2019. Disponível em: [https://martinfowler.com/architecture/](https://martinfowler.com/architecture/). Acesso em: 03 de Março de 2021

> Fowler, M. MicroservicePrerequisites. MartinFowler. Agosto de 2014. Disponível em: [https://martinfowler.com/bliki/MicroservicePrerequisites.html](https://martinfowler.com/bliki/MicroservicePrerequisites.html). Acesso em: 03 de Março de 2021

> Fowler, M. Lewis, J. Microservice. MartinFowler. Março de 2014. Disponível em: [https://martinfowler.com/articles/microservices.html](https://martinfowler.com/articles/microservices.html). Acesso em: 03 de Março de 2021

## 2. Representação Arquitetural

* **ReactJS**: React é uma biblioteca de JavaScript flexível, declarativa e eficiente para construção de interfaces para exibição ao usuário. O React permite a criação desde interfaces complexas até pequenos e isolados pedaços de código chamados “componentes”.

* **NodeJS**: NodeJS é um software de código aberto que executa códigos Javascript no backend/servidor e no frontend. É baseado no interpretador de Javascript em C++ V8.

* **Typescript**: Typescript é um superconjunto de Javascript que insere na linguagem conceitos como tipagem estática, forte e inferida.

* **Redis**: Redis é um banco de dados em memória altamente performático com funciona com base em estruturas de chave-valor.

* **Microsserviços**: É uma abordagem arquitetônica e organizacional do desenvolvimento de software na qual consiste em pequenos serviços independentes, como módulos, que se comunicam usando API’'s. Dessa forma, os microsserviços facilitam a escalabilidade do software. Os microsserviços usados nesta aplicação são: 

    - **Módulo de Usuário**: Módulo responsável pelo registro e gerenciamento de usuários da aplicação;

    -  **Módulo de Denúncias**: Módulo responsável por relatar e armazenar as denúncias relacionadas aos posts dentro da aplicação ;

    - **Módulo de Email**: Módulo responsável pelo envio de email para as instituições governamentais;

    - **Módulo de Report**: Módulo responsável por gerar os relatórios das denúncias;

    - **Gateway**: Ponte entre a interação da interface do usuário com os microsserviços do back-end;

    - **Front-end**: Tela de interface do usuário por onde o mesmo vai interagir com a aplicação;

* **Service Worker**: Os services workers são extremamente importantes para a criação de PWA’s. Ele é um script no navegador que roda separado da página web, possibilitando recursos que não precisam da interação do usuário. Na prática ele é um script em javascript que controla a página do site na qual ele é associado.

* **Sass**: O Sass é uma linguagem de folha de estilo compilada para CSS, adicionando poder para a linguagem. Com o Sass é possível utilizar variáveis, regras de alinhamento, mixins, funções e várias outras funcionalidades.

![Documeto de arquitetura](../assets/img/produtos/docArquitetura.png)

## 3. Metas e Restrições da Arquitetura

São metas da arquitetura:

* Facilitação no processo de desenvolvimento.

* Acessibilidade para a maior parte da população.

* Independência no desenvolvimento das equipes.

* Alta mutabilidade em seus serviços.

* Clareza no desenvolvimento dos serviços.

São restrições da arquitetura:

* A aplicação deverá se comportar como um *Progressive Web App*;

* A aplicação necessita de ser executada nos navegadores Google Chrome, Mozilla Firefox e Safari;

## 4. Visão Lógica 

### 4.1 Visão Geral

A aplicação é baseada na arquitetura de microsserviços, com o intuito de facilitar o desenvolvimento como a escalabilidade do software. Dessa forma, cada microsserviço vai ser responsável por executar uma tarefa, uma requisição ou um processamento de dados, resultando assim, em uma implementação mais rápida com facilidade na sua manutenção.

### 4.2 Pacotes de Design Significativos do Ponto de Vista da Arquitetura

O *Back End* será construído por completo em cima da tecnologia *NodeJs*. No diagrama abaixo enxerga-se como será a estrutura básica de pacotes de um dos microsserviços.

![back](../assets/img/produtos/backArquitetura.png)

A aplicação no *Front End* será construído por completo em cima da tecnologia *ReactJs*. No diagrama abaixo enxerga-se como será a estrutura básica de pacotes do nosso PWA.

![front](../assets/img/produtos/front.png)

### 4.3 Visão de Dados

O Diagrama Entidade Relacionamento ficou da seguinte forma:

![Diagrama Entidade Relacionamento](../assets/img/produtos/DataModel.png)