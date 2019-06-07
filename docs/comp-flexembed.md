---
id: flexembed
title: FlexEmbed
---

<style>
.example-Parent{
    width: 60%;
    margin: 10px auto;
 }
.example-Parent > div{
    margin: 20px 0;
    border: 2px #bbb solid;
}
</style>

CSS for responsive, intrinsic ratio embeds.


## Available classes

* `FlexEmbed`: The root node.
* `FlexEmbed-ratio`: The element that provides the aspect ratio (1:1 by default).
* `FlexEmbed-ratio--5by4`: The modifier class for 5:4 aspect ratio embed.
* `FlexEmbed-ratio--4by3`: The modifier class for 4:3 aspect ratio embed.
* `FlexEmbed-ratio--3by2`: The modifier class for 3:2 aspect ratio embed.
* `FlexEmbed-ratio--8by5`/`FlexEmbed-ratio--16by10`: The modifier class for 8:5 aspect ratio embed.
* `FlexEmbed-ratio--5by3`: The modifier class for 5:3 aspect ratio embed.
* `FlexEmbed-ratio--16by9`: The modifier class for 16:9 aspect ratio embed.
* `FlexEmbed-ratio--2by1`: The modifier class for 2:1 aspect ratio embed,
* `FlexEmbed-ratio--3by1`: The modifier class for 3:1 aspect ratio embed.
* `FlexEmbed-content`: The descendent class for the content that is being displayed.


## Usage

Example:

```html
<div class="FlexEmbed">
  <div class="FlexEmbed-ratio FlexEmbed-ratio--16by9"></div>
  <iframe class="FlexEmbed-content" src="..."></iframe>
</div>
```

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="example-Parent">
    No modifier
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                               &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
        frameborder="0" height="300" width="500"></iframe>
    </div>
    5by4
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--5by4"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    4by3
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--4by3"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>    
    3by2
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--3by2"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    8by5
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--8by5"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    5by3
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--5by3"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    16by9
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--16by9"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    2by1
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--2by1"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    3by1
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--3by1"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
</div>
```
<!--CSS-->
```css
.example-Parent{
    width: 60%;
    margin: 10px auto;
}
.example-Parent > div{
    margin: 20px 0;
    border: 2px #bbb solid;
}
```

<!--END_DOCUSAURUS_CODE_TABS-->
<div class="example-Parent">
    No modifier
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                               &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
        frameborder="0" height="300" width="500"></iframe>
    </div>
    5by4
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--5by4"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    4by3
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--4by3"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>    
    3by2
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--3by2"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    8by5
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--8by5"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    5by3
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--5by3"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    16by9
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--16by9"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    2by1
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--2by1"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
    3by1
    <div class="FlexEmbed">
        <div class="FlexEmbed-ratio FlexEmbed-ratio--3by1"></div>
        <iframe class="FlexEmbed-content" src="https://maps.google.com/maps?hl=en&q=Farmington,Maine
                                                       &ie=UTF8&t=roadmap&z=15&iwloc=B&output=embed"
                frameborder="0" height="300" width="500"></iframe>
    </div>
</div>
</div>

If the child content has a width and height of 100% you can also nest it within
`FlexEmbed-content`.

```html
<div class="FlexEmbed">
  <div class="FlexEmbed-ratio FlexEmbed-ratio--16by9"></div>
  <div class="FlexEmbed-content">
    <!-- child content -->
  </div>
</div>
```

You can add custom aspect ratios. For example, to create a 2.35:1 aspect
ratio:

```css
/**
 * Modifier: 47:20 aspect ratio
 */

.FlexEmbed-ratio--47by20 {
  padding-bottom: 42.55%;
}
```

Alternatively, aspect ratios can be calculated programmatically and the
corresponding `padding-bottom` value applied using an inline style.

```html
<div class="FlexEmbed">
  <div class="FlexEmbed-ratio" style="padding-bottom:{{percentage}}%"></div>
  <div class="FlexEmbed-content">
    <!-- child content -->
  </div>
</div>
```
