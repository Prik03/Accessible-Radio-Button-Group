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
  <label> <input type="radio" name="fruit" value="apple" /> Apple </label>
  ```

  ```html
  <input type="radio" id="apple" name="fruit" value="apple" />
  <label for="apple">Apple</label>
  ```

## UI Design

- Simple and clean layout with accessible color contrast.
- Proper spacing and readable font for a better user experience.
- Uses plain HTML and CSS for clarity and learning purposes.

## File Structure

```
radio-button-accessibility-demo/
│
├── index.html        # Main HTML file demonstrating accessibility concepts
├── style.css         # Optional CSS file for styling
├── script.js         # Optional JavaScript file for enhancements
└── README.md         # Project documentation

```

## How to Run

1. Clone or download this repository:

```
git clone https://github.com/your-username/radio-button-accessibility-demo.git

```

2. Open the index.html file in any web browser.
3. Explore each example to understand how accessibility improves step by step.

## Accessibility Tips

- Always group related form controls using <fieldset> and <legend>.
- Ensure every input has a visible, descriptive label.
- Avoid removing outlines; they are important for keyboard focus.
- Test your forms using both screen readers and keyboard navigation.

## License

This project is licensed under the MIT License.
