# Testes

## Histórico de revisão

| Autor                                | Mudanças             | Data       | Versão |
| ------------------------------------ | -------------------- | ---------- | ------ |
| [Pedro Féo](https://github.com/phe0) | Criação do documento | 13/03/2021 | 1.0    |

Os testes no ambiente do frontend serão feitos utilizando dois pacotes:

- react-testing-library
- jest

## Como rodar

Para rodar a suite de testes: `npm test`

Para buildar o coverage de testes da aplicação: `npm run coverage`

## Como realizar testes

Libs para serem importadas:

`import React from 'react'; // React`

`import { render, screen } from '@testing-library/react'; // feramentas do react-testing-lib para renderizar e manuzear os elementos`

`import userEvent from '@testing-library/user-event'; // ferramenta do react-testing-lib para forjar interações com a interface`

`import Button from '../../components/Button'; // o componente a ser testado`

### Declarando uma suíte de testes

```
describe('Nome da suite de testes', () => {
    // declarar de 1 a N testes aqui dentro
})
```

### Declarando um teste

```
describe('Nome da suite de testes', () => {
    test('Nome do teste', () => {
        // regras do teste
        expect(true).toBe(true);
        //expect é uma função wrapper que deve estar em volta do elemento a ser analizado, toBe é uma função que nos permite dizer qual é o valor esperado para o elemento
    })
})
```

### Renderizando um componente

O componente é renderizando se utilizando a função render

```
describe('Nome da suite de testes', () => {
    test('Nome do teste', () => {
        render(<Componente />);

        screen.debug() // essa função não é necessária, mas ela mostra o html renderizado ao rodar npm test, pode ajudar bastante na hora de escrever os testes
    })
})
```

### Como selecionar elementos para testar

Depois de renderizar seu componente, a react-testing-lib oferece algumas funções
para selecionar elementos. Esses elementos serão usados depois para realizar
_assertions_(verificar ma funcionalidade) ou interações de usuário.

No exemplo abaixo usamos o seletor _getByText_, ele procura um elemento que
possua o texto passado como parametro, no caso "testing".

```
describe('Nome da suite de testes', () => {
    test('Nome do teste', () => {
        render(<Button text="testing" />);

        expect(screen.getByText("testing"));
    })
})
```

Agora podemos adicionar uma _assertion_ para verificar se existe um elemento na
tela com esse texto.

```
describe('Nome da suite de testes', () => {
    test('Nome do teste', () => {
        render(<Button text="testing" />);

        expect(screen.getByText("testing")).toBeInTheDocument();
    })
})
```

No exemplo acima usamos a função _getByText_ para selecionar o elemento, porém
existem outras funções que podem ser usadas.

Você pode ver as demais funções na documentação do pacote,
[aqui](https://testing-library.com/docs/queries/about/).

Além dessas, existem variantes nos seletores, que são destacados pelas palavras
_getBy_, _queryBy_ e _findBy_. Cada uma delas tem usos específicos.

- _getBy_: ela pode retornar um elemento ou um erro, então se você quiser
  testar a falta de um elemento, essa função não é adequada, pois irá falhar
  no seletor em vez de falhar na _assertion_.
- _queryBy_: o _queryBy_ é uma alternativa ao _getBy_, ele não ira retornar um
  erro caso não encontre um elemento, assim você poderá fazer _assertions_
  pela falta de elementos.
- _findBy_: é usado para elementos assíncronos, por exemplo, você pode
  adicionar uma chamada de API quando o componente terminar de renderizar e
  dependendo da resposta ele vai causar uma rerenderização, os seletores
  _getBy_ e _queryBy_ só iriam testar a primeira renderização, enqquanto no
  _findBy_, você poderia fazer algo como `await screen.findByText('loaded')`,
  assim o teste irá parar sua execução, esperando um elemento com o texto
  "loaded".

### Como fazer _assertions_

As _assertion functions_ são funções e que você pode determinar um valor
esperado para um elemento em questão, caso sua _assertion_ não esteja correta,
ela irá retornar um erro.

Assim como os seletores, existem várias opções de _assertions_, que podem ser
úteis dependendo do contexto. Você pode ler mais sobre elas
[aqui](https://github.com/testing-library/jest-dom).

### Como simular eventos

O react-testing-lib oferece uma interface para forjar eventos de usuários,
chamada `userEvents`.

Com ela, você pode executar ações como cliques ou digitação. Segue um exemplo:

```
	test('test click event', () => {
		const onClick = jest.fn(); // mock de uma função de clique
		render(<Button text='testing' onClick={onClick} />);
		userEvent.click(screen.getByText('testing')); // forjando um clique

		expect(onClick).toHaveBeenCalledTimes(1); // fazendo uma assertion para verificar quantas vezes a função de clique foi chamada
	});
```

### Como mockar funções em elementos estáticos

Em alguns casos, elementos vão receber funções como props, nesses casos não é
possível verificar uma mudança na renderização do elemento só por forjar uma
ação do usuário.

Para isso é possível usar o _jest_ para criar uma função que possamos rastrear.
Segue exemplo:

```
	test('test click event', () => {
		// aqui estamos usando o jest para mockar a função de clique, com isso poderemos rastrear as chamadas da função passando onClick como props e usando-a nos assertions
        const onClick = jest.fn();
		render(<Button text='testing' onClick={onClick} />);
		userEvent.click(screen.getByText('testing')); // forjando um clique

		expect(onClick).toHaveBeenCalledTimes(1); // fazendo uma assertion para verificar quantas vezes a função de clique foi chamada
	});
```

### Como mockar chamadas de API

Em alguns casos, o componente a ser testado irá fazer chamadas à uma API, porém
não é ideal que o script de testes realize essas chamadas, pois pode trazer
falhas inesperadas além de poder realizar operações de escrita no banco de
dados. Por isso as chamadas à API devem todas ser mockadas.

Para isso vamos mockar a chamada ao axios utilizando o seguinte trecho de
código: `jest.mock('axios');`

e dentro do teste poderemos usar o mock da seguinte forma:

```
  test('fetches stories from an API and displays them', async () => {
    const stories = [
      { objectID: '1', title: 'Hello' },
      { objectID: '2', title: 'React' },
    ];

    // abaixo o get do axios está sendo mockado, nesse caso ele irá substituir a chamada da API por uma função que irá retornar uma Promise resolvida, que retorna um objeto de resposta.
    // No caso de querer testar uma falha, a Promise deve retornar um Reject com um erro
    axios.get.mockImplementationOnce(() =>
      Promise.resolve({ data: { hits: stories } })
    );

    render(<App />);

    await userEvent.click(screen.getByRole('button'));

    const items = await screen.findAllByRole('listitem');

    expect(items).toHaveLength(2);
  });
```
