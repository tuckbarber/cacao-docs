---
   id: base
   title: Base
---



## Affected Type Selectors

 * `body`: Sets body background color as a best practice.
 * `img`:
    * Sets alt text style to italic.
    * Scales image fluidity with its container for rich text editor convenience.
    * Align to middle to prevent white space created by aligning to text baseline.
 * `iframe`: Removes the default border from iframes.
 * `[role='button']`: Fixes clickability of issue for traditionally non-focusable elements with role='button'.
 * `[tabindex='-1]`: Suppresses focus outline on non-focusable items.
 * `a, area, button, [role='button'], input, label, select, summary, textarea`: Avoid 300ms click delay on devices that support the 'touch-action' CSS property.
 * `button` : Work around a Firefox/IE bug where the transparent `button` background results in a loss of the default `button` focus styles.
 * `hidden`: Always hiden an element with `hidden` HTML attribute.
 
 ## Configurable Variables
 
 * `--base-body-background`: The background color of the body of the document.