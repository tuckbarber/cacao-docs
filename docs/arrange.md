---
id: arrange
title: Arrange Component
---

<style>
.example-Child {
    background-color: #329A5C;
    padding: 5px 10px;
}
</style>

This component lets you lay out a row of cells in various ways. You can
specify whether a cell should be wide enough to fit its content, or take up
the remaining space in the row. It's also possible to give all cells an
equal width, and to control their vertical alignment.
 
## Available classes
 
 * `Arrange`: The core arrange component.
 * `Arrange--equal`: Force child cells to be of equal width.
 * `Arrange--middle`: Vertically align `sizeFit`/`sizeFill` children.
 * `Arrange--withGutter`: Add a gutter between cells.
 * `Arrange-row`: Start a new row context.
 * `Arrange-sizeFill`: Fills remaining space not filled by `sizeFit` elements.
 * `Arrange-sizeFit`: Elements of default size.

## Configurable variables

* `--Arrange-gutter-size`: The width of the gutter applied by the `Arrange--withGutter` modifier class.

## Examples

For a comparison of `sizeFit` vs `sizeFill` elements:

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="example-Parent Arrange Arrange--withGutter">
    <div class="Arrange-sizeFit"> 
        <div class="example-Child"> sizeFit<br>Element </div>
    </div>
    <div class="Arrange-sizeFill"> 
        <div class="example-Child"> One<br>sizeFill </div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> Another<br>sizeFit </div>
    </div>
</div>
```
<!--CSS-->
```css
.example-Child {
    background-color: #329A5C;
    padding: 5px 10px;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="example-Parent Arrange Arrange--withGutter">
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit<br>Element </div> </div>
    <div class="Arrange-sizeFill"> <div class="example-Child"> One<br>sizeFill </div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> Another<br>sizeFit </div> </div>
</div>
</div>

Using `Arrange--equal` to keep child elements of equal size despite their content.

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="example-Parent Arrange Arrange--equal Arrange--withGutter">
    <div class="Arrange-sizeFit">
        <div class="example-Child"> sizeFit<br>Element </div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> sizeFit with more content but is the same size</div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> Another<br>sizeFit </div>
    </div>
</div>
```
<!--CSS-->
```css
.example-Child {
    background-color: #329A5C;
    padding: 5px 10px;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->


<div class="example-Parent Arrange Arrange--equal Arrange--withGutter">
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit<br>Element </div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit with more content but is the same size</div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> Another<br>sizeFit </div> </div>
</div>

</div>

