# Backlog do Produto

## Histórico de Revisão
|Autor|Mudanças|Data|Versão|
|--|--|--|--|
|[Luiz Henrique](https://github.com/luiz-herique)|Criação do documento|03/03/21|0.1|
|[Luiz Henrique](https://github.com/luiz-herique)|Arrumando o caminho do documento para a wiki|05/03/21|0.2|
|[Luiz Henrique](https://github.com/luiz-herique)|Refinamento dos eṕicos e textos|05/03/21|0.3|
|[Matheus Blanco](https://github.com/MatheusBlanco)|Arrumando histórico de revisão|05/03/21|0.4|
|[Matheus Blanco](https://github.com/MatheusBlanco)|Arrumando links e features|06/03/21|0.5|
|[Matheus Blanco](https://github.com/MatheusBlanco)|Arrumando textos|06/03/21|0.6|

## Histórias de Usuário

O escopo do projeto foi delimitado explorando a necessidade de simplificação do processo de denúncias, que atualmente é demorado e ineficiente, analisando o mesmo a fim de listar as funcio nalidades necessárias para realizar um intermédio entre o cidadão morador da comunidade e o orgão responsável por resolver o problema da denúncia.

Definidas as funcionalidades as mesmas foram dividas em um contexto macro em Épicos, que são subdividos em Features, as quais contém as Histórias de Usuário. As mesmas foram priorizadas utilizando o metódo MoSCoW, sendo classificas como: Must Have (Tenho que fazer), Should Have (Devo fazer), Could Have (Poderia fazer), Would Have (poderia fazer).

É importante frisar que o backlog sofrerá ajustes ao longo do andamento do projeto para que as necessidades sejam todas atendidas, sendo re-analisado a cada sprint para que se mantenha alinhado com a evolução de nível técnico da equipe.


## Épico 01 - Usuário

Este épico determina as histórias que formarão as funcionalidade relacionadas ao usuário, dentro dela são definidos paramentros que um desenvolvedor deseja ter para possuir um bom gerenciamento de seus usuários. Também contém funcionalidades que um usuário dejesa utilizar para realizar ações relativas ao seu perfil e interação geral com a aplicação.

### Feature 01 - CRUD de usuário

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US01|Eu, como desenvolvedor, desejo salvar um usuário com os campos: Usuário {id, nome, sobrenome, imagem, data de nascimento, email e cpf}, Localização {id, latitude, longitude, endereço, CEP, id de usuário}|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US02|Eu, como desenvolvedor desejo poder visualizar os dados de um usuário no banco, para que eu possa saber quem está cadastrado|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US03|Eu, como desenvolvedor, desejo poder criar uma rota para edição de dados do usuário, para que o mesmo possa mudar informações de seu cadastro|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US04|Eu, como desenvolvedor, desejo poder ser capaz de deletar usuários do banco, para que eu possa retirar possíveis usuários da aplicação|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US05|Eu, como usuário, desejo me cadastrar no Eccoar para que eu possa realizar anúncios e denúncias de problemas em minha comunidade|Must|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US06|Eu, como usuário, desejo visualizar meu perfil, para que eu possa ter noção de meus dados e informações relativas a minha conta|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US07|Eu, como usuário, desejo poder editar meu perfil, para que eu possa alterar informações básicas e essenciais da minha conta|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US08|Eu, como usuário, desejo poder deletar minha conta, caso eu deseje me desvincular do aplicativo e cerrar minhas atividades no mesmo|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|

### Feature 02 - Interação de usuário com a aplicação

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US09|Eu, como usuário, desejo ver informações básicas de negócio e funcionamento do sistema em uma landing page, para que eu possa entender melhor seu funcionamento|Should|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US10|Eu, como usuário, desejo poder ver informações de legislação sobre o assunto, para que eu possa me informar sobre a ação do estado e dos orgãos responsáveis|Would|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)
|US11|Eu, como usuário, desejo poder ver informações e elementos lúdicos e que me motivem a continuar utilizando a plataforma|Could|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)
|US12|Eu, como desenvolvedor, desejo ter um canal de comunicação com o usuário, para que eu possa tirar dúvidas com o mesmo sobre a aplicação|Could|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)
|US13|Eu, como usuário, desejo me comunicar com a equipe de desenvolvimento do software, para que eu possa tirar dúvidas e resolver problemas|Could|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)
|US14|Eu, como usuário, desejo ver em minha página de perfil, informações sobre os problemas que ajudei a resolver, sendo em votação, denúncia, confirmação de solução, para que eu possa ver em dados minha contribuição para minha sociedade|Could|[Perfil de usuário, COLAB](https://app.colab.re/user/356534)|

## Épico 02 - Denúncia

Este épico determina as histórias de usuário que formarão as funcionalidades de denúncias. Estão descritas as funcionalidades que um desenvolvedor necessita para fazer o controle e encaminhamento adequado de denúncias, bem como as necessárias para que um usuario possa realizar uma denúncia e possa interagir com denúncias criadas por outros usuários.

### Feature 03 - CRUD de denúncia

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US15|Eu, como desenvolvedor, desejo salvar no banco informações sobre uma denúncia, com os dados: Denúncia {id, nome, imagem, descrição, latitude, longitude, categoria, data de criação, data de fechamento, status e id de usuário} Votos {id da denúncia, id do usuário}|Must|[Perguntas 2, 3 e 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US16|Eu, como usuário, desejo poder preencher um formulário para que eu possa registrar minha denúncia|Must|[Perguntas 2, 3 e 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US17|Eu, como usuário, desejo categorizar minha denúncia, para que eu tenha a certeza que a mesma está sendo enviada para o orgão correto|Should|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US18|Eu, como usuário, desejo ter a opção de fazer denúncias sem foto, para que eu possa agilizar o processo de denúncia|Must|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US19|Eu, como usuário, desejo poder tirar uma foto dentro do próprio aplicativo para postar em minha denúncia, para que eu possa realizar a mesma de maneira rápida|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US20|Eu, como desenvolvedor, desejo poder ser capaz de deletar denúncias do banco, para que eu possa retirar possíveis denúncias inválidas da aplicação|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US21|Eu, como usuário, desejo poder deletar minha denúncia, caso eu sinta que a mesma não foi justificada ou tenha me enganado quanto ao seu teor|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US22|Eu, como desenvolvedor, desejo poder ser capaz de alterar dados das denúncias no banco, para que o usuário possa alterar informações essenciais da mesma|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US23|Eu, como usuário, desejo poder editar minha denúncia, para que eu possa editar informações sobre a mesma, caso sinta que seja necessário ou que algo tenha mudado|Could|[Lean, Brainstorm de funcionalidades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US24|Eu, como desenvolvedor, desejo poder ser capaz de ver do banco as denúncias criadas por usuário, para que o mesmo possa ter acesso a elas em seu sistema|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US25|Eu, como usuário, desejo poder ver as denúncias que criei, para que eu possa acompanhar seu andamento, comentários|Must|[Colab, feed de notícias](https://app.colab.re/home)|
|US26|Eu, como desenvolvedor, desejo poder ser capaz de ver do banco todas as denúncias criadas pelos usuários, para que o mesmo possa ter acesso a elas no feed de denúncias|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US27|Eu, como usuário, desejo poder ver o feed de denúncias, para que eu possa ver as denúncias na página principal do sistema|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US28|Eu, como desenvolvedor, desejo poder acessar os dados de uma denúncia a partir de seu ID, para que eu possa focar nas informações providas na mesma|Should|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|


### Feature 04 - Interação de usuário com denúncia

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US29|Eu, como usuário, desejo poder abrir uma denúncia para ver mais detalhes sobre a mesma, incluindo comentários|Should|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[brainstorm](https://miro.com/app/board/o9J_lVC-W9A=/?moveToWidget=3074457354169694144&cot=10)|
|US30|Eu, como usuário, desejo poder votar em uma denúncia que eu tenha visto na aplicação, para que ela receba mais visibilidade e relevância a partir de testemunhos|Must|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|
|US31|Eu, como usuário, desejo poder comentar em uma denúncia, para que eu possa deixar e ver mais informações sobre a mesma|Could|[Lean, Brainstorm de funcionaliadades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US32|Eu, como desenvolvedor, desejo poder filtrar denúncias de acordo com suas categorias, para que eu possa ver com maior foco aquelas em uma categoria específica|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US33|Eu, como usuário, desejo poder pesquisar uma denúncia de acordo com sua categoria, para que eu possa visualizar mais rapidamente denúncias de áreas específicas(Ex. Problemas elétricos, Saneamento Básico, Vias Públicas)|Could|[Pergunta 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US34|Eu, como desenvolvedor, desejo poder filtrar as denúncias por resolvidas, para que eu possa mostrar ao usuário quais já foram resolvidas|Should|[Perguntas 2, 3 e 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US35|Eu, como usuário, desejo poder ver quais problemas foram resolvidos pelo estado, para que eu possa ter uma melhor noção do avanço da melhoria de minha comunidade|Could|[Lean, Brainstorm de funcionaliadades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|


### Feature 05 - Alteração de status da denúncia

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US36|Eu, como desenvolvedor, desejo ser capaz de alterar apenas o status de uma denúncia, para que eu possa mostrar ao usuário qual o seu progresso atual|Must|[Perguntas 2, 3 e 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|
|US37|Eu, como usuário, desejo saber quando uma denúncia foi dada como resolvida, para que eu possa checar se o problema foi realmente solucionado|Must|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|
|US38|Eu, como usuário, desejo saber quando uma denúncia foi dada como resolvida, para que eu possa checar se o problema foi realmente solucionado|Must|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|
|US39|Eu, como usuário, desejo poder confirmar no sistema que um problema foi resolvido, para que eu possa testemunhar tal resolução e fechar a denúncia|Must|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 1](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=2-1590072209220)|
|US40|Eu, como desenvolvedor, desejo poder fechar uma denúncia quando a mesma tenha uma quantidade x de confirmações de resolução, para que eu possa notificar os usuários de tal notícia|Must|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 1](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=2-1590072209220)|


## Épico 03 - Comunicação com orgãos

Este épico determina as histórias que formarão as funcionalidades relacionadas a comunicação com orgãos responsaveis, contemplando envio de e-mails para os orgãos responsáveis pela resolução dos problemas, construção do relatório a ser enviado

### Feature 06 - Envio de relatório para orgãos responsáveis

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US41|Eu, como desenvolvedor, desejo filtrar as denúncias na aplicação por quantidade de votos, para que eu possa fazer o envio das mesmas para os orgãos responsáveis|Should|[Lean, Brainstorm de funcionaliadades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US42|Eu, como desenvolvedor, desejo poder ser capaz de enviar mensagens de e-mail para qualquer e-mail que eu deseje, para que mais tarde eu possa enviar tais mensagens para orgãos específicos|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US43|Eu, como desenvolvedor, desejo poder enviar mensagens de e-mail para orgãos do governo, para que eu possa cumprir minha missão de dar visibilidade aos problemas|Must|[Perguntas 2](https://forms.gle/XKECTpJPDEERX1ci9)|

### Feature 07 - Construção do relatório para ser enviado

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US44|Eu, como desenvolvedor, desejo que a aplicação gere um relatório automatizado, com informações básicas sobre a denúncia, para que eu possa enviá-la por e-mail|Must|[Lean, Brainstorm de funcionaliadades](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb)|
|US45|Eu, como desenvolvedor, desejo realizar text-mining dos dados da denúncia, para que eu possa gerar o relatório mais rapidamente|Must|[Perguntas 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|


### Feature 08 - Identificação do Orgão responsável

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US46|Eu, como desenvolvedor, desejo que a aplicação saiba identificar quais orgãos receberão a denúncia a partir da categorização feita pelo usuário, para que eu possa redirecionar a denúncia para o orgão identificado|Could|Must|[Perguntas 8.1](https://forms.gle/XKECTpJPDEERX1ci9)|

## Épico 04 - Geolocalização

Este épico determina as histórias que formarão as funcionalidades relacionadas a Geolocalização, comtemplando funcionalidade que permitirão a setorização das denúncias que auxiliarão os desenvolvedores a mostrar para os usuários as denúncias que estejam dentro do raio de localização dos mesmos.

### Feature 09 - Filtro de denúncias por geolocalização

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US47|Eu, como desenvolvedor, desejo poder identificar a localização de uma denúncia a partir de sua longitude e latitude, para que eu possa saber sua geolocalização|Should|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 1](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=2-1590072209220)|
|US48|Eu, como desenvolvedor, desejo poder pegar a localização de um usuário em tempo real, para que eu possa fazer o filtro de denúncias|Should|[Perfil contendo mapa, COLAB](https://app.colab.re/user/356534)
|US49|Eu, como desenvolvedor, desejo ser capaz de filtrar as denúncias que estejam em um raio de até X km de uma localização específica, para que eu possa mostrar ao usuário ditas denúncias|Would|[Perfil contendo mapa, COLAB](https://app.colab.re/user/356534)
|US50|Eu, como usuário, desejo poder ver as denúncias perto de mim, para que eu possa identificar os problemas existentes em minha localidade|Must|[Perfil contendo mapa, COLAB](https://app.colab.re/user/356534)
|US51|Eu, como usuário, desejo selecionar a localização de uma denúncia em sua criação, para que eu possa criá-la com mais acurácia em termos de geolocalização|Should|[Perfil contendo mapa, COLAB](https://app.colab.re/user/356534)

## Épico 04 - Notificação

Este épico determina as histórias que formarão as funcionalidades relacionadas a notifições, as histórias de usuário comtemplam as necessidades para que o sistema seja capaz de enviar notificações para os usuários, de acordo com o seu assunto.

### Feature 10 - Notificações relativas ao status da denúncia

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US52|Eu, como usuário desejo receber notificações sobre mudanças de status de uma denúncia que interagi com, para que eu possa estar informado sobre seu progresso|Could|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|
|US53|Eu, como usuário, desejo receber notificações sobre o status atual de uma denúncia de maneira regular, para que eu possa estar alinhado sobre a situação da mesma|Could|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|

### Feature 11 - Notificações relacionadas a envio do relatório

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US54|Eu, como usuário, desejo receber uma notificação sobre o envio do relatório para o orgão responsável, para que eu tenha certeza de que o sistema esteja fazendo seu trabalho|Should|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|

### Feature 12 - Notificações relacionadas a envio do relatório

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US55|Eu, como usuário, desejo receber uma notificação sobre a resolução de um problema, para que eu possa checar o status da mesma|Should|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Jornada 2](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb?wid=1-1590072209220)|
