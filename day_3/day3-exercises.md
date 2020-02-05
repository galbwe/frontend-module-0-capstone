# Frontend Mod 0 Capstone - Day 3 Exercises

## Form Questions

1. When using an input element in a form, the `type` attribute controls the behavior of the input.
2. The *select* element is used to create a dropdown list.
3. To send form data to a server with an input element, the `type` attribute should be set to `submit`.
4. Similar from items can be grouped together in the *fieldset* element.

## Box Sizing and Layout Questions

1. Border, padding, and margin are 3 components of an element's box.
   1. An element's *border* surrounds the edge of its box. It separates the inside of the box from the outside.
   2. An element's *margin* is the space outside the box. It creates space between adjacent elements.
   3. An element's *padding* is the space inside the box which separates the element's border from its content.
2. A css rule like `padding: 1px 2px 10px 20px;` is used as shorthand for separately defining the properties
    `padding-top`, `padding-right`, `padding-bottom`, and `padding-left`. These order of the directions in these
    rules is always *top*, *right*, *bottom*, *left*. You can also specify one or two values separated by spaces.
    For example, the rule `margin: 10px 20px;` will set both `margin-top` and `margin-bottom` to `10px`, and `margin-left` and `margin-right` to `20px`. The rule `padding: 15px;` will set the padding for all directions simultaneously.
3. Block level elements always start on a new line. Example include headers, paragraphs and list items. Inline level elements
   do not start on a new line. An element can be forced to be block level or inline level with the rules `display: inline;` and `display: block;`.
4. Fixed positioning is used to take an element out of the normal document flow, and place it somewhere in the window. Fixed position elements do not move relative to the browser window as the user scrolls. When an element is taken out of the usual document flow, it may overlap with other elements. The `z-index` property is used to determine which element is displayed when two or more elements overlap.
5. Elements in fixed layouts do not change size as the user changes the browser window size. In contrast, elements in liquid layouts dynamically adjust their size as the browser window size changes. Liquid layouts are becoming more common as devices with varying screen sizes have become more popular. 
