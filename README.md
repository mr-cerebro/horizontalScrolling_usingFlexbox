<h1 align="center">Como criar uma rolagem horizontal usando Flexbox</h1>

## 💻 Projeto

<p align="center">
    <img src="./assets/img/1_8MiXDWg3C4evyq1WtRWTcw.png"/>
</p>

Se você desenvolve sites para web, certamente já precisou criar componentes com rolagem horizontal. Com o Flexbox, criar essa barra de rolagem é muito simples. Basta escrever apenas algumas linhas de código. Vou mostrar para você como fazer isso neste artigo.

## 🔖 Layout do Projeto

```html
    <div class="container">
        <img src="./assets/img/source.unsplash.com/random?a=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?b=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?c=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?e=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?f=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?g=1" alt="">
        <img src="./assets/img/source.unsplash.com/random?h=1" alt="">
    </div>
```

## Estilização do projeto

O próximo passo é adicionar o estilo para que o contêiner role horizontalmente. Para isso, vamos adicionar ``display: flex`` ao contêiner. Além disso, estou definindo o valor ``overflow-x`` como auto. Abaixo temos o código pronto já com os estilos:

```css
    .container {
        display: flex;
        overflow-x: auto;
    }
```

A rolagem horizontal deverá ficar dessa maneira:

<p align="center">
    <img src="./assets/img/modelo.gif"/>
</p>

<small align="center">A versão inicial de nossa rolagem horizontal</small>

Isso já faz com que nossas imagens rolem horizontalmente. Eu, no entanto, não estou muito satisfeito com a aparência. Há três coisas que quero mudar:

- Adicionar um espaçamento entre as imagens.
- Esconder a barra horizontal.
- Centralizar as imagens na tela.

Vamos começar adicionando um espaçamento entre as imagens. Para isso, vamos adicionar uma margem à direita de 15px. Aqui está o código do CSS:

```css
    .container img {
        margin-right: 15px;
    }
```

Em seguida, quero esconder a barra de rolagem horizontal e podemos fazer isso usando o código abaixo:

```css
    .container::-webkit-scrollbar {
        display: none;
    }
```
A última mudança que quero fazer é centralizar as imagens no centro da tela. Por padrão, a altura do html é a altura de seus elementos. Então, precisamos fazer com que a altura do html seja de 100% da viewport.

Com o Flexbox, podemos centralizar itens usando a propriedade ``align-items``. Para utilizarmos essa propriedade, precisamos adicionar ``display: flex`` no elemento ``body`` do nosso html. Aqui está o código que adicionaremos ao nosso body:

```css
    body {
        display: flex;
        align-items: center;
        height: 100vh;
    }
```
Com essas mudanças, esse será o resultado final da nossa barra de rolagem utilizando o Flexbox e escrevendo apenas algumas linhas de código:

<p align="center">
    <img src="./assets/img/qJCD4OP64IdYdHTGPKnFVBKhFLrkiIWDrKSe.gif"/>
</p>

## Conclusão

Com o Flexbox, é muito fácil criar uma barra de rolagem horizontal. Muito obrigado por ler até o final! :)