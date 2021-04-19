# Contribuindo para o projeto 🎈

Adoramos a contribuição de novas pessoas! Gostaríamos de transformar a contribuição desse projeto na mais fácil possível. E adoramos todos os tipos de contribuição, seja:

- Reportando um _bug_;
- Enviando correções de _bugs_;
- Enviando propostas de correções visuais;
- Propondo novas funcionalidades;

Precisa tirar alguma dúvida ou precisa de alguma inspiração? Conheça a nossa [Documentação](https://fga-eps-mds.github.io/EPS-2020-2-G2/).

# Como iniciar o seu processo de Contribuição? 🎉

Para contribuir com o projeto você pode estar abrindo _issues_ de sugestões e reports de acordo com o nosso [template](https://github.com/fga-eps-mds/EPS-2020-2-G2/blob/main/.github/ISSUE_TEMPLATE/issue-template.md). Ou você pode estar contribuindo para o nosso código. Basta seguir os seguintes passos:

- Abra uma _issue_ em nosso repositório, seguindo o nosso [template](https://github.com/fga-eps-mds/EPS-2020-2-G2/blob/main/.github/ISSUE_TEMPLATE/issue-template.md);
  - Se você só quer resolver uma _issue_ já aberta no respositório, se marque na _issue_ e comente nela (Atenção: Certifique-se de que não existe um responsável por essa _issue_ antes);
- Faça um _fork_ do nosso projeto, se você for um contribuidor externo;
- Crie uma _branch_ a partir da develop, seguindo a nossa [política de _branch_](#politica-de-branch);
- Crie um _Pull Request_ com o status de **_WIP_**, no repositório para certificarmos que você está trabalhando na _issue_;
- Siga a [política de _commits_](#politica-de-commits) durante o desenvolvimento;
- Ao final do desenvolvimento cetifique-se que seu código está funcionando e os testes passando;
- Ao concluir o desenvolvimento, edite o seu _Pull Request_ removendo o status de **_WIP_** e seguindo o nosso [template padrão para _pull request_]().

# Política de _Branches_ 🧠

A nossa política de _Branches_ é baseada no [_GitHub flow_](https://guides.github.com/introduction/flow/).

Utilizamos dessa forma as seguintes _branches_:

## **main**

É a _branch_ principal do projeto, ela é usada tanto para o ambiente de Homologação quanto o ambiente de Produção.

Existe somente uma regra para essa _branch_, que o código nela deve ser sempre possível de realizar o deploy.

Quando um novo código vai para essa _branch_ o deploy é realizado automaticamente para o ambiente de Homologação e caso uma tag seja gerada a partir dessa branch, irá automaticamente para o ambiente de Produção.

Todos os _commits_ diretos nessa _branch_ estão bloqueados, sendo acessível apenas através de _Pull Requests_.

### **_Nomeclatura_**

As _features_ _branches_ devem seguir o seguinte padrão de nome `id_nome_issue`.

**Exemplo**: Na _issue_ **_Criar Guia de Contribuição do Projeto #2_**, você deverá nomear a branch da seguinte forma: `2_criar_guia_contribuicao`.

As _hotfix_ _branches_ devem seguir o seguinte padrão de nome `hotfix_id_nome_issue`.

**Exemplo**: Na _issue_ **_Corrigir Bug no Login #221_**, você deverá nomear a _branch_ da seguinte forma: `hotfix_221_corrigir_bug_login`.

Já as _releases_ _branches_ devem seguir o seguinte padrão de nome
`release/numero_de_versao`.

### **_Branches_ Atualizadas**

Sempre mantenha a sua _branch_ atualizada com a _branch_ de origem.
Recomendamos a utilização do comando _rebase_ para isso.

**Exemplo**:

```
> git pull --rebase origin branch_origem
```

# Política de _Commits_ ☄️

Seguimos os seguintes padrões na nossa política de _commits_:

- Realize o seu _commit_ em inglês.
- Ele deve descrever de forma objetiva o que você fez.
- Evite _commits_ desnecessários.
- Evite coisas como "_This commit..._" ou "_I have..._"
- Utilize as frases no imperativo.

**Exemplo**:

```
> git commit -m "Create route to get report"
```

Caso você esteja em um _pair programming_ utilize o _co-authored-by_ para poder atribuir reconhecimento para o seu colega de trabalho.
Basta seguir os seguintes comandos:

```
> git commit
```

Isso irá abrir o seu editor de texto padrão. A partir disso edite o conteúdo que estiver dentro para algo parecido com:

```
Create route to get report


Co-authored-by: Kazuma Kiryu <kiryu.dragon.2020@email.com>
```

Dessa forma o _commit_ será atribuido para ambos desenvolvedores.
