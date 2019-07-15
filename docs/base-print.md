---
   id: print
   title: Print
---

## Affected Type Selectors


* `*`: Sets bagrounds to transparent, text to black, and removes shadows.
* `a`: Adds underline to links.
* `a[href]`: Adds value of href attribute in parentheses after link text.
* `abbr[title]:after`: Adds value of title attribute in parentheses after abbr text.
* `a[href^="#"]:after, a[href^="javascript:"]:after`: Don't show links that are fragment identifiers, or use the `javascript:` pseudo protocol.
* `pre`: Sets white-space to pre-wrap.
* `pre, blockquote`: Adds thin border and avoid having the page brak in the middle of element.
* `thead`: Displays as table-header-group.
* `tr, img`: Avoid page breaking in the middle of element.
* `p, h2, h3`: Avoid page breaking from separating small pieces of text.
* `h2, h3`: Avoid the page breaking after this element.
