<div align="center">
<br>
<h1>gridline</h1>

[![npm](https://img.shields.io/npm/v/gridline.svg?colorB=brightgreen)](https://www.npmjs.com/package/gridline)
[![GitHub package version](https://img.shields.io/github/package-json/v/ux-ui-pro/gridline.svg)](https://github.com/ux-ui-pro/gridline)
[![NPM Downloads](https://img.shields.io/npm/dm/gridline.svg?style=flat)](https://www.npmjs.org/package/gridline)

<p><sup>650B gzipped</sup></p>

<h3><a href="https://t8th3h.csb.app/">Demo</a></h3>
</div>
<br>


### Install  
```bash
$ yarn add gridline
```
<br>

### Import

<sub>**CSS**</sub>
```css
@import "gridline/dist";
```
<sub>**SCSS**</sub>
```css
@import "gridline/src";
```
<br>

### Usage  
```html
<div class="gridline">
  <div>
    ...
  </div>
  ...
</div>
```
<br>

### Settings  
<sub>**Container**</sub>

| HTML class              | Requires a child | Description                                                                                                  |
| :---------------------- | :--------------: | :----------------------------------------------------------------------------------------------------------- |
| `.gridline`             |        —         | Will create a container that will occupy the full width of the layout.                                       |
| `.gridline--center`     |        —         | Creates a container aligned to the center of the layout.                                                     |
| `.gridline--left`       |        —         | Creates a container, the left edge of which will be stretched to the left edge of the layout.                |
| `.gridline--right`      |        —         | Creates a container, the right edge of which will be stretched to the right edge of the layout.              |
| `.gridline--scrolling`  |     required     | Will create a container that, when overflowing with content horizontally, will receive a horizontal scroll.  |

<br><sub>**CSS styling**</sub>

| Variable     | Target        | Default    | Unit                 | Description                                           |
| :----------- | :-----------: | :--------: | :------------------: | :---------------------------------------------------- |
| `--width`    |  `.gridline`  |    100%    |         `px`         | Width of the layout.                                  |
| `--padding`  |  `.gridline`  |   `20px`   |      `px`, `vw`      | Sets indents between columns.                         |
| `--gap`      |  `.gridline`  |   `20px`   |      `px`, `vw`      | Sets indents between columns. `0px` to turn off gap.  |
| `--column`   |     child     |    `1`     |  integer or decimal  | Sets column width.                                    |
| `--offset`   |     child     |    `0`     |  integer or decimal  | Sets the column offset to the right.                  |

<br>

### Continue to the edge  
To extend the left or right column to the edge of the window, you need to add the `.edge` class to the column, or a class that has `edge` in its name.

<br>

### Scrolling  
In order for a horizontal scroll to appear when the container overflows, it is necessary to add a styling class to the parent container `.gridline--scrolling`, and add a `.scrolling` class or a class containing `scrolling` in the name to the child block.

<br>

### License  
gridline is released under MIT license