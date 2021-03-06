---
title: Use PropTypes to Define the Props You Expect
---
# Use PropTypes to Define the Props You Expect

---
## Problem Explanation
This challenge has you set a `propTypes` for the `Items` component.
```jsx
const Items = (props) => {
  return <h1>Current Quantity of Items in Cart: {props.quantity}</h1>
};
```

To set a propTypes, the syntax to be followed is
```jsx
itemName.propTypes = {
  props: PropTypes.dataType.isRequired
};
```

---
## Solutions

<details><summary>Solution 1 (Click to Show/Hide)</summary>

Following the Syntax, the following code should be set below the given code for the `quantity` props of `Items` component
```jsx
Items.propTypes = {
  quantity: PropTypes.number.isRequired
};
```

</details>