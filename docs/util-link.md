---
   id: link
   title: Link
---

To be used with links to provide more functionality and alterations.

## Available classes

* `u-linkClean`: Reset all links styles and decorations.
* `u-linkObvious`: Ensure the link has an underline in order to standout as an obvious link.
* `u-linkNatural`: Link will inherit the text color of it's parent but will have an underline
to standout as an obvious link.
* `u-linkSubtle`: Similar to a natural link but the underline is only shown on hover.
* `u-linkComplex`: Link that mostly shows no decoration on text except inside child that has 
`u-linkComplexTarget` class.
* `u-linkComplexTarget`: Section of `u-linkComplexTarget` that shows underline on interaction.

## Usage

<div class="code-sample code-sample--padded">
<br>
This is <a href="#">a link without utilities.</a><br>
This is <a class="u-linkClean" href="#">a link using `u-linkClean`</a><br>
This is <a class="u-linkObvious" href="#">a link using `u-linkObvious`</a><br>
This is <a class="u-linkNatural" href="#">a link using `u-linkNatural`</a><br>
This is <a class="u-linkSubtle" href="#">a link using `u-linkSubtle`</a><br>
This is <a class="u-linkComplex" href="#">a link using <span class="u-linkComplexTarget">`u-linkComplex`</span></a>
</div>