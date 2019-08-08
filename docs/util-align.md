---
   id: align
   title: Align
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/align/align.css"></a>

<style>
.Example-parent {
    border: 2px #bbb solid;
    height: 100px;
    text-align: center;
    position: relative;
    font-size: 2em;
    line-height: 1.5em;
}
.Example-element {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    display: inline;
    font-size: 0.5em;
    min-width: 15%;
    padding: 0.5em;
}
.example-other{
    background-color:#5378A2;
    border-radius: 5px;
    color: #FFF; 
    display: inline-block;
    height: 60px;
    margin: 0.5em;
    padding: 0.2em;
}
.line{
    border-top: 1px #444 dashed;
    width: 100%;
    position: absolute;
    display: block;
    top: 1.8em;
}


</style>

To adjust vertical alignment. The affected element must also have an
appropriate `display` value.

## Available classes
* `u-alignBaseline`: Align element toward the baseline.
* `u-alignBottom`: Align element toward the bottom
* `u-alignMiddle`: Align element toward the middle.
* `u-alignTop`: Align element toward the top.

## Usage

<div class="CodeSample CodeSample--padded">
    <div class="Example-parent">
        <div class="line"></div>
        <div class="example-other">Parent-sized font</div>
        <div class="Example-element u-alignBaseline">baseline</div>
        <div class="Example-element u-alignBottom">bottom</div>
        <div class="Example-element u-alignMiddle">middle</div>
        <div class="Example-element u-alignTop">top</div>
    </div>
</div>