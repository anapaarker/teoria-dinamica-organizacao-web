## A Semântica por Trás da Apresentação: Desvendando a Estrutura Textual em HTML

## Atividade 1: 
*Análise da Estrutura Textual de Páginas Web (Individual)*

*Página 1:* https://www.legiaodosherois.com.br/ (Site de notícias de entretenimento e cultura geek pop).

Utilizando a ferramenta de ''inspecionar elemento'', temos:

A classe para ativar um tema escuro (dark mode, que altera o esquema das cores das telas dos programas) em uma página web, geralmente usando CSS.

```javascript
<body class="bg--enabled theme--dark">:
```
Classe que pode ser utilizada para agrupar elementos para fins de estilos (usando class - ), ou porque eles compartilham valores de atributos, como lang.
Ela deve ser utilizada somente quando não tiver outro elemento de semântica (tal como <  article  > - composição independente em um documento ou <  nav  > - seção de uma página que aponta para outras páginas ou para outras áreas da página):

```javascript
<div class="mobile-fixed-banner">:
```
Estrutura da barra de cabeçalho (header) de um site. Ele contém um elemento <  section  > que encapsula o conteúdo da barra de cabeçalho, com a classe CSS site-header. 
Dentro dessa seção, há um <  div  > com a classe container que define um contêiner para o conteúdo da barra, e um <  div  > com a classe row que utiliza um sistema de grade (  grid  ) para organizar os elementos. Há também o < a >, que são links que permitem aos utilizadores navegar para outra página da web ou para uma secção diferente da mesma página. 

  ````javascript
<section class="site-header">
  <div class="container">
    <div class="row site-header__content">
      <a href="https://www.legiaodosherois.com.br" class="site-header__content__link">
        <img src="//www.legiaodosherois.com.br/wp-content/themes/legiao3.0.0/images/lh-logo/full.svg" width="120" height="22" alt="Logo da Legião">
      </a>
