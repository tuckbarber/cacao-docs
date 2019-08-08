---
   id: util-typography 
   title: Typography
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/typography/typography.css"></a>

## Available classes

#### Transforms
*  `u-textNoTransform`: No text transformation.
*  `u-textUpper`: Convert text to uppercase.

#### Styles
*  `u-styleNone`: No font style.
*  `u-styleEm`: Give text an italic style.

#### Horizontal alignment
*  `u-textCenter`: Center align text.
*  `u-textLeft`: Left align text.
*  `u-textRight`: Right align text.

#### Weight

* `u-weightNormal`: Set the font to a normal weight.
* `u-weightLight`: Set the font to a light weight.
* `u-weightBold`: Set the font to a bold weight.
* `u-weightLighter`: Set the font to a lighter weight.
* `u-weightBolder`: Set the font to a bolder weight.
* `u-weightLightest`: Set the font to a lightest weight.
* `u-weightBoldest`: Set the font to a boldest weight.

#### Font scale

* `u-fontSize1`: Set the font size factor to 1.
* `u-fontSize2`: Set the font size factor to 2.
* `u-fontSize3`: Set the font size factor to 3.
* `u-fontSize4`: Set the font size factor to 4.
* `u-fontSize5`: Set the font size factor to 5.
* `u-fontSize6`: Set the font size factor to 6.
* `u-fontSize7`: Set the font size factor to 7.
* `u-fontSize8`: Set the font size factor to 8.
* `u-fontSize9`: Set the font size factor to 9.
* `u-fontSize10`: Set the font size factor to 10.
* `u-fontSizeH1`: Set the font size factor to H1.
* `u-fontSizeH2`: Set the font size factor to H2.
* `u-fontSizeH3`: Set the font size factor to H3.
* `u-fontSizeH4`: Set the font size factor to H4.
* `u-fontSizeH5`: Set the font size factor to H5.
* `u-fontSizeH6`: Set the font size factor to H6.

#### Misc

* `u-textInheritColor`:  Text will inherit its ancestor's text color.
* `u-textBreak`: Break strings when their length exceeds the width of their container.
* `u-textNoWrap`: Prevent whitespace wrapping.
* `u-textKern`: Enables font kerning.
* `u-textTruncate`: Prevent text from wrapping onto multiple lines, and truncate with an ellipsis.

### Large Typography
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/typography/typography-lg.css"></a>

Only applies to viewports defined as large or smaller. 

*  `u-lg-textCenter`: Center align text.
*  `u-lg-textLeft`: Left align text.
*  `u-lg-textRight`: Right align text.

### Medium typography
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/typography/typography-md.css"></a>

Only applies to viewports defined as medium or smaller. 

*  `u-md-textCenter`: Center align text.
*  `u-md-textLeft`: Left align text.
*  `u-md-textRight`: Right align text.

### Small typography
<a class="SourceView-section" href="https://github.com/aptuitiv/cacao/blob/master/src/css/utils/typography/typography-sm.css"></a>

Only applies to viewports defined as small or smaller. 

*  `u-sm-textCenter`: Center align text.
*  `u-sm-textLeft`: Left align text.
*  `u-sm-textRight`: Right align text.


## Configurable variables

Adjusts each of the font scales' size and line height.

* `--utils-typography-fontSize-1`
* `--utils-typography-fontSize-2`
* `--utils-typography-fontSize-3`
* `--utils-typography-fontSize-4`
* `--utils-typography-fontSize-5`
* `--utils-typography-fontSize-6`
* `--utils-typography-fontSize-7`
* `--utils-typography-fontSize-8`
* `--utils-typography-fontSize-9`
* `--utils-typography-fontSize-10`
* `--utils-typography-lineHeight-1`
* `--utils-typography-lineHeight-2`
* `--utils-typography-lineHeight-3`
* `--utils-typography-lineHeight-4`
* `--utils-typography-lineHeight-5`
* `--utils-typography-lineHeight-6`
* `--utils-typography-lineHeight-7`
* `--utils-typography-lineHeight-8`
* `--utils-typography-lineHeight-9`
* `--utils-typography-lineHeight-10`

## Usage

<link href='//fonts.googleapis.com/css?family=Open+Sans:100,200,300,400,700,800,900' rel='stylesheet' type='text/css'>
<style>
.Example-parent{
    margin: 20px 10px;
    border-left: 2px #000 solid;
    font-family: 'Open Sans';
    padding-left: 10px;
}
.Example-parent > span {
    display: block;
}
</style>
<div class="CodeSample">
    <br>
    u-weight
    <div class="Example-parent" style="font-size: 2em;">
        <span class="u-weightLightest">u-weightLightest</span>
        <span class="u-weightLighter">u-weightLighter</span>
        <span class="u-weightLight">u-weightLight</span>
        <span class="u-weightNormal">u-weightNormal</span>
        <span class="u-weightBold">u-weightBold</span>
        <span class="u-weightBolder">u-weightBolder</span>
        <span class="u-weightBoldest">u-weightBoldest</span>
    </div>
    <br>
    u-fontSize
    <div class="Example-parent">
        <span class="u-fontSize1"> u-fontSize1 </span>
        <span class="u-fontSize2"> u-fontSize2 </span>
        <span class="u-fontSize3"> u-fontSize3 </span>
        <span class="u-fontSize4"> u-fontSize4 </span>
        <span class="u-fontSize5"> u-fontSize5 </span>
        <span class="u-fontSize6"> u-fontSize6 </span>
        <span class="u-fontSize7"> u-fontSize7 </span>
        <span class="u-fontSize8"> u-fontSize8 </span>
        <span class="u-fontSize9"> u-fontSize9 </span>
        <span class="u-fontSize10"> u-fontSize10 </span>
        <span class="u-fontSizeH1"> u-fontSizeH1 </span>
        <span class="u-fontSizeH2"> u-fontSizeH2 </span>
        <span class="u-fontSizeH3"> u-fontSizeH3 </span>
        <span class="u-fontSizeH4"> u-fontSizeH4 </span>
        <span class="u-fontSizeH5"> u-fontSizeH5 </span>
    </div>
</div>