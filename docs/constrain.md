---
id: constrain
title: Constrain
---

<style>
.example-Parent{
    display: inline-block;   
    margin: 2%;
    width: 45%;
    border: 2px #ddd solid;
}
.example-Element{
    background-image: url(https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=400&q=80);
}
</style>

Constrains an image of unknown size to the specified aspect ratio.
The image is potentially cropped using the specified gravity.
Similar to `FlexEmbed` but meant to be used specifically with images.

This method will be used until the `object-fit` and `object-position`
properties are well supported. <http://caniuse.com/#feat=object-fit>

Basic visual tests are in [`test/modules/constrain.html`](http://aptuitiv.github.io/cacao/test/modules/constrain.html).


## Available classes

* `Constrain`: The base component.
* `Constrain--contain`: Contains the image within the ratio rather than filling
  the ratio and potentially cropping.
* `Constrain--5by4`: The modifier class for 5:4 aspect ratio image.
* `Constrain--4by3`: The modifier class for 4:3 aspect ratio image.
* `Constrain--3by2`: The modifier class for 3:2 aspect ratio image,
* `Constrain--8by5` / `Constrain--16by10`: The modifier class for 8:5/16:10 
  aspect ratio image.
* `Constrain--16by9`: The modifier class for 16:9 aspect ratio image.
* `Constrain--top`: Sets the image to gravitate towards the top edge.
* `Constrain--bottom`: Sets the image to gravitate towards the bottom edge.
* `Constrain--left`: Sets the image to gravitate towards the left edge.
* `Constrain--right`: Sets the image to gravitate towards the right edge.
* `Constrain--topLeft`: Sets the image to gravitate towards the top left 
  corner.
* `Constrain--topRight`: Sets the image to gravitate towards the top right 
  corner.
* `Constrain--bottomLeft`: Sets the image to gravitate towards the bottom 
  left corner.
* `Constrain--bottomRight`: Sets the image to gravitate towards the bottom 
  right corner.


## Usage

The image must be applied to the element via the `background-image` property,
either by applying a custom class or using inline styles.

```html
<div class="Constrain Constrain--16by9" style="background-image: url('...');"></div>
```

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--3by2"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--5by4"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--3by2 Constrain--contain Constrain--left"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--5by4 Constrain--contain Constrain--topRight"></div>
</div>
```
<!--CSS-->
```css
.example-Parent{
    display: inline-block;   
    margin: 2%;
    width: 45%;
    border: 2px #ddd solid;
}
.example-Element{
    /* Photo by Hannah Busing on Unsplash */
    background-image: url(https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=400&q=80);
}
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="example-Parent">
    <div class="example-Element Constrain Constrain--3by2"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--5by4"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--3by2 Constrain--contain Constrain--left"></div>
</div>
<div class="example-Parent">
    <div class="example-Element Constrain Constrain--5by4 Constrain--contain Constrain--topRight"></div>
</div>

</div>

You can add custom aspect ratios. For example, to create a 2.35:1 aspect
ratio:

```css
/**
 * Modifier: 47:20 aspect ratio
 */

.Constrain--47by20 {
  padding-bottom: 42.55%;
}
```

Alternatively, aspect ratios can be calculated programmatically and the
corresponding `padding-bottom` value applied using an inline style.

```html
<div class="Constrain Constrain--16by9" style="background-image: url('...'); padding-bottom: 42.55%;"></div>
```

