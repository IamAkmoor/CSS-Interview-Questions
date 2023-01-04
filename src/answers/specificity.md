## What is Specificity?

If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style declaration will be applied to that HTML element.

Think of specificity as a score/rank that determines which style declaration is ultimately applied to an element.

#### Specificity Hierarchy

Every CSS selector has its place in the specificity hierarchy.

There are four categories which define the specificity level of a selector:

    Inline styles - Example: &lt;h1 style=&quot;color: pink;&quot;&gt;
    IDs - Example: #navbar
    Classes, pseudo-classes, attribute selectors - Example: .test, :hover, [href]
    Elements and pseudo-elements - Example: h1, :before

#### How to Calculate Specificity?

Memorize how to calculate specificity!

Start at 0, add 100 for each ID value, add 10 for each class value (or pseudo-class or attribute selector), add 1 for each element selector or pseudo-element.

__Note__: Inline style gets a specificity value of 1000, and is always given the highest priority!

__Note 2__: There is one exception to this rule: if you use the !important rule, it will even override inline styles!
