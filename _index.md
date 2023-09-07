---
bookCollapseSection: true
weight: 8
draft: false
---

# Geometry transformations

Geometry transformations are changes done in a quadrille shape by [rotation]({{< relref "rotate" >}}), [reflection]({{< relref "reflect" >}}) and [transposition]({{< relref "transpose" >}}) of its cells.

{{< hint info >}}
**Observation**\
The methods of this section may be [chained](https://en.wikipedia.org/wiki/Method_chaining), e.g., `quadrille.rotate().reflect().transpose()` which is equivalent to:
```js
quadrille.rotate();
quadrille.reflect();
quadrille.transpose();
```
{{< /hint >}}