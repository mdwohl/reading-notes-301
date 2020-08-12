### Class 04 Reading

## CSS Grids

Grid column starting spans one column, but it's important to realize that each *line* is counted as the column start. It can work toward the right or left -- that is, the end value can be less than the start.

Grid can also travel backwards with a *negative value*. Grids don't need to be given a fixed start and end position based on grid lines; instead, they can use *span* (but only with positive values). Span can be used to set the item width relative to an end as well as a start.

A convenient shorthand is grid-column: x/y in which the x is the start and y is the end. It saves a lot of typing!

Grids are powerful in that they allow you to position elements in both columns and rows -- vertical and horizontal dimensions.

The combination of grid-column x/y and grid-row x/y shorthand can be used to span a large area quickly. Grid-area makes this even more simple, using four values:

Grid-area: a / b / c / d

Grid-area can be used for multiple grid overlays.

Grid templates can use % to divide space evenly or specifically across a page. Even more, it can use length units such as px and ems. They can be used in combination with one another.

Grids can also divide by fr -- fractional units.