# Assignment 6.1 - Box Model Inspection

## The Box Model

Every HTML element is a box made of four parts, from the inside to the outside:

1. Content: the text or image inside the element.
2. Padding: the space between the content and the border.
3. Border: the line around the padding.
4. Margin: the space outside the border that separates the box from other elements.

## Boxes Used

| Box | box-sizing | Padding | Border | Margin |
|---|---|---|---|---|
| Box One | content-box | 10px | 2px | 10px |
| Box Two | border-box | 30px | 8px | 30px |
| Box Three | content-box | 20px | 5px | 20px |

## content-box vs border-box

All three boxes have width: 300px.

- With content-box, the width only sets the content area. Padding and border are added on top, so Box One is 324px wide and Box Three is 350px wide.
- With border-box, the width includes the padding and border, so Box Two stays exactly 300px wide even with large padding and border.

This is why border-box is easier to use in layouts: the size you set is the size you get.

## DevTools Inspection

I opened Chrome DevTools, selected each box in the Elements tab, and looked at the box model diagram in the Computed panel. It shows the content, padding, border and margin sizes as nested colored rectangles.