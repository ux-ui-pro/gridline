<br>
<p align="center"><strong>gridline</strong></p>

<div align="center">

[![npm](https://img.shields.io/npm/v/gridline.svg?colorB=brightgreen)](https://www.npmjs.com/package/gridline)
[![GitHub package version](https://img.shields.io/github/package-json/v/ux-ui-pro/gridline.svg)](https://github.com/ux-ui-pro/gridline)
[![NPM Downloads](https://img.shields.io/npm/dm/gridline.svg?style=flat)](https://www.npmjs.org/package/gridline)

</div>

<p align="center"><sup>450B gzipped</sup></p>
<p align="center"><a href="https://t8th3h.csb.app/">Demo</a></p>
<br>

&#10148; **Install**

```console
yarn add gridline
```
<br>

&#10148; **Import**

<sub>CSS</sub>
```scss
@import "gridline/dist";
```

<sub>SCSS</sub>
```scss
@import "gridline/src";
```
<br>

&#10148; **Usage**
 
```html
<div class="gridline">
  <div>
    ...
  </div>
  ...
</div>
```
<br>

&#10148; **Settings**

<sub>Container</sub>

| HTML class             | Requires a child | Description                                                                                                 |
|:-----------------------|:----------------:|:------------------------------------------------------------------------------------------------------------|
| `.gridline`            |        —         | Will create a container that will occupy the full width of the layout.                                      |
| `.gridline--center`    |        —         | Creates a container aligned to the center of the layout.                                                    |
| `.gridline--left`      |        —         | Creates a container, the left edge of which will be stretched to the left edge of the layout.               |
| `.gridline--right`     |        —         | Creates a container, the right edge of which will be stretched to the right edge of the layout.             |
| `.gridline--scrolling` |     required     | Will create a container that, when overflowing with content horizontally, will receive a horizontal scroll. |
| `.gridline--collapse`  |        —         | Lines up the grid in a single column.                                                                       |

<sub>CSS styling</sub>

| Variable     |   Target    | Default |        Unit        | Description                                          |
|:-------------|:-----------:|:-------:|:------------------:|:-----------------------------------------------------|
| `--width`    | `.gridline` |  100%   |        `px`        | Width of the layout.                                 |
| `--padding`  | `.gridline` | `20px`  |     `px`, `vw`     | Sets indents between columns.                        |
| `--gap`      | `.gridline` | `20px`  |     `px`, `vw`     | Sets indents between columns. `0px` to turn off gap. |
| `--column`   |    child    |   `1`   | integer or decimal | Sets column width.                                   |
| `--offset`   |    child    |   `0`   | integer or decimal | Sets the column offset to the right.                 |
<br>

&#10148; **Continue to the edge**

<p>To extend the left or right column to the edge of the window, you need to add the `.edge` class to the column, or a class that has `edge` in its name.</p>

<br>

&#10148; **Scrolling**

<p>In order for a horizontal scroll to appear when the container overflows, it is necessary to add a styling class to the parent container `.gridline--scrolling`, and add a `.scrolling` class or a class containing `scrolling` in the name to the child block.</p>

<br>

&#10148; **License**

<p>gridline is released under MIT license</p>
