html5-paper-input
================

## See the [component page](http://cbalit.github.io/html5-paper-input) for more information.

## Installation

````
bower install html5-paper-input
````
## Usage

Because the component is built on Polymer, you should add the script in your page
```html
<script src="webcomponentsjs/webcomponentsjs.js"></script>
```


Import the component:
```html
<link rel="import" href="html5-paper-input.html">
```

use it:
```html
 <html5-paper-input label="Required field" required floatinglabel></html5-paper-input>
```

## Error message

You can customize error messages by:
* setting the error attribute: The same message will be displayed regardless of the type of error
```html
 <html5-paper-input label="Required field" required error="You must enter a value"></html5-paper-input>
```
* setting a custom error map  with the setMessage method:
 ```
  var input = document.querySelector('html5-paper-input');
  input.setMessage({valueMissing:"You must enter a value"});
 ```
 The keys are:
  * valueMissing: message for require error
  * patternMismatch: message for pattern error
  * rangeUnderflow: message for min error
  * rangeOverflow: message for max error
  * tooLong: message for maxlength error
  * default: message for default error
