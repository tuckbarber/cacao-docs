---
id: form
title: Form Component
---

Provides custom styling for form fields and their various states.

## FormError

### Available classes

* `FormError`: Indicates that there is an error in form.
* `FormError-list`: Display a list of form errors.
* `FormError-listItem`: One of errors within error list.

## FormLabel

### Available classes

* `FormLabel`: A label for a field within a form.
* `FormLabel--block`: Display label as a `block` element.


## FormRequired

### Available Classes

* `FormRequired`: Indicates a required message within a form.

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


## FormSuccess

### Available classes

* `FormSuccess`: Indicates that the form is successful.


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