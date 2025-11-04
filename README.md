# Radio Button Accessibility Demo

This project demonstrates how to make **radio buttons accessible** using proper **grouping**, **label association**, and the **`name` attribute**.  
It includes examples showing both correct and incorrect implementations to help understand best practices for web accessibility.

---

## Overview

Radio buttons are commonly used in forms to allow users to select one option from multiple choices.  
However, without proper HTML structure and labeling, they can be confusing for screen reader users or those navigating via keyboard.

This demo covers:

1. Without Grouping — radio buttons presented without context.
2. With Grouping — using `<fieldset>` and `<legend>` to define related options.
3. Using the `name` Attribute — to connect radio buttons in one logical group.
4. Label Association — comparing labeled vs. unlabeled inputs for clarity and accessibility.

---

## Key Concepts

### 1. Grouping Radio Buttons
- Use `<fieldset>` and `<legend>` to group related radio buttons.  
- Screen readers announce the group name before reading the options.
- Improves context and structure for users.

### 2. The `name` Attribute
- The `name` attribute connects radio buttons functionally.  
- Only one radio button in a group with the same `name` can be selected.
- Assists both browsers and assistive technologies in identifying the group.

### 3. Label Association
- Labels describe the purpose of form elements.
- Associating a label ensures the option is announced correctly by screen readers.
- Two correct methods:
  ```html
  <label>
    <input type="radio" name="fruit" value="apple"> Apple
  </label>
