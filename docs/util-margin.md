---
   id: margin
   title: Margin
---

Add margin spacing in various sizes, with modifiers for large/medium/small screens. The 
difference with the padding gutters is that this uses margins instead of padding.



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
* `u-lg-margBottom1`: Gives bottom margin of size factor 1 (large displays).
* `u-lg-margBottom2`: Gives bottom margin of size factor 2 (large displays).
* `u-lg-margBottom3`: Gives bottom margin of size factor 3 (large displays).
* `u-lg-margBottom4`: Gives bottom margin of size factor 4 (large displays).
* `u-lg-margBottom5`: Gives bottom margin of size factor 5 (large displays).
* `u-md-margBottom0`: Set size of bottom margin to zero.
* `u-md-margBottom1`: Gives bottom margin of size factor 1 (mediu displaysm).
* `u-md-margBottom2`: Gives bottom margin of size factor 2 (mediu displaysm).
* `u-md-margBottom3`: Gives bottom margin of size factor 3 (mediu displaysm).
* `u-md-margBottom4`: Gives bottom margin of size factor 4 (mediu displaysm).
* `u-md-margBottom5`: Gives bottom margin of size factor 5 (mediu displaysm).
* `u-sm-margBottom0`: Set size of bottom margin to zero.
* `u-sm-margBottom1`: Gives bottom margin of size factor 1 (small displays).
* `u-sm-margBottom2`: Gives bottom margin of size factor 2 (small displays).
* `u-sm-margBottom3`: Gives bottom margin of size factor 3 (small displays).
* `u-sm-margBottom4`: Gives bottom margin of size factor 4 (small displays).
* `u-sm-margBottom5`: Gives bottom margin of size factor 5 (small displays).

### Top margin
* `u-margTop0`: Set size of top margin to zero.
* `u-margTop1`: Gives top margin of size factor 1.
* `u-margTop2`: Gives top margin of size factor 2.
* `u-margTop3`: Gives top margin of size factor 3.
* `u-margTop4`: Gives top margin of size factor 4.
* `u-margTop5`: Gives top margin of size factor 5.
* `u-lg-margTop0`: Set size of top margin to zero.
* `u-lg-margTop1`: Gives top margin of size factor 1 (large displays).
* `u-lg-margTop2`: Gives top margin of size factor 2 (large displays).
* `u-lg-margTop3`: Gives top margin of size factor 3 (large displays).
* `u-lg-margTop4`: Gives top margin of size factor 4 (large displays).
* `u-lg-margTop5`: Gives top margin of size factor 5 (large displays).
* `u-md-margTop0`: Set size of top margin to zero.
* `u-md-margTop1`: Gives top margin of size factor 1 (mediu displaysm).
* `u-md-margTop2`: Gives top margin of size factor 2 (mediu displaysm).
* `u-md-margTop3`: Gives top margin of size factor 3 (mediu displaysm).
* `u-md-margTop4`: Gives top margin of size factor 4 (mediu displaysm).
* `u-md-margTop5`: Gives top margin of size factor 5 (mediu displaysm).
* `u-sm-margTop0`: Set size of top margin to zero.
* `u-sm-margTop1`: Gives top margin of size factor 1 (small displays).
* `u-sm-margTop2`: Gives top margin of size factor 2 (small displays).
* `u-sm-margTop3`: Gives top margin of size factor 3 (small displays).
* `u-sm-margTop4`: Gives top margin of size factor 4 (small displays).
* `u-sm-margTop5`: Gives top margin of size factor 5 (small displays).

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

## Usage

<style>
.example-parent{
    border: 2px #bbb dashed;
    display: inline-block;
}
.example-parent > span{
    background-color: #329A5C;
    color: #FFF;
    display: inline-block;
    margin-bottom: 10px;
    padding: 5px;
    vertical-align: bottom;
}
</style>

<div class="code-sample code-sample--padded">
    u-guttersMarg
    <br>   
    <div class="example-parent">
        <span class="u-guttersMarg0"> Gutters size 0 </span>
        <br>
        <span class="u-guttersMarg1"> Gutters size 1 </span>
        <br>
        <span class="u-guttersMarg2"> Gutters size 2 </span>
        <br>
        <span class="u-guttersMarg3"> Gutters size 3 </span>
        <br>
        <span class="u-guttersMarg4"> Gutters size 4 </span>
    </div>
    <br>
    <br>
    u-margBottom
    <br>
    <div class="example-parent">
        <span class="u-margBottom0">Margin size 0 </span>
        <span class="u-margBottom1">Margin size 1 </span>
        <span class="u-margBottom2">Margin size 2 </span>
        <span class="u-margBottom3">Margin size 3 </span>
        <span class="u-margBottom4">Margin size 4 </span>
        <span class="u-margBottom5">Margin size 5 </span>
    </div>
</div>
