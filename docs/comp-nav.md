---
id: navigation
title: Navigation
---

<a class="sourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation"></a>

## Dropdown
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/dropdown.css"></a>

Base structure for dropdown menus. Can easily be extended and / or themed.


### Available classes

* `Dropdown`: Applied to the menu's parent to provide context for the dropdown 
  menu.
* `Dropdown-menu`: The actual dropdown.
* `Dropdown-item`: Items within the dropdown menu.
* `Dropdown-link`: Links within the dropdown menu.

#### States

* `is-last`: When applied to `Dropdown` this causes menus to align and fly-out 
  to the right.


### Configurable variables

* `--Dropdown-background`: Default dropdown menu background shorthand.
* `--Dropdown-fontSize`: Font size of base dropdown menu.
* `--Dropdown-lineHeight`: Line height of base dropdown menu.
* `--Dropdown-item-padding`: Padding of items within the dropdown menu.
* `--Dropdown-link-color`: Foreground color of links within the dropdown.
* `--Dropdown-link-colorHover`: Foreground color of hovered links within the dropdown.


### Usage

Basic use:

```html
<span class="Dropdown">
  Dropdown
  <ul class="Dropdown-menu">
    <li class="Dropdown-item">
      <a class="Dropdown-link" href="#is-last">Item 1</a>
    </li>
    <li class="Dropdown-item">
      <a class="Dropdown-link" href="#is-last">Item 2</a>
    </li>
  </ul>  
</span>
```

<style>
.example-holder{
    border: 2px #bbb solid;
    margin: 0 auto 100px auto;
    width: 500px;
}
.example-holder > .Dropdown{
    width: 150px;
    display: inline-block;
}
</style>

#### is-last

The `is-last` state can be applied to the last `Dropdown` element to prevent the dropdown menu from extending
too far to the right.

<div class="code-sample">

<br>
Without is-last on last dropdown
<div class="example-holder">
    <span class="Dropdown">
      Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Item 1</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Item 2</a>
        </li>
      </ul>  
    </span>
    <span class="Dropdown">
      Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
      </ul>  
    </span>
    <span class="Dropdown">
      Last Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
      </ul>  
    </span>
</div>

Using is-last on last dropdown
<div class="example-holder">
    <span class="Dropdown">
      Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Item 1</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Item 2</a>
        </li>
      </ul>  
    </span>
    <span class="Dropdown">
      Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
      </ul>  
    </span>
    <span class="Dropdown is-last">
      Last Dropdown
      <ul class="Dropdown-menu">
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
        <li class="Dropdown-item">
          <a class="Dropdown-link" href="#is-last">Some long navigation link</a>
        </li>
      </ul>  
    </span>
</div>


</div>


## FooterNav
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/footer.css"></a>

A navigation menu for the footer of the page.

### Available classes

* `FooterNav`: The parent element of the footer navigation menu.
* `FooterNav-item`: Menu items containing content such as links.
* `FooterNav-link`: Menu item links.

#### States

* `is-current` / `is-currentParent`: When applied to menu item the item will be styled to stand out 
  from the other items.

## MainNav
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/mainnav.css"></a>

Base structure for main navigation menus. Can easily be extended and / or 
themed.


### Available classes

* `MainNav`: Applied to the menu container.
* `MainNav-item`: Menu items containing content such as links.
* `MainNav-link`: Menu item links.

#### States

* `is-current` / `is-currentParent`: When applied to menu item the item will be styled to stand out 
  from the other items.


### Configurable variables

* `--MainNav-fontFamily`: Base menu font family.
* `-MainNav-fontSize`: Base menu font size.
* `-MainNav-lineHeight`: Base menu line height.
* `-MainNav-link-background`: Background shorthand for menu links.
* `-MainNav-link-backgroundHover`: Background shorthand for hovered menu links.
* `-MainNav-link-color`: Foreground color of menu links.
* `-MainNav-link-colorHover`: Foreground color of hovered menu links.


### Usage

Basic use:
```html
<ul class="MainNav">
  <li class="MainNav-item">
    <a class="MainNav-link" href="#">Menu item 1</a>
  </li>
  <li class="MainNav-item is-currentParent">
    <a class="MainNav-link" href="#">Menu item 2</a>
    <ul class="MainNav">
      <li class="MainNav-item">
        <a class="MainNav-link" href="#">Sub menu item 1</a>
      </li>
      <li class="MainNav-item is-current">
        <a class="MainNav-link" href="#">Sub menu item 2</a>
      </li>
    </ul>
  </li>
  <li class="MainNav-item">
    <a class="MainNav-link" href="#">Menu item 3</a>
  </li>
  <li class="MainNav-item">
    <a class="MainNav-link" href="#">Menu item 4</a>
  </li>
</ul>
```

## NavBar
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/bar.css"></a>

The bar to hold main navigation, contains `MainNav`.

### Available Classes

* `NavBar`: Applied to the parent element of `MainNav`.

## SidebarNav
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/sidebar.css"></a>

### Available classes

* `SidebarNav`: The parent element of the sidebar navigation menu.
* `SidebarNav-item`: Menu items containing content such as links.
* `SidebarNav-link`: Menu item links.

#### States

* `is-current` / `is-currentParent`: When applied to menu item the item will be styled to stand out 
  from the other items.
  

## SmScBtn
<a class="sourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/navigation/small-screen-button.css"></a>

A button to expand/compact navigation menu for smaller displays.

### Available classes

* `SmScBtn`: The clickable item element.
* `SmScBtn-icon`: Icon within the button, displays whether the menu is expanded or compacted.

#### States

* `is-active`: When the button has been pressed and the menu is expanded.

### Usage

```html
<button class="SmScBtn">
    <span class="SmScBtn-icon"></span>Menu
</button>
```

**Note**: this component will only be visible when the viewport is appropritately small. The expansion of the menu and the
addition of the `is-active` class requires additional JavaScript code.

<div class="code-sample">
<button class="SmScBtn" style="display:inherit; background-color: #3264a8;" 
        onClick="this.classList.contains('is-active') ? this.classList.remove('is-active') : this.classList.add('is-active')">
    <span class="SmScBtn-icon"></span>Menu
</button>
</div>


## Complete Example
<div class="code-sample">
<style>
#nav-display {
    background-color: #fff;
    border: 3px #aaa dashed;
    margin: 40px auto;
    height: 400px;
    overflow: hidden;
    transition: width 0.5s;
    width: 80%;
}
#nav-display.mobile-view {
    width: 30%;
    transition: width 0.5s;
}
#nav-display iframe {
    height: 800px;
    max-width: 200%;
    width: 200%;
    -ms-zoom: 0.5;
    -moz-transform: scale(0.5);
    -moz-transform-origin: 0 0;
    -o-transform: scale(0.5);
    -o-transform-origin: 0 0;
    -webkit-transform: scale(0.5);
    -webkit-transform-origin: 0 0;
}
</style>

<script type="text/javascript">function switchDisplay(){fdisp=document.getElementById("nav-display"),fdisp.classList.contains("mobile-view")?fdisp.classList.remove("mobile-view"):fdisp.classList.add("mobile-view")}</script>

<button class="Button" onclick="switchDisplay()"> Switch Display Type </button>

<div id="nav-display">
    <iframe src="assets/example-nav.html"></iframe>
</div>

</div>