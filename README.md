# cacao-docs
Documentation for the CSS Framework Cacao


This website for documentation was made using [Docusaurus](https://docusaurus.io/).

# Get Started in 5 Minutes

1. Make sure all the dependencies for the website are installed:

```sh
# Install dependencies
$ yarn
```
2. Run your dev server:

```sh
# Start the site
$ yarn start
```


# Uploading code to gh-pages

This can be done manually by running 
```sh
$ yarn run build
# or
$ npm run build
```

and deploying. However, an easy method is to use Docusaurus's built-in `publish-gh-pages`. Make sure that 
in `siteConfig.js` the `projectName`/`organizationName` are set accordingly:

```js
// Used for publishing and more
projectName: 'cacao-docs',
organizationName: 'GIT_USERNAME/ORGANIZATION_NAME',
```

You can then run the terminal command

```sh
$ GIT_USER="GIT_USERNAME" \npm run publish-gh-pages
```

# Making changes

Most information about file structure can be found on the Docusaurus site. This project uses minimal additional features, with no blog/users/i18n.

## Doc structure

Any changes to the actual Documentation itself can be made in the `docs/` directory. The different types of modules of the Cacao framework, Base, Components, and Utilities were given `base-`/`comp-`/`util-` prefixes respectively in order to group them alphabetically and differentiate them. This is was done because Docusaurus v1 does not yet support sub-directories in the documentation directory.

Each file begins with a header, for example

```
---
id: grid
title: Grid
---
```

The id is used to identify the file, and the title is displayed as the main heading of that doc page.

In order to add/change the documentation pages, changes must be made to `sidebars.json` by putting the id's from the header of the corresponding .md file in the array of the desired section within `docs`. For example
 
```js
"Components": ["grid", ...]
```

For more information about docs, click [here](https://docusaurus.io/docs/en/navigation).

## Custom CSS

There are CSS classes custom to this project in `static/css/custom.css`.

## Markdown

The doc pages use a mixture of markdown and html to show examples of the elements. The styles needed to display the examples are contained in inline `<style>` tags at the top of the file because many examples on the page use the same CSS. 

Code samples with multiple tabs for HTML/CSS are put in `.CodeSample` divs and use `<!--DOCUSAURUS_CODE_TABS-->` to get the code tab format. The format for Docusaurus code tabs is:

````html
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
HTML TEXT HERE
```
<!--CSS-->
```css
CSS TEXT HERE
```
<!--END_DOCUSAURUS_CODE_TABS-->
````

and inside the `CodeSample` div, that would look like

````html
<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->
<!--HTML-->
```html
HTML TEXT HERE
```
<!--CSS-->
```css
CSS TEXT HERE
```
<!--END_DOCUSAURUS_CODE_TABS-->
HTML CODE FOR EXAMPLE GOES HERE
</div>
````

*Note:* discretion should be taken with indentation and spacing for code sample code, otherwise the markdown parser will surround HTML with `<p>` tags, causing undesired effects. This usually means that first example tag after `<!--END_DOCUSAURUS_CODE_TABS-->` can't be indented or have an extra line break between.

For an example that is just visual with no code, the html for the example can go directly in the `CodeSample` div. If the element would benefit from padding, then `CodeSample--padded` can be used.

```html
<div class="CodeSample">
HTML HERE
</div>

<!-- or -->

<div class="CodeSample CodeSample--padded">
HTML HERE
</div>
```

## Linking GitHub Source
There are two classes to place a button for the GitHub source for a specific piece of code.

An `<a>` tag with a `SourceView-page` class should be placed at the top of the .md file under the header.

```md
---
id: SOME ID
title: SOME TITLE
---

<a class="SourceView-page" href="GITHUB URL"></a>
``` 

If the module has multiple files or classes, you can link to a specific CSS file in that directory. To get a source button next to a markdown header, just place an `<a>` tag with the class `SourceView-section` directly under the heading. 

```md
## SOME SECTION HEADER
<a class="SourceView-section" href="GITHUB URL"></a>
``` 



