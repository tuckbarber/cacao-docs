---
id: message
title: Message
---

<a class="SourceView-page" href="https://github.com/aptuitiv/cacao/blob/master/src/css/components/message/message.css"></a>

### Available classes

* `Message`: The core message component.
* `Message--success`: Indcates a message of success.
* `Message--error`: Indicates an error message.

### Configurable variables

* `--Message-padding`: Padding in the message area.
* `--Message-border-radius`: Border radius of the message area.
* `--Message-background`: Background color of the message area.
* `--Message-borderColor`: Border around the message area.
* `--Message-color`: Text color of the message.
* `--Message-success-background`: Message area background color in case of success.
* `--Message-success-borderColor`: Message area border color in case of success.
* `--Message-success-color`: Message area text color in case of success.
* `--Message-error-background`: Message area background color in case of error.
* `--Message-error-borderColor`: Message area border color in case of error.
* `--Message-error-color`: Message area text color in case of error.

<div class="CodeSample">
<!--DOCUSAURUS_CODE_TABS-->

<!--HTML-->
```html
<div class="Message">
    <b>Hello,</b> this is a message.
</div>
<br>
<div class="Message Message--error">
    <b>Error:</b> task has failed to succeed.
</div>
<br>
<div class="Message Message--success">
    <b>Success:</b> task has successfully failed. 
</div>
```
<!--END_DOCUSAURUS_CODE_TABS-->
<div class="Message">
    <b>Hello,</b> this is a message.
</div>
<br>
<div class="Message Message--error">
    <b>Error:</b> task has failed to succeed.
</div>
<br>
<div class="Message Message--success">
    <b>Success:</b> task has successfully failed. 
</div>

</div>