Like headings, a visitor who cannot visually see the layout of a page uses the underlying structure to learn about the content as an overview and to jump to specific regions. You can control the labels and what is contained in these areas using landmarks.

Many HTML5 elements are landmarks built-in which enables accessibility support out of the box. These elements are `<header>`, `<nav>`, `<main>`, `<aside>`, `<section>`, and `<footer>`.

You may have multiple of these elements on a page, for example, a site and breadcrumbs navigation. You can label each instance with `aria-labelledby`, if the label is visible on the page, or provide your own label with `aria-label` on the landmark element.

The landmarks pair well with the skip links/bypass blocks on your page. Pairing the bypass blocks with regions emphasizes the importance of structured markup.

## Example

![Visual overview of using the Landmarks browser extension to highlight each landmark and all at once](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/76nj1U93Mti6jZX2wp12Mq/email)

Overview of highlighting each landmark individually and then all at the same time

The example above shows an overview of the regions available to the visitor. The “Show all landmarks” option highlights all at the same time and gives a visual overview to ensure all page content is contained within a landmark.

## Task

1. Install the Landmarks browser extension below
2. Visit the homepage of your website
3. Open the Landmarks extension to see an overview of the landmarks available
4. Make sure the landmarks are appropriate for the content they contain
5. If there are missing landmarks, add HTML elements to contain that content
6. Review each landmark label, are they descriptive enough?
7. Move to another page and repeat this process

## Considerations

- When possible, use native HTML elements instead of relying on ARIA attributes on `<div>` elements
- Ideally, all content on a page would be covered in a region
- Often the regions are taken care of in the overall template of the site, but each page may contain `<aside>` or `<section>` elements within the `<main>` content. These two elements are often confused with each other. “aside” is content related to the main content, and “section” is not related to the main content.

## Tools

- [​Landmarks browser extension​](https://matatk.agrip.org.uk/landmarks/)

## Further resources

- [​Technique ARIA11:Using ARIA landmarks to identify regions of a page​](https://www.w3.org/WAI/WCAG22/Techniques/aria/ARIA11)
- [​W3C - ARIA Landmarks Example​](https://www.w3.org/WAI/ARIA/apg/patterns/landmarks/examples/main.html)