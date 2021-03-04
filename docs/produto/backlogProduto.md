# Backlog do Produto

## Histórico de Revisão
|Autor|Mudanças|Data|Versão|
|--|--|--|--|
|[Luiz Henrique](https://github.com/luiz-herique)|Criação do documento; Adição de introdução, descrição do produto, objetivo do produto, e stakeholders.|03/02/21|0.1|

## Histórias de Usuário

## Épico 01 - Épico

### Feature 01 - CRUD de usuário

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US01|Eu, como desenvolvedor, desejo salvar um usuário com os campos: Usuário {id, nome, sobrenome, imagem, data de nascimento, email e cpf}, Localização {id, latitude, longitude, endereço, CEP, id de usuário}|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US02|Eu, como desenvolvedor desejo poder visualizar os dados de um usuário no banco, para que eu possa saber quem está cadastrado|Must|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US03|Eu, como desenvolvedor, desejo poder criar uma rota para edição de dados do usuário, para que o mesmo possa mudar informações de seu cadastro|Could|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US04|Eu, como desenvolvedor, desejo poder ser capaz de deletar usuários do banco, para que eu possa retirar possíveis usuários da aplicação|[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US05|Eu, como usuário, desejo me cadastrar no Eccoar para que eu possa realizar anúncios e denúncias de problemas em minha comunidade||[Análise do Backlog](https://docs.google.com/spreadsheets/d/1BWgLcNVli3B1-w7T_7j1X5dLGAuc9UeXKd8Q0DTE0Eg/edit#gid=0)|
|US06|Eu, como usuário, desejo visualizar meu perfil, para que eu possa ter noção de meus dados e informações relativas a minha conta|Could|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Brainstorm](https://miro.com/app/board/o9J_lVC-W9A=/?moveToWidget=3074457354169336052&cot=14)|
|US07|Eu, como usuário, desejo poder editar meu perfil, para que eu possa alterar informações básicas e essenciais da minha conta|Could|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Brainstorm](https://miro.com/app/board/o9J_lVC-W9A=/?moveToWidget=3074457354169336052&cot=14)|
|US08|Eu, como usuário, desejo poder deletar minha conta, caso eu deseje me desvincular do aplicativo e cerrar minhas atividades no mesmo|Could|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Brainstorm](https://miro.com/app/board/o9J_lVC-W9A=/?moveToWidget=3074457354169336052&cot=14)|

### Feature 02 - Interalção de usuário

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US09|Eu, como usuário, desejo ver informações básicas de negócio e funcionamento do sistema em uma landing page, para que eu possa entender melhor seu funcionamento|Should|[Lean](https://app.mural.co/t/fgaepsmds202027717/m/fgaepsmds202027717/1613056199650/dc36dda8d33d71de5a9c01f907d758d2d2b109eb),[Brainstorm](https://miro.com/app/board/o9J_lVC-W9A=/?moveToWidget=3074457354169336052&cot=14)|
|US10|Eu, como usuário, desejo poder ver informações de legislação sobre o assunto, para que eu possa me informar sobre a ação do estado e dos orgãos responsáveis|Would|[Pergunta 8.1]()
|US11|Eu, como usuário, desejo poder ver informações e elementos lúdicos e que me motivem a continuar utilizando a plataforma|Could|[Pergunta 8.1](https://docs.google.com/forms/d/1nR_GXzUPexrl8MHE9hvB0abfEM2osplWkIA6OWhR6_A/edit#responses)
|US12|Eu, como desenvolvedor, desejo ter um canal de comunicação com o usuário, para que eu possa tirar dúvidas com o mesmo sobre a aplicação|Could|[Pergunta 8.1](https://docs.google.com/forms/d/1nR_GXzUPexrl8MHE9hvB0abfEM2osplWkIA6OWhR6_A/edit#responses)
|US13|Eu, como usuário, desejo me comunicar com a equipe de desenvolvimento do software, para que eu possa tirar dúvidas e resolver problemas|Could|[Pergunta 8.1](https://docs.google.com/forms/d/1nR_GXzUPexrl8MHE9hvB0abfEM2osplWkIA6OWhR6_A/edit#responses)
|US14|Eu, como usuário, desejo ver em minha página de perfil, informações sobre os problemas que ajudei a resolver, sendo em votação, denúncia, confirmação de solução, para que eu possa ver em dados minha contribuição para minha sociedade|Could|[Perfil de usuário, COLAB](https://app.colab.re/user/356534)|

## Épico 02 - Denúncia

### Feature 03 - CRUD de denúncia]

|ID|História de Usuário|Prioridade|Rastro|
|--|--|--|--|
|US15|Eu, como desenvolvedor, desejo salvar no banco informações sobre uma denúncia, com os dados: Denúncia {id, nome, imagem, descrição, latitude, longitude, categoria, data de criação, data de fechamento, status e id de usuário} Votos {id da denúncia, id do usuário}|Must|[Perguntas 2, 3 e 8.1](https://docs.google.com/forms/d/1nR_GXzUPexrl8MHE9hvB0abfEM2osplWkIA6OWhR6_A/edit#responses)|
|US16|Eu, como usuário, desejo poder preencher um formulário para que eu possa registrar minha denúncia|Must|[Perguntas 2, 3 e 8.1](https://docs.google.com/forms/d/1nR_GXzUPexrl8MHE9hvB0abfEM2osplWkIA6OWhR6_A/edit#responses)|
|US17|Eu, como usuário, desejo categorizar minha denúncia, para que eu tenha a certeza que a mesma está sendo enviada para o orgão correto|Should|[Pergunta 8.1]()|
|US18|Eu, como usuário, desejo ter a opção de fazer denúncias sem foto, para que eu possa agilizar o processo de denúncia|Must|[Lean](),[brainstorm]()|
|US19|Eu, como usuário, desejo poder tirar uma foto dentro do próprio aplicativo para postar em minha denúncia, para que eu possa realizar a mesma de maneira rápida|Could|[US12]()|
|US20|Eu, como desenvolvedor, desejo poder ser capaz de deletar denúncias do banco, para que eu possa retirar possíveis denúncias inválidas da aplicação|Could|[Análise do Backlog]()|
|US21|Eu, como usuário, desejo poder deletar minha denúncia, caso eu sinta que a mesma não foi justificada ou tenha me enganado quanto ao seu teor|Could|[Lean](),[brainstorm]()|
|US22|Eu, como desenvolvedor, desejo poder ser capaz de alterar dados das denúncias no banco, para que o usuário possa alterar informações essenciais da mesma|Could|[Análise do Backlog]()|
|US23|Eu, como usuário, desejo poder editar minha denúncia, para que eu possa editar informações sobre a mesma, caso sinta que seja necessário ou que algo tenha mudado|Could|[Lean](),[brainstorm]()|
|US24|Eu, como desenvolvedor, desejo poder ser capaz de ver do banco as denúncias criadas por usuário, para que o mesmo possa ter acesso a elas em seu sistema|Must|[Análise do Backlog]()|
|US25|Eu, como usuário, desejo poder ver as denúncias que criei, para que eu possa acompanhar seu andamento, comentários|Must|[Colab, feed de notícias]()|
|US26|Eu, como desenvolvedor, desejo poder ser capaz de ver do banco todas as denúncias criadas pelos usuários, para que o mesmo possa ter acesso a elas no feed de denúncias|Must|[Análise do Backlog]()|
|US27|Eu, como usuário, desejo poder ver o feed de denúncias, para que eu possa ver as denúncias na página principal do sistema|Must|[Análise do Backlog]()|
|US28|Eu, como desenvolvedor, desejo poder acessar os dados de uma denúncia a partir de seu ID, para que eu possa focar nas informações providas na mesma|Should|[Análise do Backlog]()|