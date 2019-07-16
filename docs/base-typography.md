---
   id: base-typography 
   title: Typography
---

Modifies typographic type selectors for compatibility, best practices, and workarounds.

Note: This sets the <html> element's font-size to 62.5%, which
equals 10px (for default browser font size of 16px).
This allows rem units to be calculated more intuitively.

Font size strategy
- <html> element font size set as a percentage so that font sizes are accessible
  if the user resizes the text size in their browser.
- Font size set on the <body> tag is a rem. A direct relation to the HTML element.
- Font sizes for components should be rem. For example, the font size of the navigation
  should be set as a rem. The relation is to the <html> tag, which by default is 10px.
- Font sizes of elements within a component should be em to be relative to the component.
  For example, a navigation link within the navigation menu would be set to an em font size,
  which would then be in relation to the navigation component (assuming that a font size in rem
  was set on the navigation item).

References that influenced this approach:
* https://css-tricks.com/rem-global-em-local/ 
* http://clagnut.com/blog/2384/


## Affected Type Selectors

* `html`: Set the base font size to be a percentage so that it's more accessible to browser text zooming, and also scales down text on smaller screen.
* `body`: Set body defaults based on configurable variables for other elements to inherit.
* `address, blockquote, dl, figure, hr, ol, p, ul`: Adjust margins.
* `blockquote`: Add left border and margins/padding.
* `a`: Set link appearance based on configurable variables.
* `a[href^=tel]`: Sets telephone links to default styling to not look like links.
* `ol, ul`: Adjusts margins/padding.
* `dt`: Sets font weight to heavy.
* `dd`: Removes margin.
* `abbr[title]`: Adds bottom border and help cursor to inline abbreviations.
* `address`: Resets browser default.
* `hr`: 
    * Remove default hr shading.
    * Inherit text or parent border color.
* `h1, h2, h3, h4, h5, h6`: Sets styling from configurable variables.


## Configurable Variables

* `--base-typography-color`
* `--base-typography-fontFamily`
* `--base-typography-fontSize: `
* `--base-typography-fontWeight`
* `--base-typography-hrule-width`
* `--base-typography-letterSpacing`
* `--base-typography-lineHeight: `
* `--base-typography-spacing: `
* `--base-typography-link-color`
* `--base-typography-link-colorHover`
* `--base-typography-link-decoration`
* `--base-typography-link-decorationHover`
* `--base-typography-h1-fontSize`
* `--base-typography-h2-fontSize`
* `--base-typography-h3-fontSize`
* `--base-typography-h4-fontSize`
* `--base-typography-h5-fontSize`
* `--base-typography-h6-fontSize`
* `--base-typography-h1-lineHeight`
* `--base-typography-h2-lineHeight`
* `--base-typography-h3-lineHeight`
* `--base-typography-h4-lineHeight`
* `--base-typography-h5-lineHeight`
* `--base-typography-h6-lineHeight`
* `--base-typography-heading-color`
* `--base-typography-heading-fontFamily`
* `--base-typography-heading-fontWeight`
* `--base-typography-heading-letterSpacing`