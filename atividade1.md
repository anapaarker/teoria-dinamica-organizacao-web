# Atividade 1 – Descrevendo Efeitos Visuais com JavaScript

## Como o JavaScript é utilizado para criar efeitos visuais em páginas web

O JavaScript é uma linguagem de programação usada para tornar as páginas web interativas. Um dos seus principais usos é criar **efeitos visuais dinâmicos** que melhoram a experiência do usuário. Esses efeitos vão desde **animações simples** (como mover uma imagem ou mudar uma cor) até **transições mais complexas**, como sliders, menus animados, janelas modais, e muito mais.

### JavaScript + CSS: como funcionam juntos

O JavaScript consegue **interagir com o CSS** para modificar o estilo de elementos HTML de forma dinâmica, ou seja, enquanto a página já está carregada no navegador. Isso acontece por meio do acesso ao **DOM (Document Object Model)**, que representa os elementos da página.

Por exemplo, o JavaScript pode alterar a cor de fundo de uma caixa quando o usuário passa o mouse sobre ela:

```javascript
document.getElementById("minhaCaixa").style.backgroundColor = "blue";

*Animações simples no navegador*
Animações simples podem ser feitas com JavaScript puro, controlando o tempo e o estilo dos elementos com funções como setInterval, setTimeout e requestAnimationFrame. Um exemplo seria mover um quadrado para a direita gradualmente:

let box = document.getElementById("box");
let pos = 0;
let id = setInterval(() => {
  if (pos >= 300) {
    clearInterval(id);
  } else {
    pos++;
    box.style.left = pos + "px";
  }
}, 10);
Essa técnica é útil para animações leves e personalizadas.

*Uso de bibliotecas JavaScript para efeitos mais avançados*
Para efeitos mais complexos e sofisticados, é comum usar bibliotecas JavaScript, como:

jQuery: facilita a criação de animações com comandos simples.
Por exemplo:
$("#minhaCaixa").fadeOut();


GSAP (GreenSock Animation Platform): permite criar animações profissionais com ótimo desempenho. Exemplo:
gsap.to("#caixa", {x: 100, duration: 2});

Referências
https://developer.mozilla.org/pt-BR/docs/Web/JavaScript

https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/DOM_scripting

https://www.w3schools.com/js/js_htmldom_animate.asp

https://api.jquery.com/

https://gsap.com/
