# Analytics Users

## Complexidade

![Complexidade](../assets/img/analytics/users/complexidade.jpg)
![ComplexidadeH](../assets/img/analytics/users/complexidade_h.jpg)
![ComplexidadeB](../assets/img/analytics/users/complexidade_b.jpg)

1. Release 1
    - 66% de arquivos não complexos.
    - 28 arquivos alterados.
        - 8 novos arquivos.
    - Nessa release, por decisão da equipe o repositório de usuários que havia sido depreciado, foi reinstaurado e reestruturado para ser utilizado como serviço de cadastro/gerenciamento de usuário.
    - Foi reestruturado o Docker do serviço, e foi estabelecida a conexão com o Firebase. Além disso, foi configurado o Morgan no ambiente para o ambiente de desenvolvimento e foi criado o tratamento de erros do serviço. O conjunto dessas mudanças resultou num aumento brusco da complexidade do serviço.


## Densidade de linhas comentadas

![Densidade de linhas comentadas](../assets/img/analytics/users/comments.jpg)
![Densidade de linhas comentadas H](../assets/img/analytics/users/comments_h.jpg)
![Densidade de linhas comentadas B](../assets/img/analytics/users/comments_b.jpg)

O repositório de Users possui uma quantidade de comentários zerados em todas as Releases pelo fato de que o time do projeto Eccoar ter decidido por eliminar a inserção de qualquer comentário nos repositórios.

## Densidade de linhas duplicadas

![Densidade de linhas duplicadas](../assets/img/analytics/users/duplication)
![Densidade de linhas duplicadas H](../assets/img/analytics/users/duplication_h.jpg)
![Densidade de linhas duplicadas B](../assets/img/analytics/users/duplication_b.jpg)

A ausência de duplicações se manteve em 100% no decorrer de todo o projeto, ficando constante no decorrer de todas as releases.

## Produtividade

![Produtividade](../assets/img/analytics/users/prod.jpg)

## Manutenibilidade

![Manutenibilidade](../assets/img/analytics/users/maintain.jpg)
![ManutenibilidadeB](../assets/img/analytics/users/maintain_b.jpg)

## Análise descritiva

![Análise descritiva](../assets/img/analytics/users/analysis.jpg)

- Na métrica m1, de complexidade, conseguimos constatar pelo quartil 50% que ½  de todas as releases geradas tiveram uma não complexidade maior que 66.67%, mostrando que durante todo o projeto o código de manteve não complexo. Confirmamos isso vendo a média alta de 76.19%.
- Na métrica m2, de densidade de linhas comentadas, temos que ela está zerada porque o time não usou comentários no desenvolvimento do código.
- Na métrica m3, de linhas de código duplicadas, vemos que ela permaneceu constante em todo o desenvolvimento.

## Análise de percentis

![Percentis](../assets/img/analytics/users/percentis.jpg)

## Regressão linear

![Regressão linear](../assets/img/analytics/users/linearRegression.jpg)

## Matriz de correlação

![Matriz de correlação](../assets/img/analytics/users/correlation.jpg)

Nessa tabela podemos perceber que:

- m1/m2/m3/m7/m9/asc1/ac1/totalAC1/asc2/totalAC2 e m2/m3 possue uma correlação nula, já que seu coeficiente é igual a zero. Dessa forma, não ocorre uma relação.

- m1 e m7 se correlacionam positivamente. Como seu valor é aproximado de 0, sua correlação é fraca.

- m1 e m9 se correlacionam negativamente. Como seu valor é aproximado de 0, sua correlação é fraca.

- m1 e asc1/ac1/totalAC1 se correlacionam positivamente. Como seu valor é igual a 1, sua correlação é forte.

- m1 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m7 e m9 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- m7 e asc1/ac1/totalAC1 se correlacionam positivamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m7 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- m9 e asc1/ac1/totalAC1 se correlacionam negativamente. Como seu valor é aproximado de zero, sua correlação é fraca.

- m9 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de 1, sua correlação é forte.

- asc1/ac1 e totalAC1 se correlacionam positivamente. Como seu valor é igual a 1, sua correlação é forte.

- asc1/ac1/totalAC1 e asc2/totalAC2 se correlacionam positivamente. Como seu valor é aproximado de zero, sua correlação é fraca.