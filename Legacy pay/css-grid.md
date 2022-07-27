<a href="https://cssgridgarden.com/">Practice</a>

# display:grid;
- `grid-template: rows / columns`.
  - repeat( numberOfTime, measure )
    - `repeat( auto-fill, minmax( min, max ) )` insert as many rows/columns of the desired size as possible. If it can't fit all the elements, it'll move them down to a new line. Takes the minimum.
    - `repeat(auto-fit, minmax(min, max))` tries to fit all the elements, stretch, takes the maximum.
  - minmax( minVal, maxVal )
- `grid-template-area:` We can define groups for the cells. Each string represents a row
  - `grid-area: group-name`, this is a item property, later is presented other way to use this approach.
```css
  .container {
    ...code
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    grid-gap: 10px;
    grid-template-areas:
      "header header header"
      "advert content content"
      "advert footer footer";
  }
```
  - add columns to the grid: `grid-template-columns: ...columns(px)`
  - add rows to the grid: `grid-template-rows: ...rows(px)`
    - fr: sets the column or row to a fraction of the available space,
    - auto: sets the column or row to the width or height of its content automatically,
    - %: adjusts the column or row to the percent width of its container.
      - We can combine the them
    - we can use multiple cells with `repeat( ncells, 100/ncells % )`
      - you can use it whatever you want `repeat(ncells, %)`
- To add a gap use `grid-gap: rows(px) columns(px)`
  - To add a gap between the columns use `grid-column-gap: (px)`
  - To add a gap between the rows use `grid-row-gap: (px)`
- justify-items: ( start, center, end ) align all items at once.

#### Grid element properties
We can overlap items.
- With `order` we control the items overlaping.
- `grid-area: rowstart / columnstart / rowend / columnend `
  - grid-column: Define the dimesions in the columns of the element, ex. 1/4 from line 1 to 4. We can use `span (cells)` as well.
  - grid-row: Define the dimesions in the rows the element will span. ex. 2/4 from line 2 to 4.
- justify-self: Align the item within its cell ( start, center, end, stretch ) in the horizontal axis.
- align-self: Align the element vertically within its cells. ( start, center, end, stretch )

<img src="https://imgs.search.brave.com/WqqkBabCEqv1XBGb9ill9YsfFB4e7h6nvSrLTUo-O-0/rs:fit:672:522:1/g:ce/aHR0cHM6Ly93d3cu/YWRpY3Rvc2FsdHJh/YmFqby5jb20vd3At/Y29udGVudC91cGxv/YWRzLzIwMTgvMDEv/Y3NzLWdyaWQtbGlu/ZXMtMi5wbmc" alt="grid lines">
