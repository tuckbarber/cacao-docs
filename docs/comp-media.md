---
id: media
title: Media
---


The [media object](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/) 
is an abstract element used as the basis for building more complex and 
repetitive components (like blog comments, Tweets, etc).

Uses a fallback for browsers that do not support flexbox. Fallbacks are
applied when `<html>` has a class of `no-flexbox` or `no-flexwrap`.

Basic visual tests are in [`test/modules/media.html`](http://aptuitiv.github.io/cacao/test/modules/media.html)
and fallback layout tests are found in [`test/modules/media-noflex.html`](http://aptuitiv.github.io/cacao/test/modules/media-noflex.html).


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

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
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
```
<!--END_DOCUSAURUS_CODE_TABS-->

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


