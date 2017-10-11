# Carousel Without Javascript

Um carousel feito somente com css, pode ser usado em sites mobile e em sites resposivos.

## Preriquisitos

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

No css basta ocultar todos que n forem checked, e na regra pra checked faze-lo aparecer.

### Veja o exemplo completo
https://goo.gl/QviTb8
