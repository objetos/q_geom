---
weight: 6
draft: false
---

# Quadrille geometry transformations

The following quadrille methods define the supported geometry transformations:

1. `rotate()`: performs π/2 clockwise rotation of the quadrille cells.
2. `reflect()`: performs a horizontal reflection of the quadrille cells.
3. `transpose()`: [transposes](https://en.wikipedia.org/wiki/Transpose) the quadrille cells.

(press **r**, **s**, or **t** to `rotate`, `reflect` or `transpose` the quadrille, respectively)
{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" id="number" width="625" height="425" >}}
`use strict`;
let quadrille;

function setup() {
  createCanvas(6 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  const e = '🚀';
  quadrille = createQuadrille(
    [
        [e],
        [e],
        [e, e]
    ]);
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}

function keyPressed() {
  if (key === 'r') {
    quadrille.rotate();
  }
  if (key === 's') {
    quadrille.reflect();
  }
  if (key === 't') {
    quadrille.transpose();
  }
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
let quadrille;

function setup() {
  createCanvas(6 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  const e = '🚀';
  quadrille = createQuadrille(
    [
        [e],
        [e],
        [e, e]
    ]);
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}

function keyPressed() {
  if (key === 'r') {
    quadrille.rotate();
  }
  if (key === 's') {
    quadrille.reflect();
  }
  if (key === 't') {
    quadrille.transpose();
  }
}
```
{{< /details >}}