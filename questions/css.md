# CSS questions

<details>
  <summary>What is CSS selector specificity and how does it work?</summary>

  * It is a "rank/score" that determines which style are ultimately applied to an element
  * 1000 - iniline styles
  * 100 - IDs
  * 10 - classes, attributes, pseudo-classes
  * 1 - elements and pseudo-elements
  * `if (equal specifity) the latest rule counts`
</details>

<details>
  <summary>Build simple, css-only modal</summary>

  * [Link to a simple modal I built](https://codepen.io/sitek94/pen/xxEQpVq?editors=1100)
</details>

<details>
  <summary>Describe inline-block element</summary>

  * compared to `inline`: `inline-block` allows us to set width and height
  * with `inline-block` the top and bottom margins/paddings are respected, with `inline`: not
  * compared to `block`: `inline-block` does not add line-break after the element
</details>

<details>
  <summary>What's the difference between a relative, fixed, absolute and statically positioned element?</summary>

  * `static`
    * default value
    * the element is positioned according to the normal flow of the document
    * `top`, `right`, `bottom`, `left`, and `z-index` properties have no effect
  * `relative`
    * the element is positioned according to the normal flow of the document
    * offset relative to itself based on the values of `top`, `right`, `bottom`, `left`
    * the offset does not affect other elements
  * `absolute`
    * the element is removed from the normal document flow
    * it is positioned relative to its closest positioned ancestor, if any,  otherwise, it is placed relative to the initial containing block
    * its final position is determined by the values of `top`, `right`, `bottom`, and `left`
  * `fixed`
    * the element is removed from the normal document flow, and no space is created for the element in the page layout
    * its final position is determined by the values of `top`, `right`, `bottom`, and `left`
    * it is positioned relative to the initial containing block established by the viewport
  * `sticky`
    * the element is positioned according to the normal flow of the document,
    * offset relative to its nearest scrolling ancestor and containing block based on the values of `top`, `right`, `bottom`, `left`
</details>
