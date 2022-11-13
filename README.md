<h1 align="center">Como criar uma rolagem horizontal usando Flexbox</h1>

## 💻 Projeto

<p align="center">
    <img src="./assets/img/1_8MiXDWg3C4evyq1WtRWTcw.png"/>
</p>

Se você desenvolve sites para web, certamente já precisou criar componentes com rolagem horizontal. Com o Flexbox, criar essa barra de rolagem é muito simples. Basta escrever apenas algumas linhas de código. Vou mostrar para você como fazer isso neste artigo.

## 🔖 Layout do Projeto

```
    <div class="container">
        <img src="./assets/img/source.unsplash.com/random?a=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?b=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?c=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?e=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?f=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?g=1" alt="">
        <img src="./assets/imgsource.unsplash.com/random?h=1" alt="">
    </div>
```

## Estilização do projeto

O próximo passo é adicionar o estilo para que o contêiner role horizontalmente. Para isso, vamos adicionar ``display: flex`` ao contêiner. Além disso, estou definindo o valor ``overflow-x`` como auto. Abaixo temos o código pronto já com os estilos: