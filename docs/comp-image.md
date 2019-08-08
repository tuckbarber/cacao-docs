---
id: image-component
title: Image
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/image/"></a>

Generic component that applies common treatments to `<img>` elements.

## Image
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/image/image.css"></a>

### Available classes

* `Image`: Base component.
* `Image--left`: Float image left.
* `Image--right`: Float image right.


### Configurable variables

* `--Image-spacing`: Spacing applied to bottom of images.


### Usage

Images can be floated to either side and text will wrap around. `Image--left` and `Image--right` 
will limit the width of the image to 40% of the parent element to provide space for the text.
<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<p>
  <!-- Photo by Hannah Busing on Unsplash -->
  <img class="Image Image--right" 
       src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
       &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80">
  Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
  laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
  architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
  sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
  voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
  amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
  labore et dolore magnam aliquam quaerat voluptatem. 
</p>
```

<!--END_DOCUSAURUS_CODE_TABS-->

<p>
  <!-- Photo by Hannah Busing on Unsplash -->
  <img class="Image Image--right" 
       src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
       &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80">
  Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
  laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
  architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
  sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
  voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
  amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
  labore et dolore magnam aliquam quaerat voluptatem. 
</p>

</div>

## Image Wrapper
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/image/wrapper.css"></a>

Provides styles to display an image on a page centered, floated left or floated 
right along with other content like a caption.

### Available Classes

* `ImageWrapper`: Base component.
* `ImageWrapper--left`: Float image left.
* `ImageWrapper--center`: Align the image center.
* `ImageWrapper--right`: Float image right.

### Usage

```html
<div class="ImageWrapper ImageWrapper--right">
    <img src="/path/to/image.jpg" alt="Image" width="200" height="120">
</div>
```

## Image Caption
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/image/caption.css"></a>

Provides styles for an image caption to be displayed below the image.

The ImageCaption class works best when paired with the ImageWrapper classes.

### Available classes

* `ImageCaption`: Base component.

### Usage

<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="Example-parent">
  <div class="ImageWrapper ImageWrapper--left">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--left caption</div>
   </div>
    <div class="ImageWrapper ImageWrapper--right">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--right caption</div>
    </div>
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
    amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
    labore et dolore magnam aliquam quaerat voluptatem. 
  <div class="ImageWrapper ImageWrapper--center">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--center caption</div>
  </div>
    Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
    amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
    labore et dolore magnam aliquam quaerat voluptatem. 
</div>
```

<!--END_DOCUSAURUS_CODE_TABS-->
<div class="Example-parent">
  <div class="ImageWrapper ImageWrapper--left">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--left caption</div>
   </div>
    <div class="ImageWrapper ImageWrapper--right">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--right caption</div>
    </div>
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
    amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
    labore et dolore magnam aliquam quaerat voluptatem. 
  <div class="ImageWrapper ImageWrapper--center">
        <!-- Photo by Hannah Busing on Unsplash -->
        <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=150&q=80" 
             alt="Image" width="150" height="150">
        <div class="ImageCaption">--center caption</div>
  </div>
    Neque porro quisquam est, qui dolorem ipsum quia dolor sit 
    amet, consectetur, adipisci velit, sed quia non numquam eius modi tempora incidunt ut 
    labore et dolore magnam aliquam quaerat voluptatem. 
</div>
</div>
