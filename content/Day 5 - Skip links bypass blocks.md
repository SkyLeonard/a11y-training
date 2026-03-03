You may have noticed in the GIF from yesterday’s email, or on your own site, a few of the first tab stops were to invisible links that became visible when tabbing. If so, they were likely “skip links” to allow a keyboard user to jump to specific spots on the page without having to tab through common items on every page.

These skip links help a user who is visiting multiple pages on your website to jump past the common elements such as the header or main navigation to get directly to the content without having to hit “Tab” dozens of times for each page visit. It is the keyboard version of having visual consistency between each page so someone doesn’t have to re-learn how to use each page on the website.

## Example

![Animation example of tabbing to skip links and selecting each to demonatrate how the focus of the page is moved around](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/iMf6Bc9rBjRE2RwcSfw3ro/email)

GIF of a bypass block in action moving between navigation and main content

## Task

1. Load a page in a browser and click the “Tab” key to focus on the first element
2. If it is not a hidden “Skip” link, at least jump to the main content area, review the resources below to get the technical details on how to implement the links

## Allowing focus on container elements

There are some technical considerations that need to be made when adding these links:

1. They need to be the first focusable items in the HTML, usually directly after the <body> tag
2. If you were to implement any, start with jumping to the main content area
3. If you are anchoring down to an element that is not an anchor tag <a>, add a tabindex=”-1” to the element to allow it to be selectable, for example: <main id="content" tabindex="-1">

## Further resources

- [​Understanding SC 2.4.1:Bypass Blocks (Level A)​](https://www.w3.org/WAI/WCAG21/Understanding/bypass-blocks.html)
- [​The A11y project - Use skip navigation links​](https://www.a11yproject.com/posts/skip-nav-links/)
- [​WebAIM - Skip Navigation Links​](https://webaim.org/techniques/skipnav/)