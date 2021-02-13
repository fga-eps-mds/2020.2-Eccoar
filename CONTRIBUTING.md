# Contribuindo para o projeto 🎈 

Adoramos a contribuição de novas pessoas! Gostaríamos de transformar a contribuição desse projeto na mais fácil possível. E adoramos todos os tipos de contribuição, seja:

* Reportando um *bug*;
* Enviando correções de *bugs*;
* Enviando propostas de correções visuais;
* Propondo novas funcionalidades;

Precisa tirar alguma dúvida ou precisa de alguma inspiração? Conheça a nossa [Documentação](https://fga-eps-mds.github.io/EPS-2020-2-G2/).

# Como iniciar o seu processo de Contribuição? 🎉 

Para contribuir com o projeto você pode estar abrindo *issues* de sugestões e reports de acordo com o nosso [template](https://github.com/fga-eps-mds/EPS-2020-2-G2/blob/main/.github/ISSUE_TEMPLATE/issue-template.md). Ou você pode estar contribuindo para o nosso código. Basta seguir os seguintes passos:

* Abra uma *issue* em nosso repositório, seguindo o nosso [template](https://github.com/fga-eps-mds/EPS-2020-2-G2/blob/main/.github/ISSUE_TEMPLATE/issue-template.md);
    * Se você só quer resolver uma *issue* já aberta no respositório, se marque na *issue* e comente nela (Atenção: Certifique-se de que não existe um responsável por essa *issue* antes); 
* Faça um *fork* do nosso projeto, se você for um contribuidor externo;
* Crie uma *branch* a partir da develop, seguindo a nossa [política de *branch*](#politica-de-branch);
* Crie um *Pull Request* com o status de ***WIP***, no repositório para certificarmos que você está trabalhando na *issue*;
* Siga a [política de *commits*](#politica-de-commits) durante o desenvolvimento;
* Ao final do desenvolvimento cetifique-se que seu código está funcionando e os testes passando;
* Ao concluir o desenvolvimento, edite o seu *Pull Request* removendo o status de ***WIP*** e seguindo o nosso [template padrão para *pull request*]().

# Política de *Branches* 🧠 

A nossa política de *Branches* é baseada no [*Gitflow*](https://www.atlassian.com/br/git/tutorials/comparing-workflows/gitflow-workflow).

Utilizamos dessa forma as seguintes *branches*:

## **main**
A *branch* do nosso ambiente de Produção. Aqui é a *branch* com o código mais estável do projeto. Todos os *commits* diretos nessa *branch* estão bloqueados.

## **develop**
A *branch* do nosso ambiente de Homologação.Essa é a *branch* de integração das novas funcionalidades. Toda nova funcionalidade deve ser desenvolvida a partir dessa *branch*.

### ***Nomeclatura***
As *features* *branches* devem seguir o seguinte padrão de nome `id_nome_issue`.

**Exemplo**: Na *issue* ***Criar Guia de Contribuição do Projeto #2***, você deverá nomear a branch da seguinte forma: `2_criar_guia_contribuicao`.

As *hotfix* *branches* devem seguir o seguinte padrão de nome `hotfix_id_nome_issue`. 

**Exemplo**: Na *issue* ***Corrigir Bug no Login #221***, você deverá nomear a *branch* da seguinte forma: `hotfix_221_corrigir_bug_login`.

Já as *releases* *branches* devem seguir o seguinte padrão de nome
`release/numero_de_versao`.

### ***Branches* Atualizadas**
Sempre mantenha a sua *branch* atualizada com a *branch* de origem.
Recomendamos a utilização do comando *rebase* para isso.

**Exemplo**:  
```
> git pull --rebase origin branch_origem
```

# Política de *Commits* ☄️ 

Seguimos os seguintes padrões na nossa política de *commits*:
* Realize o seu *commit* em inglês. 
* Ele deve descrever de forma objetiva o que você fez. 
* Evite *commits* desnecessários.
* Evite coisas como "*This commit...*" ou "*I have...*"
* Utilize as frases no imperativo.

**Exemplo**:
```
> git commit -m "Create route to get report"
```

Caso você esteja em um *pair programming* utilize o *co-authored-by* para poder atribuir reconhecimento para o seu colega de trabalho.
Basta seguir os seguintes comandos:
```
> git commit
```
Isso irá abrir o seu editor de texto padrão. A partir disso edite o conteúdo que estiver dentro para algo parecido com:
```
Create route to get report


Co-authored-by: Kazuma Kiryu <kiryu.dragon.2020@email.com>
```

Dessa forma o *commit* será atribuido para ambos desenvolvedores.