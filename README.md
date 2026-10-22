# Stylized To-Do List

A small static web page that displays a styled to-do list, built with plain HTML and CSS. This project is a freeCodeCamp lab from the Responsive Web Design course ("Build a Stylized To-Do List"), focused on practicing list styling, spacing, and link states.

## Features

- Centered white card on a light gray page background, with rounded corners and a soft shadow
- Four to-do items, each in its own light green rounded box
- A checkbox and a linked label for every item (clicking the label toggles the checkbox)
- A nested list under each item with a square bullet and a helpful resource link
- Link styles for every state: default, visited, hover, focus, and active
- Links open in a new tab

## Project Structure

```
.
├── index.html   # Page structure: the to-do list, checkboxes, labels, and links
├── styles.css   # All visual styling
└── README.md    # Project documentation
```

## HTML Structure

The page uses one unordered list (`.todo-list`). Each list item contains:

1. An `input` of type `checkbox` with a unique `id`
2. A `label` whose `for` attribute matches that `id`
3. A nested unordered list (`.sub-item`) holding a list item with an anchor (`.sub-item-link`) that has a valid `href` and `target="_blank"`

## CSS Concepts Practiced

- **Spacing:** `margin-bottom` for the gap between items, `padding` for space inside each box, and `line-height` for readable text
- **Layout:** centering the card with `max-width` and `margin: 0 auto`
- **Box styling:** `border-radius`, `box-shadow`, and background colors
- **List styling:** removing default bullets with `list-style: none` and customizing nested bullets with `list-style: square`
- **Selectors:** class selectors, the child combinator (`.todo-list > li`), attribute selectors (`input[type="checkbox"]`), and `:last-child`
- **Link states:** `:visited`, `:hover`, `:focus`, and `:active` pseudo-classes

## Getting Started

1. Clone the repository:
   
  git clone <https://github.com/zakiya3037/To-Do-List.git>
   
2. Open the project folder.
3. Open `index.html` in any web browser. No build step or dependencies are needed.

## Customization

Colors and spacing are easy to change in `styles.css`:

| What to change | Where |
| --- | --- |
| Page background | `body { background-color }` |
| Card size and shape | `.todo-list { max-width, padding, border-radius }` |
| Item box color | `.todo-list > li { background-color }` |
| Gap between items | `.todo-list > li { margin-bottom }` |
| Link colors | `.sub-item-link` and its pseudo-classes |

## Accessibility Notes

- Every checkbox has an associated `label`, which makes the clickable area larger and works with screen readers.
- Links show a visible outline on keyboard focus.

## Acknowledgements

Based on the "Build a Stylized To-Do List" lab from [freeCodeCamp](https://www.freecodecamp.org/).