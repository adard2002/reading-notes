# Reading 04 Notes

[Home](README.md)
# CSS Grid

## CSS Grid Garden
Grid-column-start is where you want to start or where you want to select the beginning of the area you want to start at.
grid-column-end is where the selected area will end. 

grid-column-end: span 2; is how many squares are going to be selected

grid-row-start is where you want the selected area to start.

grid-column: and grid-row allows you to select a large area. an example is a 5 x 5 grid and you want to select everything from the 2nd column from the 5th column. All of those rows have carrots in them and you want to select everywhere with carrots. so you would do:
grid-column: 2/6;
grid-row: 1/6;

grid-area: lets you select a bigger area: 1 / 1 / 1 / 1;

grid-template-columns: 20% 20% 20% 20% 20% this lets you create how many columns you want in your grid. each 20% is it's own column. In this example there are 5 columns
grid-template-columns: repeat(5, 12.5); is an easier way to make columns and set the width and height of it.

## Regex Tutorial
### Anchors-^ and $ 
- ^The        matches any string that <b>starts with The</b>
- end$        matches a string that <b>end with end</b>
- ^The end$   exact string match (starts and ends with <b>The end</b>)
- roar        matches any string that <b>has the text roar in it</b>

## Quantifiers- ^ + ? and {}
- abc*        matches a string that has <b>ab followed by zero or more c</b>
- abc+        matches a string that has <b>ab followed by one or more c</b>
- abc?        matches a string that has <b>ab followed by zero or one c</b>
- abc{2}      matches a string that has <b>ab followed by 2 c</b>
- abc{2, }    matches a string that has <b>ab followed by 2 or more c</b>
- abc{2,5}    matches a string that has <b>ab followed by 2 up to 5 c</b>
- a(bc)*      matches a string that has <b>a followed by zero or more copies of the sequence bc</b>
- a(bc){2,5}  matches a string that has <b>a followed by 2 up to 5 copies of the sequence bc</b>

## OR operator- | or []
- a(b|c)      matches a string that has <b>a followed by b or c</b>
- [bc]        same as previous, but without capturing b or c

## Character classes- \d\w\s and .
- \d          matches a <b>single character</b> that is a <b>digit</b>
- \w          matches a <b>word character</b>  
- \s          matches a <b>whitespace character</b> (uncludes tabs and line breaks)

## CSS Grid Reference https://css-tricks.com/snippets/css/complete-guide-grid/
## Responsive web design with css grid https://medium.com/samsung-internet-dev/common-responsive-layouts-with-css-grid-and-some-without-245a862f48df