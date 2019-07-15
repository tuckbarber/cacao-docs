---
   id: forms
   title: Forms
---

## Affected Type Selectors

* `fieldset`: Sets border, margin, padding to zero.
* `label`: Allows margins to use magin for spacing.
* `input, button, select, textarea`: 
    * Removes rounded borders.
    * Sets line-height to inherit.
    * Removes all margin.
* `textarea`: 
    * Only allows for vertical resizing to prevent layouts from breaking.
    * Easier to read default alignment.
* `input[type='search']`: Overrides the extra rounded corners on search inputs in iOS.
* `input[type='radio'], input[type='checkbox']`: Add right margin to radio buttons and checkboxes.
* `html input[disabled], html input[readonly]`: Change background color.