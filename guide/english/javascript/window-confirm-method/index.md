---
title: Window Confirm Method
---
## Window Confirm Method

You can use the `confirm` method to ask a user to double check a decision on a web page. When you call this method, the browser will display a dialog box with two choices along the lines of "OK" and "Cancel."

For example, say someone has just clicked a Delete button. You could run the following code:

```javascript
if (window.confirm("Are you sure you want to delete this item?")) {
  // Delete the item
}
```

The message "Are you sure you want to delete this item?" will appear in the dialog box. If the user clicks "OK", the confirm method will return `true` and the browser will run the code inside the if statement. If the user clicks "Cancel" or the close button(x) in the top right corner, the method will return `false` and nothing else will happen. This provides some protection against someone accidentally clicking Delete.

**Note**: This method takes the focus away from the current window as it prevents the user from accessing other parts of the page until the box is closed.

#### More Information:
<a href='https://developer.mozilla.org/en-US/docs/Web/API/Window/confirm' target='_blank' rel='nofollow'>MDN Docs</a>
