# Analytics Reports

## Complexidade

![Complexidade](../assets/img/analytics/reports/complexidade.jpg)
![ComplexidadeH](../assets/img/analytics/reports/complexidade_h.jpg)
![ComplexidadeB](../assets/img/analytics/reports/complexidade_b.jpg)

1. Release 1:
    - 77% de arquivos não complexos.
    - 26 arquivos alterados
        - 15 novos arquivos
    - Além de configurações relacionadas ao ambiente de desenvolvimento, nessa release foi adicionada toda a estrutura de geração do PDF de relatório e o envio do arquivo ao serviço de armazenamento na nuvem da AWS, o S3. Ainda foi adicionado ao serviço, o tratamento de erros. O conjunto dessas alterações refletiu no aumento da complexidade.

2. Release 3:
    - 70% de arquivos não complexos.
    - 3 arquivos alterados
    - Essa release representou um aumento da complexidade ciclomática. Nela foi realizada a adição do Sentry, que conta com um handler de erro para caso haja algum problema na execução. Esse tratamento acaba aumentando a complexidade por se configurar como um desvio de fluxo.


## Densidade de linhas comentadas

![Densidade de linhas comentadas](../assets/img/analytics/reports/comments.jpg)
![Densidade de linhas comentadas H](../assets/img/analytics/reports/comments_h.jpg)
![Densidade de linhas comentadas B](../assets/img/analytics/reports/comments_b.jpg)

O repositório Reports possui uma quantidade de comentários zerados em todas as Releases pelo fato de que o time do projeto Eccoar ter decidido por eliminar a inserção de qualquer comentário nos repositórios.

## Densidade de linhas duplicadas

![Densidade de linhas duplicadas](../assets/img/analytics/reports/duplication.jpg)
![Densidade de linhas duplicadas H](../assets/img/analytics/reports/duplication_h.jpg)
![Densidade de linhas duplicadas B](../assets/img/analytics/reports/duplication_b.jpg)

A ausência de duplicações se manteve em 100% no decorrer de todo o projeto, ficando constante no decorrer de todas as releases.

## Produtividade

![Produtividade](../assets/img/analytics/reports/prod.jpg)

## Manutenibilidade

![Manutenibilidade](../assets/img/analytics/reports/maintain.jpg)
![ManutenibilidadeB](../assets/img/analytics/reports/maintain_b.jpg)

## Análise descritiva

![Análise descritiva](../assets/img/analytics/reports/analysis.jpg)

- Na m1, podemos ver que a média de não complexidade ficou em 78%, o que demonstra que o código apresenta um bom nível de linearidade de execução no seu fluxo. Possuindo pouca queda da mesma para sua métrica mínima de complexidade, o que confirma a hipótese apresentada anteriormente.
- Na m2, podemos observar baixa variação na taxa de linhas comentadas, o que demonstra que o time não utilizou comentários como uma ferramenta em seu desenvolvimento.
- Na m3, observando os dados, olhamos que a constância de densidade de código duplicado permanece máxima em todo momento, demonstrando a efetividade do time.

## Análise de percentis

![Percentis](../assets/img/analytics/reports/percentis.jpg)

## Regressão linear

![Regressão linear](../assets/img/analytics/reports/linearRegression.jpg)

## Matriz de correlação

![Matriz de correlação](../assets/img/analytics/reports/correlation.jpg)

Nessa tabela podemos perceber que:

- m1/m2/m3/m7/m9/asc1/ac1/totalAC1/asc2/totalAC2 e m2/m3 possue uma correlação nula, já que seu coeficiente é igual a zero. Dessa forma, não ocorre uma relação.

- m1 e m7 se correlacionam negativamente. Como seu valor é aproximado de 0, sua correlação é fraca.

- m1 e m9 se correlacionam negativamente. Como seu valor é aproximado de 0, sua correlação é fraca.

- m1 e asc1/ac1/totalAC1 se correlacionam positivamente. Como seu valor é igual a 1, sua correlação é forte.

- m1 e asc2/totalAC2 se correlacionam negativamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m7 e m9 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- m7 e asc1/ac1/totalAC1 se correlacionam negativamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m7 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- m9 e asc1/ac1/totalAC1 se correlacionam negativamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m9 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- asc1/ac1 e totalAC1 se correlacionam positivamente. Como seu valor é igual a 1, sua correlação é forte.

- asc1/ac1/totalAC1 e asc2/totalAC2 se correlacionam negativamente. Como seu valor é aproximado de zero, sua correlação é fraca.