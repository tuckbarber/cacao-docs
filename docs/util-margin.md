---
   id: margin
   title: Margin
---

Add margin spacing in various sizes. The difference with the padding gutters is that this 
uses margins instead of padding.

## Available classes

### Gutters
* `u-guttersMarg0`: Set size of gutters to zero.
* `u-guttersMarg1`: Gives gutter of size factor 1.
* `u-guttersMarg2`: Gives gutter of size factor 2.
* `u-guttersMarg3`: Gives gutter of size factor 3.
* `u-guttersMarg4`: Gives gutter of size factor 4.

### Bottom margin
* `u-margBottom0`: Set size of bottom margin to zero.
* `u-margBottom1`: Gives bottom margin of size factor 1.
* `u-margBottom2`: Gives bottom margin of size factor 2.
* `u-margBottom3`: Gives bottom margin of size factor 3.
* `u-margBottom4`: Gives bottom margin of size factor 4.
* `u-margBottom5`: Gives bottom margin of size factor 5.
* `u-lg-margBottom0`: Set size of bottom margin to zero.
* `u-lg-margBottom1`: Gives bottom margin of size factor 1 (large).
* `u-lg-margBottom2`: Gives bottom margin of size factor 2 (large).
* `u-lg-margBottom3`: Gives bottom margin of size factor 3 (large).
* `u-lg-margBottom4`: Gives bottom margin of size factor 4 (large).
* `u-lg-margBottom5`: Gives bottom margin of size factor 5 (large).
* `u-md-margBottom0`: Set size of bottom margin to zero.
* `u-md-margBottom1`: Gives bottom margin of size factor 1 (medium).
* `u-md-margBottom2`: Gives bottom margin of size factor 2 (medium).
* `u-md-margBottom3`: Gives bottom margin of size factor 3 (medium).
* `u-md-margBottom4`: Gives bottom margin of size factor 4 (medium).
* `u-md-margBottom5`: Gives bottom margin of size factor 5 (medium).
* `u-sm-margBottom0`: Set size of bottom margin to zero.
* `u-sm-margBottom1`: Gives bottom margin of size factor 1 (small).
* `u-sm-margBottom2`: Gives bottom margin of size factor 2 (small).
* `u-sm-margBottom3`: Gives bottom margin of size factor 3 (small).
* `u-sm-margBottom4`: Gives bottom margin of size factor 4 (small).
* `u-sm-margBottom5`: Gives bottom margin of size factor 5 (small).

### Top margin
* `u-margTop0`: Set size of top margin to zero.
* `u-margTop1`: Gives top margin of size factor 1.
* `u-margTop2`: Gives top margin of size factor 2.
* `u-margTop3`: Gives top margin of size factor 3.
* `u-margTop4`: Gives top margin of size factor 4.
* `u-margTop5`: Gives top margin of size factor 5.
* `u-lg-margTop0`: Set size of top margin to zero.
* `u-lg-margTop1`: Gives top margin of size factor 1 (large).
* `u-lg-margTop2`: Gives top margin of size factor 2 (large).
* `u-lg-margTop3`: Gives top margin of size factor 3 (large).
* `u-lg-margTop4`: Gives top margin of size factor 4 (large).
* `u-lg-margTop5`: Gives top margin of size factor 5 (large).
* `u-md-margTop0`: Set size of top margin to zero.
* `u-md-margTop1`: Gives top margin of size factor 1 (medium).
* `u-md-margTop2`: Gives top margin of size factor 2 (medium).
* `u-md-margTop3`: Gives top margin of size factor 3 (medium).
* `u-md-margTop4`: Gives top margin of size factor 4 (medium).
* `u-md-margTop5`: Gives top margin of size factor 5 (medium).
* `u-sm-margTop0`: Set size of top margin to zero.
* `u-sm-margTop1`: Gives top margin of size factor 1 (small).
* `u-sm-margTop2`: Gives top margin of size factor 2 (small).
* `u-sm-margTop3`: Gives top margin of size factor 3 (small).
* `u-sm-margTop4`: Gives top margin of size factor 4 (small).
* `u-sm-margTop5`: Gives top margin of size factor 5 (small).

## Configurable variables
* `--utils-margin-gutter`: The base size for the`u-guttersMarg` utilities.
* `--utils-margin-bottom`: The base size for the`u-margBottom` utilities.
* `--utils-margin-lg-bottom`: The base size for the`u-lg-margBottom` utilities.
* `--utils-margin-md-bottom`: The base size for the`u-md-margBottom` utilities.
* `--utils-margin-sm-bottom`: The base size for the`u-sm-margBottom` utilities.
* `--utils-margin-top`: The base size for the`u-margTop` utilities.
* `--utils-margin-lg-top`: The base size for the`u-lg-margTop` utilities.
* `--utils-margin-md-top`: The base size for the`u-md-margTop` utilities.
* `--utils-margin-sm-top`: The base size for the`u-sm-margTop` utilities.

<style>
.example-parent{
    border: 2px #ddd solid;
    display: block;
}
.example-parent > span{
    border: 1px #555 solid;
    display: inline-block;
    vertical-align: bottom;
</style>

<div class="code-sample">
    u-margBottom
    <div class="example-parent">
        <span class="u-margBottom0">Margin size 0 </span>
        <span class="u-margBottom1">Margin size 1 </span>
        <span class="u-margBottom2">Margin size 2 </span>
        <span class="u-margBottom3">Margin size 3 </span>
        <span class="u-margBottom4">Margin size 4 </span>
        <span class="u-margBottom5">Margin size 5 </span>
    </div>
</div>