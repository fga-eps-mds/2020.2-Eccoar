# Earned Value Management

## Histórico de revisão

| Autor                                              | Mudanças                                   | Data       | Versão |
| -------------------------------------------------- | ------------------------------------------ | ---------- | ------ |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Criação do documento                       | 13/03/2021 | 1.0    |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Adição da tabela e explicação das fórmulas | 13/03/2021 | 2.0    |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Ajuste dos valores de custo                | 21/03/2021 | 3.0    |

## 1. Introdução

A técnica de mensuração _Earned Value Management_ é amplamente utilizada por gerentes de projeto, por ser capaz de integrar a definição de recursos, escopo e de cronograma, de um determinado projeto, de maneira a medir regularmente o progresso de dito projeto, mostrando valores monetários relativos a essa medição para a facilitação do entendimento.

O EVM é calculado em uma série de etapas que comprimem a relação de custos, a quantidade de progresso alcançado em determinado período de tempo e o valor planejado a ser definido pelo time e pelo escopo. São os valores:

- Valor planejado (PV);
- Custo atual (AC);
- Valor agregado (EV);

A tabela de EVM da equipe encontra-se [aqui](https://docs.google.com/spreadsheets/d/1dIPz4ku9tcfeAwUH-QSNfKg3fyFHK_nozA9CRUzxwNs/edit?usp=sharing).

<iframe src="https://docs.google.com/spreadsheets/d/1dIPz4ku9tcfeAwUH-QSNfKg3fyFHK_nozA9CRUzxwNs/edit?usp=sharing" frameborder="0" width="960" height="569" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

## Valor planejado (PV)

O valor planejado de um projeto se refere ao custo total do mesmo em determinado período de tempo, levando em consideração o BAC, valor total de custos calculado para o projeto. O BAC deste projeto foi calculado de acordo com custos de ferramentas, salário de membros envolvidos e de equipamentos necessitados para que os mesmos pudessem produzir. Tais valores encontram-se melhor detalhados no [Termo de Abertura de Projeto](./tap.md), e se resume no valor de **R$ 133.520,96**.

A partir do cálculo do BAC, pode-se calculcar o PV dividindo-se o BAC na quantidade de checkpoints existentes no projeto (_sprints_), e atribuindo-se a cada uma das _sprints_ um valor parcelado do BAC. Normalmente divide-se o BAC pelo número de _sprints_ e atribui-se este valor a cada uma delas.

Utilizando-se então da fórmula **PV = % completado(planejado) \* BAC**, pode-se alcançar o valor do PV alcançado até determinado ponto do projeto.

Ex: Se o projeto dura 4 meses, o BAC é de **R$ 133.520,96**, e dois meses se passaram, com 75% de completude, o PV seria = 75% \* **R$ 133.520,96**.

## Custo Atual (AC)

O AC representa os custos atuais utilizados para se completar determinada porcentagem do projeto. Seu resultado final nos mostra o valor que foi gasto pela equipe para completar uma quantidade X de sprints, Histórias de Usuário, ou ter alcançado um determinado checkpoint do projeto. Não tem uma fórmula fixa pois é o representado diretamente pelos gastos atuais do projeto.

## Valor Agregado (EV)

O EV representa o valor criado até determinado momento do projeto. Se o mesmo for parado, por exemplo, depois de dois meses, o EV irá mostrar para o cliente o valor gerado com o progresso do projeto.

Sua fórmula é: **EV = % completado(atual) \* BAC**.

Ex: Se o projeto dura 4 meses, o BAC é de **R$ 133.520,96**, e dois meses se passaram, com 75% de completude e **R$ 50.000,00** foram gastos, o EV seria = 75% \* **R$ 133.520,96,76** = **R$ 100.140,72**. O projeto então vale mais do que o que foi gasto atualmente.

## Outros índices de cálculo

Além dos três valores principais, existem variações que podem ser calculadas a partir de seus resultados e devem ser medidas por _sprint_. Estas variações são:

**Variação de Cronograma (SV)**, que indica a variação entre a quantidade de trabalho realizado e a quantidade de trabalho a ser feita. Sua fórmula envolve valor planejado e valor agregado (**SV = EV - PV**), e seu resultado deve ser analisado em questão de positividade, quando o projeto está adiantado, neutralidade, quando o projeto está no tempo esperado, e negatividade, quando o projeto está atrasado.

**Variação de Custo (CV)**, que indica a diferença entre a o custo planejado e o custo atual do projeto (**CV = EV - AC**), e seu resultado deve ser analisado em questão de positividade, quando o projeto está abaixo do orçamento, neutralidade, quando o projeto está no orçamento esperado, e negatividade, quando o projeto estourou o orçamento.

**Índice de perfomance por cronograma (SPI)**, que mostra o progresso do projeto em relação ao seu cronograma. É representado pela fórmula **SPI = EV/PV**, e seu resultado deve ser analisado:

- Maior que 1: O projeto está adiantado no cronograma;
- Menor que 1: O projeto está atrasado no cronograma;
- Igual a 1: O projeto está de acordo com o cronograma;

**Índice de performance por custo (CPI)**, igual ao SPI, que mostra a eficiência de custo do projeto e mede o valor agregado em relação aos custos atuais do projeto. É calculado com **CPI = EV/AC**, onde o resultado:

- Maior que 1: O projeto está dentro do orçamento e o projeto está sendo lucrativo;
- Menor que 1: O projeto está acima do orçamento e o projeto não está valendo os custos realizados
- Igual a 1: O valor agregado é igual aos custos do projeto;

## Referências:

- **A BEGINNER’S Guide to Earned Value Management**: Earned value is a technique used in project management to estimate where a project is versus the planned budget and schedule. We’ll consider its benefits and how to calculate it.. [S. l.], 9 jan. 2021. Disponível em: https://www.fool.com/the-blueprint/earned-value-management/. Acesso em: 13 mar. 2021.
