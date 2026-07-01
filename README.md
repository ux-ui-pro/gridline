# gridline

Flexbox grid system for building responsive 12-column layouts with CSS custom properties.

[![npm](https://img.shields.io/npm/v/gridline.svg?colorB=brightgreen)](https://www.npmjs.com/package/gridline)
[![NPM Downloads](https://img.shields.io/npm/dm/gridline.svg?style=flat)](https://www.npmjs.com/package/gridline)

[Demo](https://codepen.io/ux-ui/pen/QWzqdbp)

---

## Features

- 12-column flexbox grid with gap and offset controls
- Container modifiers: center, left, right, scrolling, collapse
- Edge-to-viewport columns via `.edge` class pattern
- Tunable layout via CSS custom properties on `.gridline` and children

---

## Installation

```bash
npm install gridline
```

Import the packaged stylesheet in your app entry:

```js
import 'gridline';
```

Or use the deep path:

```scss
@use "gridline/dist/index.css" as *;
```

---

## Quick Start

```html
<div class="gridline">
  <div style="--gridline-column: 6">...</div>
  <div style="--gridline-column: 6">...</div>
</div>
```

---

## Settings

### Container classes

| Class | Requires a child | Description |
| --- | :---: | --- |
| `.gridline` | — | Full-width layout container. |
| `.gridline--center` | — | Container centered in the viewport. |
| `.gridline--left` | — | Container aligned to the left edge of the layout. |
| `.gridline--right` | — | Container aligned to the right edge of the layout. |
| `.gridline--scrolling` | required | Horizontal scroll when content overflows. |
| `.gridline--collapse` | — | Single-column collapsed grid. |

### CSS custom properties

| Variable | Target | Default | Unit | Description |
| --- | --- | :---: | --- | --- |
| `--gridline-width` | `.gridline` | `100%` | `px` | Width of the layout. |
| `--gridline-padding` | `.gridline` | `20px` | `px`, `vw` | Outer padding of the container. |
| `--gridline-gap` | `.gridline` | `20px` | `px`, `vw` | Gap between columns; `0px` disables gap. |
| `--gridline-column` | child | `1` | integer or decimal | Column span width. |
| `--gridline-offset` | child | `0` | integer or decimal | Column offset to the right. |

---

## Styling

### Continue to the edge

To extend a column to the left or right edge of the viewport, add the `.edge` class to the column, or any class name containing `edge`.

### Scrolling

For horizontal scroll on overflow, add `.gridline--scrolling` to the parent container and `.scrolling` (or a class containing `scrolling`) to the child block.

---

## License

MIT
