---
id: form
title: Form
---

Provides custom styling for form fields and their various states.

## FormError

### Available classes

* `FormError`: Indicates that there is an error in form.
* `FormError-list`: Display a list of form errors.
* `FormError-listItem`: One of errors within error list.

### Usage

<div class="code-sample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="FormError">
    <h3>There are errors in the submitted form</h3>
    <ul class="FormError-list">
        <li class=FormError-listItem> Here is one issue </li>
        <li class=FormError-listItem> This is another </li>
        <li class=FormError-listItem> This one's a doozy </li>
    <ul>
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->

<div class="FormError">
    <h3>There are errors in the submitted form</h3>
    <ul class="FormError-list">
        <li class=FormError-listItem> Here is one issue </li>
        <li class=FormError-listItem> This is another </li>
        <li class=FormError-listItem> This one's a doozy </li>
    <ul>
</div>

</div>

## FormLabel

### Available classes

* `FormLabel`: A label for a field within a form.
* `FormLabel--block`: Display label as a `block` element.

### Usage

<div class="code-sample">

<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<label class="FormLabel"> Enter favorite type of cloud: </label> 
<input type="text" name="cloud">

<label class="FormLabel FormLabel--block"> Reason for choice: </label> 
<input type="text" name="reason">
```
<!--END_DOCUSAURUS_CODE_TABS-->

<label class="FormLabel" for="cloud"> Enter favorite type of cloud: </label> 
<input type="text" name="cloud" id="cloud">

<label class="FormLabel FormLabel--block" for="cloud"> Reason for choice: </label> 
<input type="text" name="cloud" id="cloud">

</div>

## FormRequired

### Available Classes

* `FormRequired`: Indicates a required message within a form.

### Usage
<div class="code-sample">

<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="FormRequired">
    <b>Attention:</b> please give us your credit card number.
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<div class="FormRequired">
    <b>Attention:</b> please give us your credit card number.
</div>

</div>

## FormSuccess

### Available classes

* `FormSuccess`: Indicates that the form is successful.

### Usage
<div class="code-sample">

<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="FormSuccess">
    <b>Thank you:</b> we now have your credit card number.
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<div class="FormSuccess">
    <b>Thank you!</b> We now have your credit card number.
</div>

</div>

## SelectInput

Provides custom styles for select menu input fields.

Any `select` that is a child of a `.SelectInput` element will be styled.

### Available Classes

* `SelectInput`: Field wrapper that theme is applied to.

#### States

* `is-invalid`: For invalid-state select input styles.
* `is-valid`: For valid-state select input styles.

### Configurable Variables

* `--SelectInput-background`: Background color of the select field.
* `--SelectInput-border`: Border of select field.
* `--SelectInput-color`: The color of text.
* `--SelectInput-errorColor`: Text and outline color in the case of error.
* `--SelectInput-successColor`: Text and outline color in the case of success.

### Usage
<div class="code-sample">

<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="SelectInput">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin"> Linux </option>
        <option value="tst"> Smart Toaster </option>
    </select>
</div>

<div class="SelectInput is-invalid">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin"> Linux </option>
        <option value="tst" selected> Smart Toaster </option>
    </select>
</div>

<div class="SelectInput is-valid">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin" selected> Linux </option>
        <option value="tst"> Smart Toaster </option>
    </select>
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<div class="SelectInput">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin"> Linux </option>
        <option value="tst"> Smart Toaster </option>
    </select>
</div>

<div class="SelectInput is-invalid">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin"> Linux </option>
        <option value="tst" selected> Smart Toaster </option>
    </select>
</div>

<div class="SelectInput is-valid">
    <select>
        <option value="">--Select OS--</option>
        <option value="win"> Windows </option>
        <option value="mac"> Mac </option>
        <option value="lin" selected> Linux </option>
        <option value="tst"> Smart Toaster </option>
    </select>
</div>

</div>


## TextInput

Provides custom styling for text input fields and textareas.

### Available Classes

* `TextInput`: Styling for text input fields.

#### States

* `is-invalid`: For invalid-state text input styles.
* `is-valid`: For valid-state text input styles.

### Configurable Variables

* `--TextInput-background`: Background color around field area.
* `--TextInput-border`: Border around field area.
* `--TextInput-padding`: Padding within field area.
* `--TextInput-color`: Text color within field area.
* `--TextInput-errorColor`: Text and outline color in the case of error.
* `--TextInput-successColor`: Text and outline color in the case of success.

### Usage
<div class="code-sample">

<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<input type="text" class="TextInput" name="one">
<input type="text" class="TextInput is-invalid" name="two" value="index starts at 1">
<input type="text" class="TextInput is-valid" name="thr" value="index starts at 0">
```
<!--END_DOCUSAURUS_CODE_TABS-->
<input type="text" class="TextInput" name="one">
<input type="text" class="TextInput is-invalid" name="two" value="index starts at 1">
<input type="text" class="TextInput is-valid" name="thr" value="index starts at 0">
</div>

