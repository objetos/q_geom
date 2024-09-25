---
bookCollapseSection: true
weight: 7
draft: false
---

# Transforms

Transform methods enable the alteration of a quadrille's geometry through operations such as [rotation]({{< relref "rotate" >}}), [reflection]({{< relref "reflect" >}}), and [transposition]({{< relref "transpose" >}}), altering the spatial arrangement of cells.

{{< hint info >}}
**Note:**\
Transformation methods support [method chaining](https://en.wikipedia.org/wiki/Method_chaining), allowing for a streamlined sequence of modifications. For example, chaining `quadrille.rotate().reflect().transpose()` applies a series of transformations succinctly, which is functionally equivalent to:
```js
quadrille.rotate();
quadrille.reflect();
quadrille.transpose();
```
This approach enhances readability and efficiency in code.
{{< /hint >}}