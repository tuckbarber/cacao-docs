---
id: media
title: Media
---

<a class="sourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/media/media.css"></a>

The [media object](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/) 
is an abstract element used as the basis for building more complex and 
repetitive components (like blog comments, Tweets, etc).

Uses a fallback for browsers that do not support flexbox. Fallbacks are
applied when `<html>` has a class of `no-flexbox` or `no-flexwrap`.


## Available classes

* `Media`: Base component.
* `Media--withGutter`: Add a gutter between media items.
* `Media--withGutterSm`: Add a smaller gutter between media items.
* `Media-content`: Child content.
* `Media-subject`: The subject(s) of the content.
* `Media-subject--middle`: Vertically align subject to middle of content.
* `Media-subject--bottom`: Vertically align subject to bottom of content.


## Configurable variables

* `--Media-cell-gutter`: Gutter width.


## Usage

### Gutters

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<b>No modifier</b>
<div class="Media">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>

<b>--withGutter</b>
<div class="Media Media--withGutter">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>

<b>--withGutterSm</b>
<div class="Media Media--withGutterSm">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<b>No modifier</b>
<div class="Media">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--withGutter</b>
<div class="Media Media--withGutter">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--withGutterSm</b>
<div class="Media Media--withGutterSm">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>

</div>

### Subject aligning
The `Media-subject` element can be aligned relative to the rest of the content with
the `Media-subject--middle` and `Media-subject--bottom` modifiers.

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<b>No modifier</b>
<div class="Media Media--withGutterSm">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--bottom</b>
<div class="Media Media--withGutter">
  <div class="Media-subject Media-subject--bottom">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--middle</b>
<div class="Media Media--withGutter">
  <div class="Media-subject Media-subject--middle">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<b>No modifier</b>
<div class="Media Media--withGutterSm">
  <div class="Media-subject">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                  &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--bottom</b>
<div class="Media Media--withGutter">
  <div class="Media-subject Media-subject--bottom">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>
<br>
<b>--middle</b>
<div class="Media Media--withGutter">
  <div class="Media-subject Media-subject--middle">
      <!-- Photo by Hannah Busing on Unsplash -->
      <img src="https://images.unsplash.com/photo-1559662780-c3bab6f7e00b?ixlib=rb-1.2.1
                &ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=crop&w=80&q=80">
  </div>
  <div class="Media-content">
    Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque 
    laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi 
    architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas 
    sit aspernatur aut odit aut fugit, sed quia consequuntur magni dolores eos qui ratione 
    voluptatem sequi nesciunt. 
  </div>
</div>


</div>

