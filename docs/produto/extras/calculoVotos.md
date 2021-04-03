# Pesquisa para cálculo de contagem de votos

## Histórico de revisão

| Autor                                              | Mudanças             | Data       | Versão |
| -------------------------------------------------- | -------------------- | ---------- | ------ |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Criação do documento | 03/04/2021 | 1.0    |

## Introdução

Um dos objetivos do projeto _Eccoar_ é impulsionar e dar visibilidade para as denúncias criadas pelos usuários. Para que possamos realizar esse impulsionamento, trabalhamos com um sistema de votos, onde existem dois tipos diferentes:

- Os votos de impulsionamento de existência de denúncias, quando a denúncia se encontra em status _open_
- Os votos de confirmação de resolução da denúncia em questão, quando a denúncia se encontra em status _wait_ (aguardando)

A partir do alcance de um determinado número de votos, os mesmos realizados pela população usuária do sistema, o voto sofre uma ação. Se o voto for no status _open_ e sua quantidade atingir um certo número, a denúncia em questão será transformada em um PDF, e o mesmo será enviado para o órgão em questão. Se o voto for no status _wait_ e atingir a mesma quantidade, a denúncia será considerada resolvida e não aparecerá mais para seus usuários.

Entende-se que a quantidade de votos de uma denúncia é de considerável importância para que o sistema atinja seus objetivos. E como a quantidade de votos depende da quantidade de usuários, consideramos importante levantar um cálculo baseado em pesquisas que demonstre quantos votos, em média, seriam ideais para que uma denúncia seja impulsionada da maneira adequada.

## A pesquisa

Para se alcançar uma fórmula satisfatória e que representasse da melhor maneira os votos em uma denúncia, realizamos uma pesquisa baseada em três pilares. São eles:

- Entendimento de interação da população do DF com o aplicativo _Colab_, que por ser nosso concorrente possui uma missão e um sistema de funcionamento parecido. A partir da utilização do Colab e do estudo das regularidades do mesmo, entendemos que em média, 3 a 6 pessoas interagiam com uma denúncia, em um contexto de aproximadamente 1097 usuários (na data da criação da conta e desse estudo). Definimos o valor de 6 votos como o valor base para nossos cálculos por hora, entretanto este número pode variar em cenários ou tempos diferentes;
- Pesquisa de densidade demográfica do DF. A partir do estudo de um censo [1] das regiões administrativas do DF, pudemos ter um paronama geral da quantidade de pessoas moradoras em uma área de 1 héctare (10 mil m²). Os resultados foram anotados em uma [tabela](https://docs.google.com/document/d/1XNyyUlRmfW0P4hhyy5SEMRSILI2vUtCO8WhCaj4CLtU/edit?usp=sharing) e utilizados para o cálculo posterior;
- Pesquisa de informação acerca dos índices recentes de isolamento social no DF. Como nosso produto é impactado principalmente pelo fluxo de pessoas na rua, sabemos que a densidade demográfica não representa necessáriamente os valores atuais. Dessa forma, pegamos em uma reportagem recente que o índice de adesão ao isolamento social se encontra na casa 44% [2];

## O cálculo

Tendo essas informações em mãos, montamos uma fórmula que considera as densidades demográficas de todas as regiões administrativas do DF, calcula uma provável porcentagem de votos baseada nas observações do Colab, e tira a média simples dessa porcentagem para que se possa obter um valor representativo do DF como um todo. Posteriormente, considerando-se o contexto de pandemia, multiplica-se essa porcentagem pelo índice de adesão ao isolamento social para que se possa obter um valor reduzido e que represente os tempos atuais que o DF se encontra.

O cálculo pode ser então formalizado com a seguinte expressão:

<img src="https://latex.codecogs.com/gif.latex?\fn_phv&space;\left&space;(\frac{\left&space;(\sum_{1}^{nR}\left[&space;\left&space;\{&space;\frac{c}{100}&space;\right&space;\}\cdot&space;dU&space;\right&space;]&space;\right&space;)}{nR}&space;\right&space;)\cdot&space;iS" title="\left (\frac{\left (\sum_{1}^{nR}\left[ \left \{ \frac{c}{100} \right \}\cdot dU \right ] \right )}{nR} \right )\cdot iS" />

## Referências:

[1] - **DENSIDADES URBANAS NAS REGIÕES ADMINISTRATIVAS DO DISTRITO FEDERAL**. 22. ed. [S. l.], fev. 2017. Disponível em: http://www.codeplan.df.gov.br/wp-content/uploads/2018/02/TD_22_Densidades_Urbanas_nas_Regi%C3%B5es_Administrativas_DF.pdf. Acesso em: 31 mar. 2021.

[2] - **UM ANO** depois, índice de isolamento social no DF cai 21 pontos percentuais: Levantamento da empresa de softwares InLoco revela que a taxa de isolamento social na capital do país está em 44,12%. O DF, que já esteve em primeiro lugar na lista, figura em 19º entre as 27 unidades da Federação. [S. l.], 24 mar. 2021. Disponível em: https://www.correiobraziliense.com.br/cidades-df/2021/03/4913716-um-ano-depois-indice-de-isolamento-social-no-df-cai-21-pontos-percentuais.html. Acesso em: 31 mar. 2021.
