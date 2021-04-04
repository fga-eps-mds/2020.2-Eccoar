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

### Tabela de RAs

| RA                 | Densidade Urbana (hab/ha) | Porcentagem escolhida |
| ------------------ | ------------------------- | --------------------- |
| Varjão             | 142,27                    | 4.2173332396148%      |
| Candangolândia     | 137,38                    | 4.3674479545785%      |
| Ceilândia          | 129,94                    | 4.6175157765122%      |
| Recanto das emas   | 117,88                    | 5.08992195453%        |
| São sebastião      | 112,75                    | 5.3215077605322%      |
| Estrutural         | 109,73                    | 5.4679668276679%      |
| Sudoeste           | 104,77                    | 5.7268301994846%      |
| Samambaia          | 103,31                    | 5.8077630432678%      |
| Cruzeiro           | 101,63                    | 5.903768572272%       |
| Brazlândia         | 93,52                     | 6.4157399486741%      |
| Paranoá            | 92,26                     | 6.5033600693692%      |
| Riacho Fundo 1     | 86,06                     | 6.9718800836626%      |
| Riacho Fundo 2     | 83,59                     | 7.1778920923555%      |
| Itapoã             | 81,93                     | 7.3233247894544%      |
| Taguatinga         | 80,5                      | 7.4534161490683%      |
| Núcleo Bandeirante | 78,60                     | 7.6335877862595%      |
| Guará              | 73,55                     | 8.1577158395649%      |
| Águas Claras       | 71,53                     | 8.3880889137425%      |
| Planaltina         | 63,72                     | 9.4161958568738%      |
| Sobradinho 2       | 58,94                     | 10.17984390906%       |
| Santa Maria        | 57,60                     | 10.416666666667%      |
| Gama               | 50,96                     | 11.773940345369%      |
| Sobradinho         | 41,73                     | 14.378145219267%      |
| Vicente Pires      | 31,95                     | 18.779342723005%      |
| Fercal             | 29,57                     | 20.290835306053%      |
| Plano Piloto       | 20,64                     | 29.06976744186%       |
| Lago Norte         | 9,99                      | 60.06006006006%       |
| Jardim Botânico    | 8,91                      | 67.340067340067%      |
| Lago Sul           | 6,66                      | 90.09009009009%       |
| Park Wway          | 3,50                      | 171.42857142857%      |
| SIA                | 1,08                      | 555.55555555556%      |
| DF                 | 47,19                     | 12.714558169104%      |

## O cálculo

Tendo essas informações em mãos, montamos uma fórmula que considera as densidades demográficas de todas as regiões administrativas do DF, calcula uma provável porcentagem de votos baseada nas observações do Colab, e tira a média simples dessa porcentagem para que se possa obter um valor representativo do DF como um todo. Posteriormente, considerando-se o contexto de pandemia, multiplica-se essa porcentagem pelo índice de adesão ao isolamento social para que se possa obter um valor reduzido e que represente os tempos atuais que o DF se encontra.

O cálculo pode ser então formalizado com a seguinte expressão:

<img src="https://latex.codecogs.com/gif.latex?\fn_phv&space;\left&space;(\frac{\left&space;(\sum_{1}^{nR}\left[&space;\left&space;\{&space;\frac{c}{100}&space;\right&space;\}\cdot&space;dU&space;\right&space;]&space;\right&space;)}{nR}&space;\right&space;)\cdot&space;iS" title="\left (\frac{\left (\sum_{1}^{nR}\left[ \left \{ \frac{c}{100} \right \}\cdot dU \right ] \right )}{nR} \right )\cdot iS" />

## Referências:

[1] - **DENSIDADES URBANAS NAS REGIÕES ADMINISTRATIVAS DO DISTRITO FEDERAL**. 22. ed. [S. l.], fev. 2017. Disponível em: http://www.codeplan.df.gov.br/wp-content/uploads/2018/02/TD_22_Densidades_Urbanas_nas_Regi%C3%B5es_Administrativas_DF.pdf. Acesso em: 31 mar. 2021.

[2] - **UM ANO** depois, índice de isolamento social no DF cai 21 pontos percentuais: Levantamento da empresa de softwares InLoco revela que a taxa de isolamento social na capital do país está em 44,12%. O DF, que já esteve em primeiro lugar na lista, figura em 19º entre as 27 unidades da Federação. [S. l.], 24 mar. 2021. Disponível em: https://www.correiobraziliense.com.br/cidades-df/2021/03/4913716-um-ano-depois-indice-de-isolamento-social-no-df-cai-21-pontos-percentuais.html. Acesso em: 31 mar. 2021.
