# Assignment 5.2 - CSS Selectors Practice

## Selectors Used

- Universal selector (`*`): applies to every element on the page. I used it to reset margin and padding and to set box-sizing.
- Element selector (`body`, `p`): styles every element of that tag. I used it for the page font and paragraph spacing.
- Grouping selector (`h1, h2` and `header, footer`): applies one rule to several selectors at once, which avoids repeating code.
- Class selector (`.card`): styles every element that has class="card". I used it for all the cards.
- ID selector (`#special`): styles only the one element with that ID. I used it to give one card a different background and border.

## Cascade and Specificity

I wrote two conflicting rules for the same paragraph:

- `.note` sets the color to blue.
- `#conflict` sets the color to red.

The paragraph has both the class `note` and the ID `conflict`. The text shows in red, because an ID selector has higher specificity than a class selector. When rules have the same specificity, the rule written later in the file wins.