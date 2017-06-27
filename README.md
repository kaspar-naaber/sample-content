# Sample content for testing and styling editable content areas in Voog CMS.

A good practice is to wrap any `{% editable %}`, `{% content %}`, `{% contentblock %}{% endcontentblock %}` etc. into a wrapper element with a specific class and style all the sample elements in this scope.

For example:

```html
<style>
  .content-area h1 {
    font-size: 24px;
    color: red;
  }

  .content-area p {
    font-size: 16px;
    color: green;
  }
</style>

<div class="content-area">{% content %}</div>

<div class="content-area">{% editable element.description %}</div>

<div class="content-area">{% contentblock %}Hello world!{% endcontentblock %}</div>
```
