# Silent Failure in HTML: Missing Element Check

This repository demonstrates a common yet subtle error in JavaScript interacting with the DOM. The code attempts to manipulate an HTML element's style without first checking if the element exists.  This leads to a silent failure—no error message is displayed, but the intended action (showing the hidden text) does not occur.

## Bug Description

The JavaScript function `showText()` tries to change the `display` style of the element with the ID `myDiv` to make it visible. However, it doesn't check if `document.getElementById('myDiv')` returns a valid element. If the element doesn't exist, the code will run without errors, but the text won't show, leading to unexpected behavior. 

## Solution

The solution involves adding a check to verify that the element exists before manipulating its style.  This prevents the silent failure and provides a more robust and reliable interaction with the DOM.
