# Frontend Mentor - solução do projeto Order summary card

![Design preview do projeto Order summary card coding](./design/desktop-preview.jpg)

Esta é uma solução para o [desafio do Order summary card no Frontend Mentor.](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj) Os desafios do Frontend Mentor ajudam você a melhorar suas habilidades de codificação criando projetos realistas.

## Índice

- [Visão geral](#visão-geral)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [Meu processo](#meu-processo)
  - [Desenvolvido com](#desenvolvido-com)
  - [Como desenvolvi](#como-desenvolvi)
  - [Desenvolvimento contínuo](#desenvolvimento-contínuo)  
- [Autor](#autor)
- [Agradecimentos](#agradecimentos)

## Visão geral

### Screenshot

![](./design/desktop-preview.jpg)

### Links

- [URL da solução no Git](https://github.com/leonardoanselmo/order-summary-component)
- [URL do site](https://order-summary-component-three-pearl.vercel.app/)

## Meu processo

### Desenvolvido com

- HTML5 semântico
- CSS3 propriedades customizadas
- Flexbox

### Como desenvolvi

Antes de começar colocando a mão no código resolvi estruturar o **style.css** resetando as margens e padding, escolhendo o FLEXBOX, pois se tratava apenas de um CARD com todos os elementos abaixo e centralizado e as cores que seriam usadas no projeto em variáveis.

```css
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'Red Hat Display', sans-serif;
}
```

OBS: Veja que deixei o ORDER-SUMMARY centralizado em tamanho e altura. E também a imagem de background, pois no layout mobile a mesma muda.
```css
body {
  margin: 0 auto;
  max-width: 1440px;
  height: 100vh;
  background-image: url('../images/pattern-background-desktop.svg');
  background-repeat: no-repeat;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;  
  ...
}
```

O que eu estou achando complicado é conseguir identificar as cores para o projeto, pois não é disponibilizado o arquivo do FIGMA e muitas das vezes o conta gotas não pega as porcentagens corretas referente a cor.
```css
:root {
  /* Primary */
  --pale-blue: hsl(225, 100%, 94%);
  --bright-blue: hsl(245, 75%, 52%);

  /* Neutral */
  --very-pale-blue: hsl(225, 100%, 98%);
  --desaturated-blue: hsl(224, 23%, 55%);
  --dark-blue: hsl(223, 47%, 23%);
}
```

No HTML escolhi a TAG semântica ``<main></main>`` e ``<footer></footer> `` por saber que é um card isolado e precisava de uma marcação principal para o conteúdo e outra para o footer(rodapé).

Todas as tags incluindo ``<img>``, ``<H2>`` e ``<p>`` foram acrescentadas classes CSS baseado na metodologia BEM.

```html
    <img src="./images/illustration-hero.svg" alt="Imagem Hero" class="c-product-card__img">

    <h1 class="c-product-card__stitle"> ...
    <p class="c-product-card__sparagraph"> ...    
```

### Desenvolvimento contínuo

Essa foi minha segunda experiência com o modelo do [Frontend Mentor](https://www.frontendmentor.io/challenges/order-summary-component-QlPmajDUj), com isso já estou começando a criar um padrão de como começar um projeto, estruturando primeiro o HTML e depois o CSS. Estava ainda com certas dúvidas na metodologia BEM, o que me fez visitar o site e analisar o modelo.

## Autor

- Website - [Léo Ansélmo](https://github.com/leonardoanselmo)
- Frontend Mentor - [@leonardoanselmo](https://www.frontendmentor.io/profile/leonardoanselmo)
- Twitter - [@barblo](https://twitter.com/barblo)

## Agradecimentos

Agradeço a toda equipe do [Frontend Mentor](https://www.frontendmentor.io) por proporcionar um modelo de práticas em desenvolvimento como esse. Logo estarei postando mais projetos aqui! 🚀
