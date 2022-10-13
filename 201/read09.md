# HTML Forms and JS

## HTML Forms

1. **Forms** are important in web development because forms allow users to enter data, which is generally sent to a web server for processing and storage, or used on the client-side to immediately update the interface in some way.
2. Something to keep in mind is to remember that the bigger your form, the more you risk frustrating people and losing users. Keep it simple and stay focused: ask only for the data you absolutely need.
3. 5 form elements:

    - The **<form>** element formally defines a form and attributes that determine the form's behavior.
    - The **<fieldset>** element is a convenient way to create groups of widgets that share the same purpose, for styling and semantic purposes.
    - The text content of the **<legend>** element formally describes the purpose of the *fieldset* it is included inside.
    - The **<label>** element is the formal way to define a label for an HTML form widget.
    - The **<input>** HTML element is used to create interactive controls for web-based forms in order to accept data from the user. 

## Learn JS: Events

1. **Events** are actions or occurrences that happen in the system you are programming, which the system tells you about so your code can react to them.
2. The 2 arguments I must provide when using the **addEventListener()** method are the name of the event and a function to handle the event.
3. The **event object** automatically passes to an event handler to provide extra features and information. The **target** property of the event object is always a reference to the element the event occurred upon which is why it is important.
4. The difference between **event bubbling** and **event capturing** is the capturing phase works form the <html> tag to the click event and the bubbling phase works from the click event to out to the <html> tag.

### Sources

- <https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form>
- <https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form>
- <https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events>

[Back To Home](../README.md)
