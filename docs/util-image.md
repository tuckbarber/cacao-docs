---
   id: image
   title: Image
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/image/image.css"></a>

To be applied to images for general sizing and positioning.

## Available classes

* `u-img`: Make an image shrink to the width of its containing element if the element 
is smaller than the image's original width.
* `u-imgFull`: Make an image scale to the width of its containing element regardless of 
the image's original width.

## Usage

<style>
.CodeSample{
    padding: 0 10% 20px;
}
.Example-parent{
    display: block;
    border: 2px #bbb dashed;
}
</style>

<!-- Photo by Taylor Simpson on Unsplash -->
<div class="CodeSample">
    <br>
    u-img (container 300px, image 100px)
    <div class="Example-parent" style="width:300px">
        <img class="u-img" src="https://images.unsplash.com/photo-1560750588-73207b1ef5b8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=100&q=80">
    </div>
    <br>
    u-imgFull (container 300px, image 100px)
    <div class="Example-parent" style="width:300px">
        <img class="u-imgFull" src="https://images.unsplash.com/photo-1560750588-73207b1ef5b8?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=100&q=80">
    </div>
</div>