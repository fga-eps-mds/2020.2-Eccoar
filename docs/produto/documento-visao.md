# Documento de Visão

## Histórico de revisão

| Autor                                                                                             | Mudanças                                                           | Data       | Versão |
| ------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | ---------- | ------ |
| [Matheus Blanco](https://github.com/MatheusBlanco) e [Brian Pina](https://github.com/DLBrianPina) | Criação do documento e tópicos: 1.1, 1.2, 1.3, 1.4, 1.5, 1.6 e 3.4 | 22/02/2021 | 0.1    |
| [Matheus Blanco](https://github.com/MatheusBlanco) e [Brian Pina](https://github.com/DLBrianPina) | Tópicos: 2.1, 2.2 e 2.3                                            | 23/02/2021 | 0.2    |
| [Matheus Blanco](https://github.com/MatheusBlanco)                                                | Tópicos: 3.1, 3.2, 3.3, 3.4.2, 3.4.3, 3.5 e 3.6                    | 23/02/2021 | 0.3    |
| [Brian Pina](https://github.com/DLBrianPina)                                                      | Tópicos: 4.1, 4.2, 5.1, 5.2, 5.3, 5.4, 5.5 e 5.6                   | 25/02/2021 | 0.4    |
| [Matheus Blanco](https://github.com/MatheusBlanco)                                                | Arrumando tópicos requisitados em PullRequest Review               | 26/02/2021 | 0.5    |
| [Matheus Blanco](https://github.com/MatheusBlanco)                                                | Arrumando tópicos requisitados em PullRequest Review               | 26/02/2021 | 0.6    |

# 1. Introdução

## 1.1 Finalidade

Este documento tem como objetivo esclarecer e documentar as características e aplicações do desenvolvimento do projeto _Eccoar_.

## 1.2 Escopo

A partir de observações realizadas por membros da equipe, notou-se que em suas respectivas comunidades, o aparecimento de um problema muitas vezes não era seguido de sua solução, em um prazo alongado de tempo. Dito problema, que poderia ser um buraco na rua, falta de luz, e afins, costumava assolar a vivência em uma comunidade de maneira duradoura. Por quaisquer motivos o governo e os orgãos responsáveis não eram capazes de atender a todas as necessidades da região, ou demoravam-se extensamente para prover uma solução.

Essas observações, juntamente de uma pesquisa de viabilidade realizada por formulário, mostraram que há uma problemática em relação a não resolução de problemas em comunidades, algo que muitas vezes força os moradores a tomarem ação por si próprios. Entende-se que apesar de que nem todos os problemas de uma comunidade serem de responsabilidade do estado, muitos são e devem ser solucionados pelo mesmo. Dessa forma, o _software_ aqui documentado surge como uma proposta de solução para o relato e informação do estados sobre problemas existentes em comunidades.

O escopo do _Eccoar_ se encontra na criação e tratamento de denúncias de problemas a partir da visão dos próprios moradores de uma determinada comunidade do Distrito Federal. A partir do relato de um problema, fica a cargo da comunidade checar a veracidade do mesmo e, caso isso seja feito, um alerta será enviado para os orgãos responsáveis, pedindo pela tomada de ação dos mesmos. Após o envio do alerta, o _software_ também teria como escopo fornecer informações para seus usuários sobre progressos em relação ao problema.

## 1.3 Não Escopo

O _software_ previsto não tem a finalidade de se tornar uma rede social para relatos de problemas ou uma plataforma que instigue a comunidade a correr atrás da solução por conta própria, de forma que se posiciona a não ser uma solução garantida para problemas da comunidade.

Além disso, diferentemente de concorrentes, o _software_ não é destinado a ser usado por civis e autoridades em conjunto, mas sim apenas por civis e a comunicação com o governo e orgãos responsáveis ocorreria de maneira automatizada.

O _software_ também não possui fins lucrativos, sendo livre da existência de movimentação monetária entre os usuários e os desenvolvedores.

## 1.4 Definições, Acrônimos e Abreviações

- _Eccoar_ - Produto a ser criado para solucionar a temática anteriormente referenciada
- MDS - Métodos de Desenvolvimento de _Software_
- EPS - Engenharia de Produto de _Software_
- _Stakeholder_ - Partes interessadas na aplicação
- Comunidade - Grupo de pessoas que compartilham algo em comum, como uma história, objetivo e, no caso da comunidade de interesse deste projeto, uma determinada área geográfica.

## 1.5 Referências

IBM. Documento de Visão. [S. l.]. Disponível em: https://www.ibm.com/support/knowledgecenter/pt-br/SSWMEQ_4.0.6/com.ibm.rational.rrm.help.doc/topics/r_vision_doc.html. Acesso em: 22 fev. 2021.

KALKULI. Documento de Visão. [S. l.], 23 nov. 2018. Disponível em: https://fga-eps-mds.github.io/2018.2-Kalkuli/docs/docVisao. Acesso em: 22 fev. 2021.

[2] - LIXO acumulado por empresa provoca problemas no Bairro Ipiranga, em São José: Moradores estão preocupados com a sujeira, pois acumula água em pneus e vasos. [S. l.], 10 fev. 2021. Disponível em: https://www.nsctotal.com.br/noticias/lixo-acumulado-por-empresa-provoca-problemas-no-bairro-ipiranga-em-sao-jose. Acesso em: 23 fev. 2021.

## 1.6 Visão Geral

Este documento tem como visão fazer a documentação descritiva dos fundamentos, organização e desenvolvimento do _Eccoar_, bem como contextos levados a sua criação. Dessa maneira contempla a oportunidade de negócios com o problema em questão, exploração dos _stakeholders_ do projeto, visão macro dos requisitos e funcionalidades criadas e utilizadas pelo mesmo a fim de cumprir seu objetivo final.

# 2. Posicionamento

## 2.1 Oportunidade de negócios

Muitas vezes um problema aparece em uma comunidade carente, e permanece. Isso pode ocorrer por diversos motivos, sejam eles a falta de atenção da administração governamental local, a quantidade de problemas existentes ser maior do que o estado é capaz de lidar com, burocracias impedirem a resolução do mesmo.

A aplicação aqui descrita tem como objetivo tentar facilitar a resolução destes problemas mudando a maneira como os mesmos chegam ao conhecimento do estado. A partir da automatização de envio de informações e da contribuição dos moradores da comunidade em fazerem a fiscalização prévia e póstuma do problema, espera-se que a mesma possa contribuir com a diminuição do impacto negativo da situação descrita.

## 2.2 Descrição do problema

|                       |                                                                                                                                                                                                |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| O problema de         | Demora e burocracias na ação para resolução de situações pertinentes a vida em comunidades                                                                                                     |
| afeta                 | comunidades e seus moradores                                                                                                                                                                   |
| cujo impacto é        | diminuição da qualidade de vida em comunidade, da realização de possíveis atividades comerciais                                                                                                |
| uma boa solução seria | a automação de reportagens de ditos problemas para o estado, com a ação de moradores de ditas comunidades a partir da procura, verificação e acompanhamento dos problemas próximos aos mesmos. |

## 2.3 Sentença de Posição do Produto

|                   |                                                                                                                    |
| ----------------- | ------------------------------------------------------------------------------------------------------------------ |
| Para              | Comunidades e seus moradores                                                                                       |
| Cujo              | Problema se encontra na demora e burocracia na de resolução de problemas                                           |
| O _Eccoar_        | É um sistema de denúncias para problemas de natureza pública                                                       |
| Que               | Visa aumentar a visibilidade dos problemas e facilitar a comunicação entre o governo, orgãos responsáveis e o povo |
| Diferentemente do | Colab                                                                                                              |
| O nosso produto   | Coleta informações sobre o problema e os envia diretamente para o Estado, facilitando o relato de problemas        |

# 3. Descrição dos Envolvidos e dos Usuários

## 3.1 Resumo dos Envolvidos

| Nome                          | Descrição                                                                     | Responsabilidades                                                                                                                                         |
| ----------------------------- | ----------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Time de desenvolvimento       | Alunos da disciplina Métodos de Desenvolvimento de _Software_ da FGA UnB/Gama | Participar de atividades de capacitação e desenvolvimento do _software_ citado                                                                            |
| Time de gestão do projeto     | Alunos da disciplina Engenharia de Produto de _Software_ da FGA UnB/Gama      | Realizar o gerenciamento dos quesitos necessários para que o projeto ocorra de maneira flúida e eficiente, como escopo, prazos, riscos e princípios ágeis |
| Equipe de avaliação e suporte | Professor e Coaches das disciplinas de EPS e MDS                              | Auxiliar a equipe ao longo do desenvolvimento do projeto                                                                                                  |

## 3.2 Resumo dos Usuários

| Nome                            | Descrição                                                                                                                                                          | Responsabilidades                                                                                                           |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------- |
| Moradores de comunidades        | Pessoas que morem e estejam dentro de um raio específico de suas comunidades                                                                                       | Utilizar o sistema para apontar problemas em seus locais e regiões de moradia, além de acompanhar o progresso dos problemas |
| Funcionários de orgãos públicos | Pessoas que trabalham em determinados orgãos públicos e seriam responsáveis por receber as denúncias de problemas e procurar ações de resolução em cima das mesmas | Utilizar dos relatórios recebidos para procurar soluções devidas para os problemas relatados                                |

## 3.3 Ambiente do Usuário

A ser definido pós documento de arquitetura.

## 3.4 Perfis dos Envolvidos

### 3.4.1 Equipe de avaliação e suporte

Esperando mais informações do professor Hilmer.

### 3.4.2 Equipe de desenvolvimento

|                      |                                                                                                                                                                                                                                                                                                                            |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Representantes       | [Arthur Matos](https://github.com/Arthur-Matos) <br> [Brian Pina](https://github.com/DLBrianPina) <br> [Gabriel Sabanai](https://github.com/Sabanai104) <br> [Luiz Henrique](https://github.com/luiz-herique) <br> [Nicolas Chagas](https://github.com/nszchagas) <br> [Victor Buendia](https://github.com/Victor-Buendia) |
| Descrição            | Equipe responsável pelo desenvolvimento da aplicação                                                                                                                                                                                                                                                                       |
| Tipo                 | Estudantes de Métodos de Desenvolvimento de Software na Universidade de Brasília - FGA UnB/Gama, segundo semestre de 2020                                                                                                                                                                                                  |
| Responsabilidades    | Desenvolver                                                                                                                                                                                                                                                                                                                |
| Critérios de Sucesso | Entregar a aplicação, com os requisitos atendidos, dentro do prazo da disciplina                                                                                                                                                                                                                                           |
| Envolvimento         | Alto                                                                                                                                                                                                                                                                                                                       |

### 3.4.3 Equipe de gestão do projeto

|                      |                                                                                                                                                                                                     |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Representantes       | [Guilherme Rosa](https://github.com/guilhesme23) <br> [Matheus Blanco](https://github.com/MatheusBlanco) <br> [Pedro Féo](https://github.com/Phe0) <br> [Saleh Kader](https://github.com/devsalula) |
| Descrição            | Equipe responsável pelo gerenciamento da aplicação                                                                                                                                                  |
| Tipo                 | Estudantes de Engenharia de Produto de Software na Universidade de Brasília - FGA UnB/Gama, segundo semestre de 2020                                                                                |
| Responsabilidades    | Gerenciar tempo, escopo, risco e realizar tomadas de decisões para garantir a viabilidade do projeto, garantindo a utilização e eficiência dos princípios ágeis                                     |
| Critérios de Sucesso | Manter o engajamento e eficiência dos times alto e constante, para fins de entregar o software a tempo e com qualidade                                                                              |
| Envolvimento         | Alto                                                                                                                                                                                                |

## 3.5 Perfis dos usuários

### 3.5.1 Moradores de comunidades

|                       |                                                                                                                                                                                              |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Representante         | -                                                                                                                                                                                            |
| Descrição             | Pessoas que moram em comunidades (bairros, regiões administrativas, condomínios) e estão passando por algum problema que ainda não foi resolvido pelo governo e/ou pelos orgãos responsáveis |
| Tipo                  | Usuários com baixo ou médio conhecimento técnico                                                                                                                                             |
| Responsabilidades     | Reportar problemas em suas redondezas no sistema, além de motivar seus vizinhos a fazerem o mesmo e/ou verificarem e acompanharem a veracidade e progresso do problema                       |
| Critérios de sucesso  | O sistema deverá ser capaz de mostrar apenas os problemas existentes em um raio de até **X** quilômetros da localização do usuário, além de mostrar atualizações sobre o problema            |
| Comentários/Problemas | Desafio de engajar-se e engajar vizinhos a participarem da iniciativa.                                                                                                                       |

## 3.6 Principais necessidades dos usuários ou dos envolvidos

| Necessidade                                                                                | Prioridade | Preocupações                                                                      | Solução atual                                                                                                                                                                                                | Soluções propostas                                                                                                                                 |
| ------------------------------------------------------------------------------------------ | ---------- | --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| Poder levar uma vida de qualidade sem ter que lidar com problemas em seu local de convívio | Alta       | Não terem seus problemas visíveis e resolvidos pelo governo e orgãos responsáveis | COLAB, plataforma de reportagen de problemas utilizada pelos governos, orgãos responsáveis e população, Redes sociais, plataformas de comunicação que acabam sendo utilizadas para visibilidade de problemas | Automatizar o contato entre o governo, orgãos responsáveis e a população a partir do envio de informações sobre os problemas de maneira automática |

## 3.7 Alternativas e Concorrências

# 4. Visão geral do produto

## 4.1 Perspectiva do produto

O sistema tem como objetivo facilitar o processo de denúncia de problemas de natureza pública para o governo e para orgãos responsáveis. O usuário poderá registrar as próprias denúncias ou suportar as denúncias de outros usuários. A aplicação realizará o encaminhamento automático para as autoridades responsáveis.

## 4.2 Resumo dos recursos

| Benefício para o cliente   | Recursos de suporte                                                                                        |
| -------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Denúncia de problema       | O usuário pode descrever o seu problema e reportá-lo para as autoridades competentes                       |
| Suporte à denúncia         | O usuário pode oferecer suporte para denúncias de outros usuários em forma de votos de apoio e comentários |
| Acompanhamento da denúncia | O usuário pode acompanhar o andamento da denúncia realizada por ele através de uma auditoria civil         |

# 5. Recursos do produto

## 5.1 Acesso

O usuário deve ser capaz de acessar a plataforma através de autenticação por login.

## 5.2 Cadastro

O usuário deve ser capaz de realizar o cadastro através da própria aplicação.

## 5.3 Submissão de denúncia

O usuário deve ser capaz de denunciar um problema de natureza pública para as autoridades responsáveis.

## 5.4 Apoio a denúncia

O usuário deve ser capaz de fornecer apoio para denúncias criadas por outros usuários na forma de votos de apoio e comentários.

## 5.5 Acompanhar a denúncia

O usuário deve ser capaz de acompanhar o andamento das denúncias que ele criou e apoiou.

## 5.6 Acionamento das autoridades

As mensagens devem ser enviadas para as autoridades competentes assim que chegarem a um certo nível de relevância.
