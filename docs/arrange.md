---
id: arrange
title: Arrange Component
---

This component lets you lay out a row of cells in various ways. You can
specify whether a cell should be wide enough to fit its content, or take up
the remaining space in the row. It's also possible to give all cells an
equal width, and to control their vertical alignment.


## Features

* Protect against the component expanding beyond the confines of its
container if properties affecting the box-model are applied to the
component. Mainly necessary because of the last bullet.
* Rely on table layout.
* Zero out the default spacing that might be on an element (e.g., `ul`).
* Make sure the component fills at least the full width of its parent.
* Reset the table-layout algorithm in case a component is nested.
 
## Available classes
 
 * `Arrange`: The core arrange component.
 * `Arrange--equal`: Force child cells to be of equal width.
 * `Arrange--middle`: Vertically align `sizeFit`/`sizeFill` children.
 * `Arrange--withGutter`: Add a gutter between cells.
 * `Arrange-row`: Start a new row context.
 * `Arrange-sizeFll`: Fills remaining space not filled by `sizeFit` elements.
 * `Arrange-sizeFit`: Elements of default size.

## Configurable variables

* `--Arrange-gutter-size`: The width of the gutter applied by the `Arrange--withGutter` modifier class.