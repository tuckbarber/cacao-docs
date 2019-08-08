---
id: button
title: Button
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/button/button.css"></a>

Provides a basic button template that includes a very basic default theme that
is ready to be extended.


## Available classes

* `Button`: The core button component.
* `Button--lg`: Adjusts padding so that button is larger.
* `Button--sm`: Adjusts padding so that button is smaller.

### States

* `is-disabled`: For disabled-state button styles 
  
  **Note**: You must also include the `disabled` attribute on `button` 
  elements. For `a` elements, you should prevent JavaScript event handlers 
  from firing.


## Configurable variables

* `--Button-background`: Background for the base button.
* `--Button-backgroundHover`: Hover background for the base button.
* `--Button-border`: Border shorthand applied to the base button.
* `--Button-border-radius`: Border radius applied to the base button.
* `--Button-color`: Foreground color for the base button.
* `--Button-disabled-opacity`: Opacity applied to disabled buttons.
* `--Button-fontFamily`: Font family for the base button.
* `--Button-fontSize`: Font size for the base button.
* `--Button-letterSpacing`: Letter spacing for the base button.
* `--Button-lineHeight`: Line height for the base button.
* `--Button-padding`: Padding shorthand.
* `--Button-paddingLg`: Larger padding shorthand.
* `--Button-paddingSm`: Smaller padding shorthand.


## Usage

Buttons can have multiple lines of text and will wrap text. Buttons are baseline-aligned.

<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<a class="Button">Sign up</a>
<button class="Button is-disabled" type="button" disabled>Close</button>
<br>
<br>
<a class="Button" style="width:150px;">Button with more text</a>
<a class="Button" style="width:150px;">Button</a>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<a class="Button">Sign up</a>
<button class="Button is-disabled" type="button" disabled>Close</button>
<br>
<br>
<a class="Button" style="width:150px;">Button with more text</a>
<a class="Button" style="width:150px;">Button</a>

</div>

### Theming / extending

The CSS is focused on common structural requirements for buttons. You can build
your application-specific theme styles in your app. For example:

<div class="CodeSample">

<!--DOCUSAURUS_CODE_TABS-->
<!--CSS-->
```css
/* import the module or write these styles directly in `button.css` */
@import "cacao/lib/button";

.Button--default {
  background-color: #0E3E62;
  color: #eee;
  border: 5px #32648a solid;
  border-radius: 2px;
}

.Button--default:hover,
.Button--default:focus,
.Button--default:active,
.Button--default.is-pressed {
  background-color: #32648a;
  border-color: #517d9f;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
}

.Button--default:focus {
  border-color: #069;
  outline: 0;
}

.Button--default:active,
.Button--default.is-pressed {
  background-color: #042a47;
  box-shadow: inset 0 1px 2px rgba(0,0,0, 0.2);
}
```
<!--HTML-->
```html
<a class="Button Button--default" href="{{url}}">Custom Button</a>
```
<!--END_DOCUSAURUS_CODE_TABS-->



<style>
.Button--default {
  background-color: #0E3E62;
  color: #eee;
  border: 5px #32648a solid;
  border-radius: 2px;
}
.Button--default:hover,
.Button--default:focus,
.Button--default:active,
.Button--default.is-pressed {
  background-color: #32648a;
  border-color: #517d9f;
  box-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
}
.Button--default:focus {
  border-color: #069;
  outline: 0;
}
.Button--default:active,
.Button--default.is-pressed {
  background-color: #042a47;
  box-shadow: inset 0 1px 2px rgba(0,0,0, 0.2);
}
</style>
<a class="Button Button--default" href="#theming-extending">Custom Button</a>