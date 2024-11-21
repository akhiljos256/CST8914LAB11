
# Lab 11: Accessible Custom Components & Widgets

## Questions and Answers

### 1. What is the keyboard interaction missing?

The original accordion component lacked essential keyboard interactions, including focus navigation, where users were unable to navigate between accordion buttons using the Tab key due to the absence of proper focus styles and keyboard support. Additionally, it did not support expanding or collapsing sections using the `Enter` or `Space` keys, which is a standard accessibility feature for interactive elements like buttons.


### 2. What is the ARIA missing?

The original accordion component lacked essential ARIA attributes for accessibility, including **`aria-expanded`**, which was missing on the buttons to indicate whether a section was expanded or collapsed, and **`aria-controls`**, which was not used to link each button to its corresponding content section, preventing screen readers from associating the button with the collapsible region. Additionally, the content sections lacked the **`role="region"`** attribute to mark them as landmark regions for screen readers, and **`aria-labelledby`** was missing on the content sections to associate them with the corresponding buttons. Addressing these issues has made the component fully accessible, supporting both keyboard navigation and screen reader users.