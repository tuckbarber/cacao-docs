---
id: container
title: Container
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/container/container.css"></a>

<style>
.Example-parent{
    border: 2px #bbb dashed;
    margin-bottom: 20px;
    width: 500px;
}
.Example-element {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    padding: 10px 20px;
}
.Container{
    max-width: 600px;
}
.Container--fixedWidth{
    width: 600px;
}
</style>

Page content container.


## Available classes

* `Container`: The base component.
* `Container--fixedWidth`: Fix the width of the component so that it is no 
  longer fluid.
* `Container--alignLeft`: Align component to the left.
* `Container--alignRight`: Align component to the right.


## Configurable variables

* `--Container-width`: Width of the component.


## Usage

```html
<div class="Container">
    <!-- child content -->
</div>
```


<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="Example-parent">
    <p class="Example-element Container">
        This is some text that is contained within the container.
    </p>
    <p class="Example-element Container Container--fixedWidth">
        A fixedWidth container will not shrink to fit viewport.
    </p>
</div>
<p class="Example-element Container Container--alignLeft">
    This container is aligned left.
</p>
<p class="Example-element Container Container--alignRight">
    And this one is aligned right.
</p>
```

<!--CSS-->
```css
/* --Container-width: 600px;
    set in container.css     */
  
.Example-parent{
    border: 2px #bbb dashed;
    margin-bottom: 20px;
    width: 500px;
}

.Example-element {
    background-color: #329A5C;
    border-radius: 5px;
    color: #FFF;
    padding: 10px 20px;
}
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="Example-parent">
    <p class="Example-element Container">
        This is some text that is contained within the container.
    </p>
    <p class="Example-element Container Container--fixedWidth">
        A fixedWidth container will not shrink to fit viewport.
    </p>
</div>
<p class="Example-element Container Container--alignLeft">
    This container is aligned left.
</p>
<p class="Example-element Container Container--alignRight">
    And this one is aligned right.
</p>

</div>


