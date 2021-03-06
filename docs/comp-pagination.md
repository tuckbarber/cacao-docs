---
id: pagination
title: Pagination
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/pagination/pagination.css"></a>

Pagination for iterative pages.

## Available classes

* `Pagination`: The core pagination component.
* `Pagination-item`: A child of the pagination component.
* `Paination-item--previous`: A pagination element to the left of the current item.
* `Pagination-item--isActive`: Current pagination element.

## Usage
<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
<div class="Pagination">
  <a href="#" class="Pagination-item">1</a>
  <a href="#" class="Pagination-item">2</a>
  <a href="#" class="Pagination-item Pagination-item--isActive">3</a>
  <a href="#" class="Pagination-item">4</a>
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="Pagination">
  <a href="#" class="Pagination-item">1</a>
  <a href="#" class="Pagination-item">2</a>
  <a href="#" class="Pagination-item Pagination-item--isActive">3</a>
  <a href="#" class="Pagination-item">4</a>
</div>
</div>