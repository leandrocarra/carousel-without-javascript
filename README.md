# Carousel Without Javascript

Um carousel feito somente com css, pode ser usado em sites normais, mobile e responsivos.

## Pré-requisito

Pre-processador scss

## Como funciona

O carousel em css funciona, nesse caso, atribuindo valores do label ao id do radio.
Logo, se for clicado no label com for "exemplo" para o radio id "exemplo" o radio será checked.

Exemplo:
```html
<label for="exemplo">CLIQUE AQUI</label>
<input id="exemplo" name="carousel" />

<label for="outroExemplo">CLIQUE AQUI</label>
<input id="outroExemplo" name="carousel" />
```
O que vai acontecer aqui é que mesmo que seja clicado nas opções, somente um radio será checked por causa da propriedade
name, que recebe o identificador carousel.

A magica acontece justamente aqui.

Cada label está atrelado ao seu radio, e todos os radios com o mesmo name, fazendo com que apenas um seja checked.

No css basta ocultar todos que n forem checked, e na regra para checked faze-lo aparecer.

Mas isso tudo funcionará automatico se o exemplo for seguido.

## Como usar

No html vc deve ter algo que traga a quantidade do lenght do array. Para que funcione automaticamente, vc deve sincronizar o scss com a quantidade de itens no array.

No scss a var
```scss
$end : xx;
````
espera receber quantas vezes o loop vai criar as classes que irão controlar o next e o prev do carousel, então é só ter esses numeros em mãos e adicionar lá.

Uma vez com a quantidade do array no html, basta apenas seguir o exemplo no index.html e tudo funcionará.

### Veja o exemplo completo
https://goo.gl/QviTb8
