<a href="https://cssgridgarden.com/">Practice</a>

# display:grid;
- add columns to the grid: `grid-template-columns: ...columns(px)`
- add rows to the grid: `grid-template-rows: ...rows(px)`
  - fr: sets the column or row to a fraction of the available space,
  - auto: sets the column or row to the width or height of its content automatically,
  - %: adjusts the column or row to the percent width of its container.
    - We can combine the them
- To add a gap use `grid-gap: rows(px) columns(px)`
  - To add a gap between the columns use `grid-column-gap: (px)`
  - To add a gap between the rows use `grid-row-gap: (px)`
- grid-column: Define the dimesions in the columns of the element, ex. 1/4 from line 1 to 4.
- grid-row: Define the dimesions in the rows the element will span. ex. 2/4 from line 2 to 4.

<img src="https://imgs.search.brave.com/WqqkBabCEqv1XBGb9ill9YsfFB4e7h6nvSrLTUo-O-0/rs:fit:672:522:1/g:ce/aHR0cHM6Ly93d3cu/YWRpY3Rvc2FsdHJh/YmFqby5jb20vd3At/Y29udGVudC91cGxv/YWRzLzIwMTgvMDEv/Y3NzLWdyaWQtbGlu/ZXMtMi5wbmc" alt="grid lines">
