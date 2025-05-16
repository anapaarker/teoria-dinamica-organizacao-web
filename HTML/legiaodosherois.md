## A Semântica por Trás da Apresentação: Desvendando a Estrutura Textual em HTML

## Atividade: 

*1-Análise da Estrutura Textual de Páginas Web (Individual)*

*Página 1:* https://www.legiaodosherois.com.br/ (Site de notícias de entretenimento e cultura geek pop).

Utilizando a ferramenta de ''inspecionar elemento'', temos:

```html
<h2>Quarteto Fantástico: linha da Funko revela spoiler do filme</h2>
```
A tag `<h2>` é usada para os títulos das notícias na página inicial, indicando seções importantes do conteúdo.

```html
<p>Visual de um personagem foi revelado na coleção do filme.</p>
```
A tag `<p>`  é usada para os resumos das notícias, trazendo uma descrição do conteúdo apresentado.

```html
<strong>Importante:</strong> Leve guarda-chuva mesmo assim!
```
A tag `<strong>` é usada para enfatizar informações importantes dentro do texto.

````html
<em>Isso é só uma recomendação!</em>
````
A tag `<em>`  adiciona ênfase leve a determinadas palavras ou frases, geralmente exibidas em itálico.

```html
Primeira linha.<br>Segunda linha.
```
A tag `<br>` é usada para quebrar linhas dentro de um parágrafo, controlando a apresentação do texto.

```html
<hr>
```
A tag `<hr>` é usada para separar visualmente diferentes seções ou tópicos na página.

*2-Explorando a Organização com Listas (Individual)*

As tags `<ul>` e `<li>` são usadas para listar itens sem uma ordem específica, como categorias ou tópicos relacionados.

```html
<ul>
  <li>Filmes</li>
  <li>Séries</li>
  <li>Quadrinhos</li>
</ul>
```
*3-A Expressão de Citações (Individual)*

A tag `<blockquote>` é usada para destacar citações longas de entrevistas ou declarações de autores.

```html
<blockquote>
  "Este é o melhor filme do ano", disse o diretor.
</blockquote>
```
A tag `<q>`é usada para citações curtas dentro de um parágrafo.

```html
<p>O ator afirmou que <q>o papel foi desafiador</q> durante a coletiva.</p>
```
**O código da estrutura exemplificada com os elementos semânticos analisados, fica assim:**
````html

<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Notícia - Legião dos Heróis</title>
</head>
<body>
  <h1>Quarteto Fantástico: Novo Visual Revelado</h1>
  <h2>Personagem Surpreende Fãs</h2>
  <p>O <strong>visual inédito</strong> de um dos personagens foi <em>revelado</em> pela nova linha de brinquedos.</p>
  <p>Confira abaixo os detalhes:<br>Imagens exclusivas e mais informações.</p>
  <hr>
  <h3>Principais Destaques</h3>
  <ul>
    <li>Design moderno</li>
    <li>Referências aos quadrinhos</li>
    <li>Expectativas para o filme</li>
  </ul>
  <h4>Ordem de Eventos</h4>
  <ol>
    <li>Vazamento das imagens</li>
    <li>Reações dos fãs</li>
    <li>Confirmação oficial</li>
  </ol>
  <h5>Glossário</h5>
  <dl>
    <dt>Funko</dt>
    <dd>Empresa de colecionáveis conhecida por seus bonecos estilizados.</dd>
    <dt>Marvel</dt>
    <dd>Editora responsável pelo Quarteto Fantástico.</dd>
  </dl>
  <h6>Depoimento</h6>
  <blockquote cite="https://legiaodosherois.com.br">
    "Este é o melhor visual que já vimos até agora", afirmou o diretor.
  </blockquote>
  <p>O ator comentou: <q>Estou animado para que todos vejam o resultado final.</q></p>
</body>
</html>
````
