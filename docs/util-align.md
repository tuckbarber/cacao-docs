---
   id: align
   title: Align
---

<style>
.example-parent {
    border: 2px #bbb solid;
    height: 100px;
    text-align: center;
    position: relative;
    font-size: 1.5em;
    line-height: 1.5em;
}
.example-element {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    display: inline-block;
    min-width: 15%;
}
.example-other{
    background-color:#355E8C; 
    height: 60px;
    padding: 0.5em;
    margin: 0.5em;
}
.line{
    border-top: 1px #222 solid;
    width: 100%;
    position: absolute;
    display: block;
    top: 2em;
}


</style>

To adjust vertical alignment. The affected element must also have an
appropriate `display` value.

## Available classes
* `u-alignBaseline`: Align element toward the baseline.
* `u-alignBottom`: Align element toward the bottom
* `u-alignMiddle`: Align element toward the middle.
* `u-alignTop`: Align element toward the top.


<div class="code-sample">
    <div class="example-parent">
        <div class="line"></div>
        <div class="example-element example-other">Some inline text</div>
        <div class="example-element u-alignBaseline">baseline</div>
        <div class="example-element u-alignBottom">bottom</div>
        <div class="example-element u-alignMiddle">middle</div>
        <div class="example-element u-alignTop">top</div>
    </div>
</div>