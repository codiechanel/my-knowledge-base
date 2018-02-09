As of March 2017, most browsers shipped native, unprefixed support for CSS Grid: Chrome \(including on Android\), Firefox, Safari \(including on iOS\), and Opera. Internet Explorer 10 and 11 on the other hand support it, but it's an old implementation with an outdated syntax. The time to build with grid is now!

CSS-Grid is now newer and better grid system than flexbox, but they can be used together. Please see the link:

[https://css-tricks.com/snippets/css/complete-guide-grid/](https://css-tricks.com/snippets/css/complete-guide-grid/)

And it's now supported by most browsers, and it's matter of time it will become the standard way of defining the grid layout.

Would Material UI implement CSS Grid as well for incoming updates?

@oliviertassinari CSS grid is the "right" way to implement a grid system, with flexbox being more appropriate for component-level layout. I've been around long enough to remember pre-table layout challenges, and the abuse of table for layout,so it is exciting that we finally have an appropriate solution \(hard to believe it's taken this long!\).

