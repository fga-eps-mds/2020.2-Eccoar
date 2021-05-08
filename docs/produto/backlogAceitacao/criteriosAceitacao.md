# Critérios de Aceitação

## Histórico de Revisão

| Autor                                              | Mudanças                                            | Data     | Versão |
| -------------------------------------------------- | --------------------------------------------------- | -------- | ------ |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Criação do documento                                | 21/03/21 | 0.1    |
| [Matheus Blanco](https://github.com/MatheusBlanco) | Atualização do documento de acordo com novo backlog | 7/05/21  | 0.2    |

Este artefato diz respeito a lista de critérios necessários para que as [histórias de usuário](./backlogProduto.md) sejam consideradas concluídas. Este artefato será concluído de acordo com a finalização da documentação de cada história.

## US01 - Eu, como cidadão, desejo me cadastrar no Eccoar para que eu possa realizar anúncios e denúncias de problemas em minha comunidade

- O usuário deve poder se cadastrar, com Nome, sobrenome, senha, e-mail, telefone e CPF e endereço;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US02 - Eu, como cidadão, gostaria de poder utilizar minhas credenciais anteriormente criadas para o sistema para que eu possa utilizá-lo em sua totalidade como um usuário pleno.

- O usuário deverá ser capaz de ser autenticado na aplicação com seu e-mail e sua senha;
- O usuário não deverá mais poder utilizar a aplicação (ver denúncias, adicionar voto, criar denúncia) se não estiver autenticado;
- Funcionalidade testada;
- De acordo com o protótipo de alta-fidelidade.

## US03 - Eu, como cidadão, desejo visualizar meu perfil, para que eu possa ter noção de meus dados e informações relativas a minha conta, além de poder ver as denúncias que interagi com ou criei recentemente, linkando com meu histórico.

- O usuário deve ser capaz de acessar suas informações de perfil e ver seu nome, sobrenome, e-mail cadastrado, telefones e CPF;
- O usuário deve ser capaz de ver em sua página de perfil informações sobre os problemas que o mesmo ajudou a resolver, seja com upvote, com confirmação da resolução;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US04 - Eu, como cidadão, desejo poder editar meu perfil, para que eu possa alterar informações básicas e essenciais da minha conta

- O usuário deve ser capaz de poder alterar as informações de seu perfil, preenchendo um formulário com as novas informações;
- Deve existir um botão que mostre facilmente o local que o usuário deve apertar para que ele possa alterar seus dados;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US05 - Eu, como cidadão, desejo poder deletar minha conta, caso eu deseje me desvincular do aplicativo e cerrar minhas atividades no mesmo

- O usuário deve poder deletar sua conta permanentemente e apagar seus dados do aplicativo, a partir de clique em botão existente na página de perfil;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US06 - Eu, como cidadão, desejo ver informações básicas de negócio e funcionamento do sistema em uma landing page, para que eu possa entender melhor seu funcionamento

- O usuário deve ser capaz de acessar uma página especial que contenha informações importantes de negócio e de utilização do sistema _Eccoar_;
- A página deve conter todas as informações necessárias, tais como: modo de uso, propósito, como o sistema tenta ajudar a resolver problemas nas comunidades do DF, como é feita a comunicação com órgãos e como ele se difere de concorrentes;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US07 - Eu, como cidadão, desejo poder ver informações de legislação sobre o assunto, para que eu possa me informar sobre a ação do estado e dos órgãos responsáveis

- O usuário deve ser capaz de acessar uma página especial que contenha informações sobre legislações e regulamentações do trabalhos dos órgãos públicos no DF;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US08 - Eu, como cidadão, desejo poder ver informações e elementos lúdicos e que me motivem a continuar utilizando a plataforma

- O usuário deve poder ter acesso a elementos que o engajem a realizar suas atividades;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US09 - Eu, como cidadão, desejo me comunicar com a equipe de desenvolvimento do software, para que eu possa tirar dúvidas e resolver problemas

- O usuário deve poder acessar uma página especial onde ele possa mandar perguntas para a equipe de desenvolvimento;
- A página deve conter um formulário de contato, com os campos: nome, e-mail, assunto e texto de pergunta;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US10 - Eu, como cidadão, desejo poder ver as denúncias que criei ou interagi, para que eu possa acompanhar seu andamento.

- O usuário deve ser capaz de accessar uma página específica que lhe mostre todas as denúncias com as quais ele interagiu (criou, votou);
- O usuário deve ser capaz de ver também as denúncias que foram dadas como resolvidas e foram fechadas;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US11 - Eu, como usuário, desejo poder preencher um formulário para que eu possa registrar minha denúncia.

- O formulário deverá ter os campos nome, imagem, descrição, latitude e longitude, categoria (selecionável);
- Deverá ter um feedback visual com os dados enviados e cadastrados no banco de dados;
- De acordo com a identidade visual

## US12 - Eu, como cidadão, desejo ter a opção de poder enviar fotos para as denúncias criadas, para que eu possa agilizar o processo de averiguação da denúncia

- O usuário deve ser capaz de inserir no formulário de denúncias um arquivo de imagem em JPEG e PNG para que o mesmo possa ser salvo, no campo de denúncias, a partir de um link em bucket apropriado (AWS S3);
- Deve haver um componente que permita ao usuário fazer o attach de imagens;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US13 - Eu, como cidadão, desejo poder tirar uma foto dentro do próprio aplicativo para postar em minha denúncia, para que eu possa realizar a mesma de maneira rápida

- O usuário deve ser capaz de tirar uma foto diretamente do sistema, sem que seja necessário tirar uma foto por fora e depois adicioná-la ao sistema;
- O sistema deve ser capaz de se comunicar com a câmera do celular onde está sendo utilizado, para que o mesmo possa tirar e armazenar a foto;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US14 - Eu, como cidadão, desejo poder deletar minha denúncia, caso eu sinta que a mesma não foi justificada ou tenha me enganado quanto ao seu teor

- O usuário deve ser capaz de, na página de detalhamento da denúncia, deletar a mesma e excluí-la permanentemente do banco de dados;
- O usuário deve ser capaz de deletar apenas as denúncias que foram criadas por si mesmo
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US15 - Eu, como cidadão, desejo poder editar minha denúncia, para que eu possa editar informações sobre a mesma, caso sinta que seja necessário ou que algo tenha mudado

- O usuário deve ser capaz de, na página de detalhamento da denúncia, abrir um formulário de edição para arrumar as informações da denúncia em questão, incluindo título, descrição, foto, localização e categoria;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US16 - Eu, como cidadão, desejo poder ver as denúncias que criei, para que eu possa acompanhar seu andamento, comentários

- O usuário deve ser capaz de, no feed de denúncias, filtrar aquelas que foram criadas pelo mesmo;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US17 - Eu, como usuário, desejo poder ver o feed de denúncias, para que eu possa ver as denúncias na página principal do sistema

- Mostrar as denúncias existentes;
- Seguir o prototipo de fidelidade;
- As denúncias devem aparecer ordenadas por data (mais recentes primeiro);

## US18 - Eu, como cidadão, desejo poder ver apenas as denúncias que estejam perto de mim, para que eu possa identificar os problemas existentes em uma área que eu possa alcançar sem muito esforço ou gasto de recursos

-O usuário deve ser capaz de ver, no feed de denúncias, apenas aquelas que estejam perto de si, em um raio de 2 quilômetros;

- O usuário deve ser capaz de ser geolocalizado;
- Funcionalidade testada;

## US19 - Eu, como cidadão, desejo poder abrir uma denúncia para ver mais detalhes sobre a mesma

- O usuário deve ser capaz de, ao clicar no card de denúncias, ser redirecionado a uma página que conterá todos os detalhes da denúncia em questão, inclusive progresso (simbolizado de acordo com os botões).
- O botão de interação deverá ser renderizado de acordo com o status atual da denúncia
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US20 - Eu, como cidadão, desejo poder confirmar uma denúncia que eu tenha visto na aplicação, para que ela receba mais visibilidade e relevância a partir de testemunhos

- Rota de contagens de upvote criada;
- A contagem de upvote alterar ao clicar no botão do card do front;
- A informações do upvote esteja vindo proveniente da rota do back e deve ter um feedback visual sobre sua existência;
- Funcionalidade testada padrão;
- De acordo com o protótipo;

## US21 - Eu, como usuário, gostaria de poder retirar meus votos, para que eu possa desvalidar uma denúncia ou fazer com que sua confirmação de resolução não seja ativada

- O usuário deve ser capaz de apertar nos seus votos e retirá-los;
- Os votos retirados não devem mais aparecer para o usuário (mudar a cor do botão);
- Funcionalidade testada;
- De acordo com a identidade visual;

## US22 - Eu, como cidadão, desejo poder comentar em uma denúncia, para que eu possa deixar e ver mais informações sobre a mesma

- O usuário deverá ser capaz de, na página de detalhamento da denúncia, ser capaz de deixar um comentário;
- A página de detalhamento deve ter uma caixa de input para que o usuário possa deixar seu comentário;
- A página de detalhamento deve mostrar todos os comentários feitos pelos outros usuários;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US23 - Eu, como cidadão, gostaria de poder filtrar o feed de denúncias de acordo com alguns parâmetros para que eu possa ver informações específicas de denúncias de maneira mais fácil e objetiva, ao invés de ter que procurar em todo o feed

- Deverá ser capaz de filtrar as denúncias de acordo com os status, as categorias e a quantidade de votos;
- Deverá mostrar apenas as denúncias que possuem as características listadas no filtro;
- Feature flag para ativar e desativar o dropdown;
- De acordo com o protótipo;
- Funcionalidade testada;

## US24 - Eu, como cidadão, desejo poder marcar que uma denúncia foi "Concluída", para que eu possa alertar o sistema e as pessoas utilizadoras do sistema sobre o progresso do problema

- Poder confirmar que a denúncia foi concluída;
- O botão de upvote do card deverá mudar a partir de um trigger baseado no campo de status da denúncia, e renderizar o botão de confirmação;
- A quantidade de confirmações deve ser contabilizada na aplicação, tiradas da nova tabela de resolução;
- Funcionalidades testada padrão;
- Estar igual ao protótipo;

## US25 - Eu, como cidadão, desejo poder ver que uma denúncia resolvida foi fechada, para que o sistema não fique me mostrando denúncias de problemas que não existem mais

- O feed de denúncias deve dar um feedback visual de que a denúncia foi fechada, por um tempo, e posteriormente, tirá-la do feed;
- A página de detalhamento de denúncia deve prover um feedback visual para mostrar ao usuário que a denúncia foi fechada;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US26 - Eu, como funcionário de orgão público, desejo receber em meu e-mail relatórios sobre as denúncias mais relevantes de diferentes áreas e que se encaixem na minha linha de trabalho, para que eu possa tomar ações de resolução sobre os problemas relatados

- O destinatário deve receber um e-mail de um provedor específico, com corpo de mensagem e assunto.
- Funcionalidade testada;

## US27 - Eu, como funcionário de órgão público, desejo receber em meu e-mail apenas as denúncias mais relevantes da aplicação, categorizadas de acordo com suas áreas de impacto para que eu possa tomar as ações necessárias

- O funcionário do órgão público em questão deverá receber em seu e-mail apenas as denúncias que são categorizadas de acordo com sua área e que se mostraram relevantes para os cidadãos da comunidade (as denúncias que estão em status de wait);
- O funcionário do órgão público deve receber esse e-mail em um dia específico do mês, e o e-mail não deve conter nem todas as denúncias de sua categoria, nem todas as denúncias que tiveram poucos votos;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US28 - Eu, como funcionário de órgão público, desejo que o e-mail enviado contenha um relatório completo e que me mostre todos os dados necessários para sua resolução, para que eu possa tomar as ações necessárias

- Deverá ser capaz de gerar o html do relatório;
- Deverá ser capaz de gerar um arquivo pdf a partir do html;
- O relatório deverá conter as seguintes informações: título da denúncia, descrição da denúncia, foto, quantos votos foram contabilizados, data da criação da denúncia;
- Funcionalidade testada;
- Relatório de acordo com a identidade visual;

## US29 - Eu, como funcionário de órgão público, gostaria de receber frequentemente em minha caixa de e-mail os relatórios gerados pelo sistema Eccoar, para que eu esteja sempre sabendo dos problemas recorrentes das comunidades.

- Deverá implementar um cronjob que irá ativar as funções de geração de report e envio de e-mails todo mês no dia 26;
- Funcionalidade testada;

## US30 - Eu, como cidadão, desejo selecionar a localização de uma denúncia em sua criação, para que eu possa criá-la com mais acurácia em termos de geolocalização e para que a mesma apareça para os outros cidadãos que estejam perto da mesma

- O usuário deve ser capaz de, no formulário de denúncia, inserir em um componente de mapa a localização de sua denúncia;
- O mapa deve se atualizar também para mostrar a localização do usuário;
- O usuário deve ser capaz de localizar a denúncia em um raio de apenas 100 metros;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US31 - Eu, como cidadão desejo receber notificações sobre mudanças de status de uma denúncia que interagi com, para que eu possa estar informado sobre seu progresso

- O usuário deve receber notificações _e-mail_ de acordo com a mudança de progresso da denúncia;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;

## US32 - Eu, como cidadão, desejo receber uma notificação sobre o envio do relatório para o órgão responsável, para que eu tenha certeza de que o sistema esteja fazendo seu trabalho

- O usuário deve receber notificações _e-mail_ de acordo com o envio do e-mail para o órgão responsável;
- Funcionalidade testada;
- De acordo com o protótipo de alta fidelidade;
