## Read 12

**Chart**

- Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

- The great things about Chart.js are that it’s simple to use and really very flexible.

**Canvas**

- At first sight a <canvas> looks like the <img> element, with the only clear difference being that it doesn't have the src and alt attributes

- Providing fallback content is very straightforward: just insert the alternate content inside the <canvas> element. Browsers that don't support <canvas> will ignore the container and render the fallback content inside it.

- Before we can start drawing, we need to talk about the canvas grid or coordinate space.

- fillRect(x, y, width, height) Draws a filled rectangle.

- strokeRect(x, y, width, height) Draws a rectangular outline.

- clearRect(x, y, width, height) Clears the specified rectangular area, making it fully transparent.

- fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

- strokeText(text, x, y [, maxWidth]) Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

