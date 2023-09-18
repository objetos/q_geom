---
weight: 6
draft: false
---

# `reflect()`

Horizontal reflection of the quadrille cells.

# Example

(mouse click or press any key to `reflect` the quadrille)  
{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" width="425" height="425" >}}
`use strict`;
let quadrille;

function setup() {
  createCanvas(4 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  quadrille = createQuadrille(4, 4, 3, '🚀');
  quadrille.rand(4, '🐒');
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}

function mouseClicked() {
  quadrille.reflect();  
}

function keyPressed() {
  quadrille.reflect();
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
let quadrille;

function setup() {
  createCanvas(4 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  quadrille = createQuadrille(4, 4, 3, '🚀');
  quadrille.rand(4, '🐒');
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}

function mouseClicked() {
  quadrille.reflect();  
}

function keyPressed() {
  quadrille.reflect();
}
```
{{< /details >}}

# Syntax

> `reflect()`