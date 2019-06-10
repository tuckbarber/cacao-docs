---
   id: align
   title: Align
---

<style>
.example-parent {
    border: 2px #bbb solid;
    height: 100px;
    text-align:center;
}
.example-element {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    display: inline-block;
    height: 40px;
    //padding: 5px 20px;
    width: 15%;
}
</style>

To adjust vertical alignment. The affected element must also have an
appropriate `display` value.

## Available classes
* `u-alignBaseline`: Align element toward the baseline.
* `u-alignBottom`: Align element toward the bottom
* `u-alignMiddle`: Align element toward the middle.
* `u-alignTop`: Align element toward the top.

<div class="example-parent">
    <div class="example-element"></div>
    <div class="example-element u-alignBaseline"></div>
    <div class="example-element u-alignBottom"></div>
    <div class="example-element u-alignMiddle"></div>
    <div class="example-element u-alignTop"></div>
</div>