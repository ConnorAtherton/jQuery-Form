jQuery-Form
===========

OK I know I'm reinventing the wheel with this but I thought it would be good practice to build one myself so I would better understand how other form plugins work.

It works, Hurrah! However, it's very brittle and requires the form elements and corresponding error messages to manually be entered into each array in the same order, which isn't exactly ideal. Also, each input can only have one validation rule which isn't too handy for mosy applications. This plugin definitely works better in small (tiny!) projects.

Here's how to create a new form..

```JavaScript
var exampleForm = new Form({
	url: mailUrl,
    fields: 'form input, form textarea',
    status: '#status',
    submit: '#submit'
})

exampleForm.init()
```
Pretty simple, just pass in..

* The url to send the form data too
* The form fields all encapsulated in one string seperated by commas in the correct order of validation rules.
* Selector string where you want the status message to go
* The submit selector. This element will actually submit the form 

If you have any suggestions about how to improve this (or my coding style in general) just get in touch.
