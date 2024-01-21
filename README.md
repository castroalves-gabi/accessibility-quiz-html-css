# Acessibility: Quiz

[Project Link
](https://accessibility-quiz-html-css.vercel.app/)

![project-img](https://github.com/castroalves-gabi/accessibility-quiz-html-css/assets/117552601/64c0dbb5-29f4-4de5-b052-7985f5703821)

## Learnings reinforced through this project:

### Placeholder Considerations

  Placeholder text is not ideal for accessibility, as users might mistake the example text for a pre-filled input.
  Example: Prefer using explicit labels instead of relying exclusively on placeholders.
  Screen Reader-Only Text:
  
  To include text that only screen readers will read, utilize the following CSS properties:
  
    position: absolute;
    width: 1px; 
    height: 1px; 
    padding: 0;
    margin: -1px; 
    overflow: hidden; 
    clip: rect(0, 0, 0, 0);
    white-space: nowrap; 
    border: 0;


### Flexbox Properties:
  
  `justify-content: space-between; align-items: center;`

### Positioning:

position: fixed;: Fixes an element on the screen even when the user scrolls.
top: 0;: Defines the distance of the fixed element relative to the top of the browser window.

### Flexbox Wrap:

`flex-wrap: wrap;`
Indicates that items should be arranged in multiple lines (or columns, depending on the flexible container's orientation) if they don't fit in a single line.

### Inline Elements:

Inline elements flow within the text context, not starting on a new line.
Width and height cannot be explicitly set for inline elements.

### Block Elements:

Block elements start on a new line and occupy the full available width of the parent container.
Width, height, margins, and padding can be defined for block elements.

### Inline-Block:

Combines characteristics of inline and block elements.
Flows within the text context like inline elements.
Allows the definition of width, height, margins, and padding like block elements.
List Style in Item Bullets:

Property list-style-type offers various options, including:

- list-style-type: disc; /* Default */
- list-style-type: circle; /* Hollow Circle */
- list-style-type: square; /* Square */
- list-style-type: decimal; /* Decimal Numbers */
- list-style-type: decimal-leading-zero; /* Decimal Numbers with Leading Zeros */
- list-style-type: lower-roman; /* Lowercase Roman Numerals */
- list-style-type: upper-roman; /* Uppercase Roman Numerals */
- list-style-type: lower-alpha; /* Lowercase Alphabet Letters */
- list-style-type: upper-alpha; /* Uppercase Alphabet Letters */
- list-style-type: none; /* No Bullets */
- Additionally, you can use images as bullets:

  `list-style-type: none;
  list-style-image: url('image-path.png');`

### Scroll-Behavior:

CSS property that defines the scrolling behavior of a container when its position changes.
- Default: auto (browser/platform-specific behavior).
- Option: smooth provides a smooth transition between scroll positions.

### aria-labelledby Attribute:

ARIA attribute to associate HTML elements, enhancing web application accessibility.
Used to link an element to another serving as a label or tag.
Example usage provided.
prefers-reduced-motion Media Feature:

A media feature within @media to define CSS based on user preferences.
Values: reduce, no-preference.
Example:


`@media (prefers-reduced-motion: no-preference) {
  html { 
    scroll-behavior: smooth; 
  }
}`

### Accesskey Attribute:

Improves navigation accessibility by providing keyboard shortcuts.
The accesskey attribute accepts a list of access keys separated by spaces.

`<button type="submit" accesskey="s">Submit</button>`
