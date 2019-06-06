---
id: arrange
title: Arrange
---

<style>
.example-Child {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    padding: 5px 10px;
    text-align: center;
}
</style>

This component lets you lay out a row of cells in various ways. You can
specify whether a cell should be wide enough to fit its content, or take up
the remaining space in the row. It's also possible to give all cells an
equal width, and to control their vertical alignment.
 
## Available classes
 
 * `Arrange`: The core arrange component.
 * `Arrange--bottom`: Vertically align `sizeFit`/`sizeFill` children to the bottom.
 * `Arrange--equal`: Force child cells to be of equal width.
 * `Arrange--middle`: Vertically align `sizeFit`/`sizeFill` children to the middle.
 * `Arrange--withGutter`: Add a gutter between cells.
 * `Arrange-row`: Start a new row context.
 * `Arrange-sizeFill`: Fills remaining space not filled by `sizeFit` elements.
 * `Arrange-sizeFit`: Elements of default size.

## Configurable variables

* `--Arrange-gutter-size`: The width of the gutter applied by the `Arrange--withGutter` modifier class.

## Usage

For a comparison of `sizeFit` vs `sizeFill` elements:

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="Arrange Arrange--withGutter">
    <div class="Arrange-sizeFit"> 
        <div class="example-Child"> sizeFit<br>element </div>
    </div>
    <div class="Arrange-sizeFill"> 
        <div class="example-Child"> one<br>sizeFill </div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> another<br>sizeFit </div>
    </div>
</div>
```
<!--CSS-->
```css
.example-Child {
    background-color: #329A5C;
    border-radius: 5px;
    padding: 5px 10px;
    text-align: center;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="Arrange Arrange--withGutter">
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit<br>element </div> </div>
    <div class="Arrange-sizeFill"> <div class="example-Child"> one<br>sizeFill </div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
</div>
</div>

Using `Arrange--equal` to keep child elements of equal size despite their content.

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="Arrange Arrange--equal Arrange--withGutter">
    <div class="Arrange-sizeFit">
        <div class="example-Child"> sizeFit<br>element </div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> sizeFit with more content but is the same size</div>
    </div>
    <div class="Arrange-sizeFit">
        <div class="example-Child"> another<br>sizeFit </div>
    </div>
</div>
```
<!--CSS-->
```css
.example-Child {
    background-color: #329A5C;
    border-radius: 5px;
    padding: 5px 10px;
    text-align: center;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->


<div class="Arrange Arrange--equal Arrange--withGutter">
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit<br>element </div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit with more content but is the same size</div> </div>
    <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
</div>

</div>

Using `Arrange-row`, one with `Arrange--middle` the other with `Arrange--bottom`:

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="Arrange Arrange--withGutter">
    <div class="Arrange-row Arrange--middle">
        <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit <br>element </div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> Using <br>Arrange--middle <br> modifier</div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
    </div>
    <br>
    <div class="Arrange-row Arrange--bottom">
        <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit <br>element </div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> Using <br>Arrange--bottom <br> modifier</div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
    </div>
</div>
```
<!--CSS-->
```css
.example-Child {
    background-color: #329A5C;
    border-radius: 5px;
    padding: 5px 10px;
    text-align: center;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->


<div class="Arrange Arrange--withGutter">
    <div class="Arrange-row Arrange--middle">
        <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit <br>element </div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> Using <br>Arrange--middle <br> modifier</div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
    </div>
    <br>
    <div class="Arrange-row Arrange--bottom">
        <div class="Arrange-sizeFit"> <div class="example-Child"> sizeFit <br>element </div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> Using <br>Arrange--bottom <br> modifier</div> </div>
        <div class="Arrange-sizeFit"> <div class="example-Child"> another<br>sizeFit </div> </div>
    </div>
</div>

</div>

