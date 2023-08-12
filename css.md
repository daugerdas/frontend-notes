# Cascading Style Sheets (CSS)

Cascading Style Sheets (CSS) is a stylesheet language used to describe the presentation of a document written in HTML or XML.

## Box model

Everything in CSS has a box around it, and understanding these boxes is key to being able to create layouts with CSS, or to align items with other items.

Parts of a box:

- Content box: The area where your content is displayed, which can be sized using properties like width and height.
- Padding box: The padding sits around the content as white space; its size can be controlled using padding and related properties.
- Border box: The border box wraps the content and any padding. Its size and style can be controlled using border and related properties.
- Margin box: The margin is the outermost layer, wrapping the content, padding and border as whitespace between this box and other elements. Its size can be controlled using margin and related properties.

In the alternative CSS box model any width is the width of the visible box on the page, therefore the content area width is that width minus the width for the padding and border. By default, browsers use the standard box model. If you want to turn on the alternative model for an element you do so by setting `box-sizing: border-box` on it.

CSSOM (CSS Object Model is a map of all CSS selectors and relevant properties for each selector in the form of a tree, with a root node, sibling, descendant, child, and other relationship. CSS takes care of default formatting of documents through the concept of user agent style sheets, a cornerstone of the cascade.

## CSS reset

CSS reset (reset stylesheet) is a collection of CSS rules used to clear the formatting of HTML elements. A reset style sheet is only used to reset basic formatting. In contrast, a CSS framework, which typically include pre-made style definitions for often-needed UI elements or a grid system, is used to speed up the development process of a website. However, a CSS reset is often part of a CSS framework.

## Flexbox

Flexbox is the commonly-used name for the CSS Flexible Box Layout Module, a layout model for displaying items in a single dimension — as a row or as a column.

Properties: `align-content`,
`align-items`,
`align-self`,
`flex`,
`flex-basis`,
`flex-direction`,
`flex-flow`,
`flex-grow`,
`flex-shrink`,
`flex-wrap`,
`justify-content`,
`order`.

## Positioning

Positioning allows you to take elements out of the normal document layout flow, and make them behave differently; for example sitting on top of one another, or always remaining in the same place inside the browser viewport. This article explains the different position values, and how to use them.

`Position` values: `static`, `relative`, `absolute`, `fixed`.

## Specificity

Specificity is the means by which browsers decide which CSS property values are the most relevant to an element and, therefore, will be applied.

Selector type: type selectors, class selectors and ID selectors. Universal selectors (`*`), combinators (`+`, `>`, `~`, ` `, `||`) and negation pseudo-class (`:not()`) have no effect on specificity.

