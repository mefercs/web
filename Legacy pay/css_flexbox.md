<a href="https://flexboxfroggy.com/">Practice</a>

## display : flex
Turns an element into a flex container, this make it possible to align any children of that element into rows or columns.
- You can add the `flex-direction` in the parent. Creating a rows(horizontally) creating a column(vertically).
- Other values are `row-reverse` and a `column reverse`, by default `flex-direction` is set with `row`.
- The reverses also place the items in the oposite place.
- the `flex-direction` also inverts the justify and align items/content properties.
* TO  THE CONTAINER
- display: | flexbox | inline-flex;
- flex-direction: row | row-reverse | column | column-reverse;
- flex-wrap: nowrap | wrap | wrap-reverse;
- flex-flow: <‘flex-direction’> || <‘flex-wrap’>
- justify-content: flex-start | flex-end | center | space-between | space-around;
- align-items: flex-start | flex-end | center | baseline | stretch;
- align-content: flex-start | flex-end | center | space-between | space-around | stretch;
  - justify-content: **Aligns** in the `main`axis
  - align-items: **Aligns** in the `cross` axis (It's expected to set `height:auto` for `align-content: stretch`), It's for the entire elements treat them like a sigle line.
  - `flex-wrap` by default is set in `nowrap` with tries to fit everything in a row, `wrap` allows the elements take another line is space is not enough and `wrap-reverse` make the same but in the second row it'll place the element from top-bottom
  - `flex-flow` is the short-hand to put the direction and wrap property in that order.i.e.`flex-flow: column wrap`
  - `align-content` aligns items with multiple lines that could be produced by `flex-wrap:wrap`, it aligns for multiple lines.
* TO THE ITEMS WITHIN THE CONTAINER 
- order: <integer>;
- flex: none | [ <'flex-grow'> <'flex-shrink'>? || <'flex-basis'> ] 
  - flex-grow: <number>; /* default 0 */ the flex-shrink opposite. This acts when the container expands.
  - flex-shrink: <number>; /* default 1 */ the bigger number smaller the shrink. This acts when the parent shrinks.
  - flex-basis: <length> | auto; /* default auto */ we can add flex-grow and flex-shrink values next to flex-basis value in a single line. It is the delimiter for shrink and grow.
- align-self: auto | flex-start | flex-end | center | baseline | stretch; 
  - The  align-self is for a single element within the parent.
  - `order` is sometimes more useful to put elements in a specific order.
  - flex-shrink will shrink the element if the parent width is too small. 

<img src="https://www.freecodecamp.org/news/content/images/2019/10/image-32.png" alt="Flex attributes">

## display : block

Takes up the full width of the line it is on.
