# Termo de Abertura do Projeto

## Histórico de Revisão

| Autor                                               | Mudanças                                                                                                                            | Data       | Versão |
| --------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------- | ------ |
| [Victor Buendia](https://github.com/Victor-Buendia) | Criação do documento; Adição de introdução, descrição do produto, objetivo do produto, e stakeholders.                              | 23/02/21   | 0.1    |
| [Victor Buendia](https://github.com/Victor-Buendia) | Criação da justificativa, produto do projeto, requisitos de alto nível, restrições do projeto, cronograma e marcos, e público alvo. | 24/02/21   | 0.2    |
| [Victor Buendia](https://github.com/Victor-Buendia) | Criação dos riscos iniciais, custos estimados e referências                                                                         | 25/02/21   | 0.3    |
| [Victor Buendia](https://github.com/Victor-Buendia) | Implementação de requisitos de alto nível, detalhamento dos riscos e ajustes gramaticais ao longo do texto                          | 26/02/2021 | 0.4    |

## Introdução

Este documento visa formalizar o início do projeto, agrupando todas as informações necessárias para a execução das atividades envolvidas.

## Descrição do Projeto

O **ECCOAR** é um sistema para moradores de comunidades públicas reportarem problemas em regiões próximas à sua localização a fim de facilitar a comunicação das demandas populacionais com órgãos públicos responsáveis.

## Justificativa

Tendo em vista que o Brasil é um país de tamanho geográfico continental, a ocupação urbana e rural do território nacional trouxe um desafio para o Governo Federal: realizar a manutenção e expansão desses espaços.

Com isso em mente, a articulação dos cidadãos torna-se fundamental para reportar problemas que ocorrem nas comunidades regionais. No entanto, atualmente os meios existentes para a denúncia dessas complicações acabam por ser desconhecidas e, muitas vezes, burocráticas.

Assim, por conta desse desafio, hoje tem-se visto um descaso e negligência por parte do poder público em resolver problemáticas das comunidades urbanas e rurais. Isso deve-se, em parte, pela falta de denúncia da população e, também, pela demora do governo em atuar nesses problemas.

Dessa maneira, o nosso sistema, chamado **ECCOAR** busca estabelecer uma forma de facilitar o reporte de problemas da comunidade do usuário por meio de uma ponte automatizada entre o governo público. Além disso, o sistema tem por finalidade agrupar as denúncias da comunidade dentro do aplicativo e o seu respectivo andamento de solução.

## Objetivo do Projeto

O objetivo do aplicativo **ECCOAR** é oferecer um sistema para regiões comunitárias a fim de engajá-la e facilitar na denúncia de problemas públicos com agente responsável sendo o governo. Assim, objetiva-se por _aumentar a visibilidade de problemáticas governamentais que afligem uma população local_ com o intuito de catalisar a resolução destas, alertando as instituições responsáveis, para melhorar a qualidade de vida dos cidadãos.

## Produto do Projeto

A proposta do projeto é de criar uma ferramenta na qual o usuário precise apenas fazer uma denúncia ou votar em denúncias já realizadas para que o sistema se encarregue de extrair as informações automaticamente e de gerar um relatório que é enviado para o órgão responsável.

O sistema também deverá armazenar essas denúncias para que o usuário possa realizar consultas nas denúncias comunitárias, votar em denúncias existentes, ver o andamento de resolução delas a fim de melhorar a qualidade de vida da comunidade.

## Requisitos de alto nível

Os requisitos de alto nível são funcionalidades escritas em linguagem natural ou ainda em forma de desenhos ou casos de uso, qualquer técnica que facilite o entendimento. Para o projeto em questão, tem-se os principais requisitos de alto nível:

- O usuário será capaz de criar uma conta, atualizá-la e deletá-la
- O usuário será capaz de criar, ler, atualizar e deletar denúncias
- O sistema permitirá votos em denúncias já existentes para aumentar sua relevância
- A aplicação enviará para o órgão responável um relatório das denúncias mais relevantes (com mais votos)
- O usuário poderá ver um mapa com as denúncias
- O sistema permitirá o comentário dos usuários em denúncias criadas por eles e outros
- A aplicação fechará as denúncias quando resolvidas pelo Estado

## Restrições do projeto

As restrições do presente projeto são:

- Aplicação dependente de conexão à internet para ser utilizada;
- Não há garantias de resolução da denúncia pelo Estado;
- A aplicação não faz uma ponte entre o governo e o usuário, mas sim se responsabiliza pela comunicação com o governo a partir da denúncia do usuário.

## Riscos iniciais

Durante a fase de iniciação do projeto, riscos foram levantados e serão rastreados continuamente, de forma que a equipe de gerência consiga prevenir, transferir, mitigar ou aceitá-los, para que o projeto ocorra sem atrasos ou grandes impedimentos que possam comprometê-lo ou até mesmo inviabilizá-lo.

### Riscos internos

- Indefinição de escopo

A indefinição de escopo é um risco que pode afligir a equipe na hora da execução, por causar ambiguidade naquilo que deve ser construído no que tangue à aplicação proposta.

- Incertezas com relação ao tema do projeto

Há algumas indeterminações no projeto que podem assolar o desenvolvimento dele, como qual instituição pública de cada região é a real responsável por determinado tipo de problema para ser contactada, como iremos contactá-la, dentre outros aspectos da proposta do produto.

- Membro faltante nas reuniões semanais

Um risco inerente à equipe diz respeito à ausência de integrantes do time em momentos síncronos de encontro virtual, uma vez que isso pode prejudicar o alinhamento pleno entre todos, dificultando o andamento fluido da execução das sprints.

- Divergência de horários dos membros

A pouca convergência de horários em comum dos membros é um risco que tensionará os colaboradores a buscarem a máxima performance de momentos síncronos, além de manter momentos assíncronos paulatinos ao decorrer do projeto. Esse desafio pode ocasionar atrasos dentro do projeto.

- Falta de integração entre a equipe

A pouca integração entre os membros do projeto pode diminui o nível de engajamento e, consequentemente, produtividade na hora de realizar as entregas no processo de desenvolvimento.

- Baixa produtividade dos integrantes da equipe

O cenário de baixa produtividade do time pode ocasionar atrasos nas iterações do projeto, além de interferir na qualidade das entregas dos membros.

- Dificuldade com tecnologias escolhidas

Um desafio eminente é a dificuldade com as tecnologias escolhidas, uma vez que parte do time de desenvolvedores (MDS) terá seu primeiro contato com elas na construção deste produto. Isso exigirá um alto grau de colaboração entre o time, especialmente no que tange ao auxílio dos membros gestores do projeto (EPS).

- Requisitos com alto nível de complexidade

A construção de _features_ de alto nível de complexidade pode causar desgaste nos membros e possíveis atrasos caso o domínio das tecnologias e engajamento no projeto não esteja em níveis adequados.

- Falta de tempo de integrantes da equipe

Observando a realidade dos integrantes para além da participação na construção desta aplicação, a maior parte possui uma carga de trabalho e estudos elevada, o que representa um risco para a execução do desenvolvimento do projeto. Isso porque exigirá um certo nível de organização e priorização da iniciativa para seu andamento fluido.

- Problemas com ambiente de desenvolvimento

O custo de aprendizado do uso dos ambientes de desenvolvimentos requeridos para o projeto e a resolução de problemas dentro dele podem causar atrasos nas entregas e desgaste do time.

- Falhas de comunicação

A comunicação ineficiente sobre prazos, expectativas das entregas e trabalho de cada um dos integrantes da equipe pode causar baixos padrões de entrega, refletidos em um constante retrabalho. Além disso, outra preocupação é o _delay_ desnecessário em atividades pontuais que precisam da contribuição dos participantes a fim de continuar o progresso do projeto.

### Riscos externos

- Pouca adesão ao uso do produto criado

O desconhecimento da plataforma, sua usabilidade e efetividade são fatores que influenciam diretamente no risco de tê-lo inutilizado pelo público alvo definido no processo de _Lean Inception_.

- Não garantia da resposta do governo às denúncias

A máquina do governo, por ter variabilidades regionais e estruturas robustas e, por vezes, lentas, podem ocasionar na não resposta do governo às denúncias reportadas na aplicação.

- Rejeição pelos órgãos públicos por inconformidade do relatório

Pelo teor formal e regulamentado dos órgãos públicos, um risco existente é a rejeição dos relatórios feitos pelo produto e enviados para a entidade responável por inconformidade do documento com as normas exigidas para a validação das denúncias.

- Enviar relatórios para órgãos não responsáveis pela denúncia em questão

Tendo em vista que o público alvo do produto são comunidades regionais, uma ameaça possível é a da aplicação não encaminhar os relatórios de denúncias para as instituições devidamente responsáveis pela resolução dos problemas referidos.

- Usabilidade baixa e burocratização da aplicação

A pouca intuitividade da aplicação e o seu intermédio com o governo pode representar para o usuário uma usabilidade baixa e alta burocratização do processo de denúncias de problemas públicos caso esses dois aspectos não sejam trabalhados bem dentro da proposta do produto.

O Scrum Master será o responsável por monitorar os riscos internos, e facilitar a adoção de medidas que mitiguem esses riscos, assim como o Product Owner será responsável por gerenciar os riscos externos. O controle é feito através das definições previstas na seção Gerenciamento de Riscos que pode ser encontrada [aqui](../metodologia/gerenciaRisco.md).

## Cronograma e marcos

| Marco             | Data                | Atividade                                                                                     |
| ----------------- | ------------------- | --------------------------------------------------------------------------------------------- |
| Início do projeto | 06/02/21            | Início da primeira Sprint do projeto                                                          |
| Release 01        | 21/03/21 - 27/03/21 | Primeira entrega de valor do projeto, que aborda os principais artefatos do início de projeto |
| Release 02        | 16/05/21 - 22/05/21 | Segunda entrega de valor, que aborda as funcionalidades definidas no escopo                   |

## Custo Estimado

Os custos estimados são para 15 sprints de projeto, ou seja, 15 semanas, totalizando 3 meses e 3 semanas de projeto.

### Pessoal

Utilizando como referência o site de busca de empregos **Glassdoor**, verificamos o salário de cada um dos papéis desempenhados pelo time.

| Papel na equipe | Quantidade de membros na função | Transporte e alimentação/dia | Salário/mês | Total por mês | Total no tempo do projeto |
| --------------- | ------------------------------- | ---------------------------- | ----------- | ------------- | ------------------------- |
| Desenvolvedor   | 6                               | R$0,00                       | R$2.772,00  | R$16.632,00   | R$66.528,00               |
| DevOps          | 1                               | R$0,00                       | R$11.000,00 | R$11.000,00   | R$44.000,00               |
| Product Owner   | 1                               | R$0,00                       | R$7.614,00  | R$7.614,00    | R$30.456,00               |
| Scrum Master    | 1                               | R$0,00                       | R$7.804,00  | R$7.804,00    | R$31.216,00               |
| Arquiteto       | 1                               | R$0,00                       | R$10.000,00 | R$10.000,00   | R$40.000,00               |
| Total           |                                 |                              |             | R$53.126,00   | R$212.200,00              |

Observações:

- Os valores pagos em transporte e alimentação são nulos porque o trabalho é desenvolvido remotamente de forma integral.

### Aquisições

Para o levantamento de custos foram considerados computadores com a especificação de um processador Intel Core i7, 1 TB de Espaço de Armazenamento, 8 GB de memória RAM e Windows 10, todos os notebooks da marca Lenovo com o [custo até o dia 25/02/2021](https://www.zoom.com.br/notebook/notebook-lenovo-ideapad-s145-intel-core-i7-8565u-15-6-8gb-hd-1-tb-geforce-mx110-windows-10?_lc=11#analise-do-especialista) de R$ 4.299,00.

| Produto  | Quantidade | Valor unitário | Valor absoluto |
| -------- | ---------- | -------------- | -------------- |
| Notebook | 10         | R$4.299,00     | R$42.990,00    |
| Total    |            |                | R$42.990,00    |

## Ferramentas

| Ferramentas                   | Descrição                                                                                                 | Valor    |
| ----------------------------- | --------------------------------------------------------------------------------------------------------- | -------- |
| ZenHub                        | Ferramenta de gerenciamento de projetos ágeis                                                             | R$0,00   |
| SonarCloud                    | Ferramenta de verificação de qualidade de código (valor da licença de 4 meses, até 100k linhas de código) | R$269,76 |
| Draw.io                       | Ferramenta para elaboração de diagramas                                                                   | R$0,00   |
| Git e GitHub                  | Ferramenta de versionamento de código                                                                     | R$0,00   |
| Telegram e Discord            | Ferramentas de comunicação do time                                                                        | R$0,00   |
| Docker                        | Ferramenta para criação de administração de ambientes isolados                                            | R$0,00   |
| Sistema operacional           | Ferramenta de uso para a construção da aplicação                                                          | R$0,00   |
| Editor de texto para o código | Ferramenta de editor de texto                                                                             | R$0,00   |
| Servidor                      | Serviço de computação em nuvem                                                                            | R$0,00   |
| Total                         |                                                                                                           | R$269,76 |

## Total

Fazendo um somatório de todos os gastos categorizados por tipo, chegamos na totalização abaixo:

| Tipo de custo | Valor        |
| ------------- | ------------ |
| Equipe        | R$212.200,00 |
| Aquisições    | R$42.990,00  |
| Ferramentas   | R$269,76     |
| Total         | R$255.459,76 |

## Stakeholders

### Público alvo

O projeto busca contemplar necessidades de comunidades regionais que tenham problemas de responsabilidade do poder público. Além disso, o governo torna-se uma parte interessada ao receber os relatórios com as informações de denúncia dos cidadãos.

### Equipe de apoio

Contemplada pelo professor da disciplina, o Professor Hilmer, agirá como _stakeholder_ do projeto auxiliando e avaliando os trabalhos realizados pela equipe de desenvolvimento e de gestão.

### Equipe de projeto

| Nome                                                | Papel         | Email                            |
| --------------------------------------------------- | ------------- | -------------------------------- |
| [Guilherme Rosa](https://github.com/guilhesme23)    | DevOps        | marquesguilherme3@gmail.com      |
| [Matheus Blanco](https://github.com/MatheusBlanco)  | Product Owner | msallesblanco@gmail.com          |
| [Pedro Féo](https://github.com/Phe0)                | Scrum Master  | pheofo@gmail.com                 |
| [Saleh Kader](https://github.com/devsalula)         | Arquiteto     | saleh.nazih.dev@gmail.com        |
| [Arthur Matos](https://github.com/Arthur-Matos)     | Desenvolvedor | git.arthurmatos@gmail.com        |
| [Brian Pina](https://github.com/DLBrianPina)        | Desenvolvedor | brian.pina2001@gmail.com         |
| [Gabriel Sabanai](https://github.com/Sabanai104)    | Desenvolvedor | gabrielsabanaitrindade@gmail.com |
| [Luiz Henrique](https://github.com/luiz-herique)    | Desenvolvedor | luizhemrique.fnandes@gmail.com   |
| [Nicolas Chagas](https://github.com/nszchagas)      | Desenvolvedor | nszchagas@gmail.com              |
| [Victor Buendia](https://github.com/Victor-Buendia) | Desenvolvedor | victorbuendia03@gmail.com        |

## Referências

Documentação Kalkuli, 2018. Página Termo de Abertura do Projeto. Disponível em: [https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/tap](https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/tap). Acesso em 23 de fevereiro de 2021.

Documentação QR Comer, 2019. Página Termo de Abertura do Projeto. Disponível em: [https://fga-desenho-2019-2.github.io/Wiki/seminario1/tap/](https://fga-desenho-2019-2.github.io/Wiki/seminario1/tap/). Acesso em 25 de fevereiro de 2021.

Glassdoor, © 2021. Página de busca de salários em determinadas regiões. Disponível em: [https://www.glassdoor.com.br/Sal%C3%A1rios/index.htm](https://www.glassdoor.com.br/Sal%C3%A1rios/index.htm). Acesso em 25 de fevereiro de 2021.

Zoom, © 2021. Página de busca de preços de produtos. Disponível em: [https://www.zoom.com.br/](https://www.zoom.com.br/). Acesso em 25 de fevereiro de 2021.
