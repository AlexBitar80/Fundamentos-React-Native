<h3 align="center">
	<img src="https://user-images.githubusercontent.com/56983783/102695094-fce2f700-4203-11eb-9098-59e52f94572c.png" alt="GoMarketplace"/>
</h3>

<p align="center">
  Desafio que se coinsistia em completar o código de uma aplicação mobile, o GoMarketplace uma aplicação de vendas que possui um carrinho de comprar e produtos que podem ser adicionados a ele, com as funcionalidades de adicionar e remover do carrinho fazendo a soma dos produtos e salvadno todos no storage.
</p>

<p align="center">
  <img alt="GitHub watchers" src="https://img.shields.io/github/watchers/AlexBitar80/Fundamentos-React-Native?style=social">

  <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/AlexBitar80/Fundamentos-React-Native">

  <img alt="GitHub Repo stars" src="https://img.shields.io/github/stars/AlexBitar80/Fundamentos-React-Native?style=social">

  <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/AlexBitar80/Fundamentos-React-Native">

  <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/AlexBitar80/Fundamentos-React-Native">
</p>

<p align="center">
  <a href="#star-como-rodar">Como usar</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;

  <a href="#rocket-testes">Testes</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;

  <a href="#gear-tecnologias-usadas-neste-projeto">Tecnologias</a>
</p>

<h3 align="center">
  <img width="246" height="533" src="https://user-images.githubusercontent.com/56983783/102694957-26e7e980-4203-11eb-975f-0ac0e1876020.gif" alt="app GoMarketplace"/>
</h3>

## :gear: Tecnologias usadas neste projeto

O projeto está utilizando as seguintes tecnologias:

-  [typescript](https://www.typescriptlang.org/)
-  [react-native](https://reactnative.dev/)
-  [jest](https://jestjs.io/)
-  [react-native-vector-icons](https://www.npmjs.com/package/react-native-vector-icons)
-  [async-storage](https://github.com/react-native-async-storage/async-storage)
-  [axios](https://www.npmjs.com/package/axios)
-  [json-server](https://www.npmjs.com/package/json-server)
-  [styled-components](https://styled-components.com/)
-  [react-navigation](https://reactnavigation.org/)
-  [react-icons](https://react-icons.github.io/react-icons/)


## :rocket: Testes

Para esse desafio, temos os seguintes testes:

- **`should be able to list the products`**: Para que esse teste passe, sua aplicação deve permitir que sejam listados na sua tela `Dashboard`, todos os produtos que são retornadas do Fake API. Essa listagem deve exibir o `title` e o `price` que deve ser formatado utilizando a função `Intl`.

- **`should be able to add a product to the cart`**: Para que esse teste passe, você deve permitir que seja possível adicionar produtos da sua `Dashboard` ao carrinho, utilizando o contexto de `cart` disponibilizado.

- **`should be able to list the products on the cart`**: Para que esse teste passe, você deve permitir que seja possível listar os produtos que estão salvos no contexto do seu carrinho na página `Cart`, nessa página exiba o nome do produto e o subtotal total de cada produto (price \* quantity).

- **`should be able to calculate the cart total`**: Para que esse teste passe, tanto na página `Dashboard`, tanto na página `Cart` você deve exibir o valor total de todos os itens que estão no seu carrinho.

- **`should be able to show the total quantity of itens in the cart`**: Para que esse teste passe, tanto na página `Dashboard`, tanto na página `Cart` você deve exibir o número total de itens que estão no seu carrinho.

- **`should be able to increment product quantity on the cart`**: Para que esse teste passe, você deve permitir que seja possível incrementar a quantidade de um produto do seu carrinho, utilizando o contexto de `cart` disponibilizado.

- **`should be able to decrement product quantity on the cart`**: Para que esse teste passe, você deve permitir que seja possível decrementar a quantidade de um produto do seu carrinho, utilizando o contexto de `cart` disponibilizado.

- **`should be able to navigate to the cart`**: Para que esse teste passe, no seu componente `FloatingCart` na Dashboard, você deve permitir que ao clicar no botão de carrinho com o testID de `navigate-to-cart-button`, o usuário seja redirecionado para a página `Cart`.

- **`should be able to add products to the cart`**: Para que esse teste passe, no seu arquivo onde contém o contexto do carrinho, você deve permitir que a função `addToCart` adicione um novo item ao carrinho.

- **`should be able to increment quantity`**: Para que esse teste passe, no seu arquivo onde contém o contexto do carrinho, você deve permitir que a função `increment` incremente em `1` unidade a quantidade de um item que está armazenado no contexto.

- **`should be able to decrement quantity`**: Para que esse teste passe, no seu arquivo onde contém o contexto do carrinho, você deve permitir que a função `decrement` decremente em `1` unidade a quantidade de um item que está armazenado no contexto.

- **`should store products in AsyncStorage while adding, incrementing and decrementing`**: Para que esse teste passe, no seu arquivo onde contém o contexto do carrinho você deve permitir que todas as atualizações que você fizer no carrinho, sejam salvas no AsyncStorage. Por exemplo, ao adicionar um item ao carrinho, adicione-o também no AsyncStorage. Lembre de também atualizar o valor do AsyncStorage quando você incrementar ou decrementar a quantidade de um item.

- **`should load products from AsyncStorage`**: Para que esse teste passe, no seu arquivo onde contém o contexto do carrinho, você deve permitir que todos os produtos que foram adicionados sejam buscados do AsyncStorage.

## :star: Como rodar

Para clonar e rodar esse projeto você vai precisar do [Node](https://nodejs.org/en/) do [Yarn](https://yarnpkg.com/) do [Npm](https://www.npmjs.com/get-npm) e do [Git](https://git-scm.com/) instalado na rua máquina



```bash
# Faça o clone deste repositório para qualquer pasta de sua preferencia
$ git clone https://github.com/AlexBitar80/Fundamentos-React-Native Fundamentos-React-Native

# Vá até essa pasta
$ cd Fundamentos-React-Native

# rode esses comandos para instalar as dependências
$ yarn || npm install

# use esses comandos para rodar o Projeto no seu emulador do android
$ yarn android || npm run android

# use esses comandos caso esteja utilizando o emulador do iOS
$ yarn ios || npm run ios

# use esses comandos para rodas os testes
$ yarn test || npm run test
```

por padrão assim que o comando para rodar no emulador for iniciado ele ira abrir uma segundo aba do terminal com o Metro Bundler que server para ficar monitorando e atualizando o app mobile, mas poder haver casos onde ele por padrão não irá abrir essa segunda aba, nesses casos basta rodar esses comandos abaixo

```bash
  $ yarn start || npm run start
```
