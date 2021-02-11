# Reading 03 Notes

[Home](README.md)

## Templating with Mustache
### What is Javascript templating?
This is a way to efficiently render a client-side template with Javascript using JSON files. 
An example is {{ name }} This is a Mustache syntax which tells us that this is a placeholder. 

## A Guide to Flexbox https://css-tricks.com/snippets/css/a-guide-to-flexbox/
justify-content has a few inputs it can take:
1. flex-start: this puts everything toward the start or left of the flex-direction
2. flex-end: this puts everything toward the end or right of the flex-direction
3. center: this centers all of the content
4. space-between: this puts spaces, the first item is on the start line, the last item on the end line and anything between them are spaces in the center
5. space-around: this spaces the content evenly within the area it is contained

## Flexbox Froggy https://flexboxfroggy.com/
align-items
1. flex-start: items align to the top of the container
2. flex-end: items align to the bottom of the container
3. center: items align at the vertical center of the container
4. baseline: items display at the baseline of the container.
5. stretch: items are stretched to fit the container.

flex-direction
1. row: items are placed the same as the text direction
2. row-reverse: items are placed opposite to the text direction
3. column: items are places top to bottom
5. column-reverse: items are places bottom to top

> if the row is reversed then so is the order of the flex-start and flex-end

order
This used to change the order of the frogs. (-2, -1, 0, 1, 2)

flex-wrap
nowrap: every item is fit to a single line
wrap: items wrap around to additional lines
wrap-reverse: items wrap around to additional lines in reverse

> flex-flow: row wrap sets rows and wraps them

align-content
1. flex-start: lines are packed at the top of the container
2. flex-end: lines are packed at the bottom of the container
3. center: lines are packed at the vertical center of the container
4. space-between: lines display with equal spacing between them.
5. space-around: lines display with equal spacing around them
6. stretch: lines are stretched to fit the container

