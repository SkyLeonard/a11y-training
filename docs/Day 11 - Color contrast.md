After image alt text, color contrast is the next thing most people think about for accessibility. Several automated scanning tools check for contrast but like everything else, some nuances require a human to review.

The most common considerations when it comes to checking the color contrast on a page:

**Text on the solid background color**

This is the most common case and automated checkers are the best to handle, checking these common areas manually would be time-consuming.

![Screenshot of a page header that says Section header, styleguide](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/x731N6aYfW8hrpPqMmEMPU/email)

**Text on images**

Anytime text is embedded into an image it requires a human to review the parts of the text that have a potentially low contrast with the background image. My favorite way to do this is the Colour Contrast Analyser (CCA) tool listed below. There are dozens of tools that can do this, but I like any app that has an eyedropper to select any pixel, regardless of where it is on the screen.

![Screenshot of an illustrated ticket stub with the words Student and emploee discounts on it](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/bkZGEicMd8RoKR6BoDrXee/email)

**Text on gradients**

Gradient backgrounds give automated checkers trouble. The ideal situation is to check the edge of the text where the gradient starts behind it.

![Screenshot of text on a gradient that shows the gradient starts above the text to ensure there is enough contrast](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/9FtfRUYHXVJQ8uucfhkS5W/email)

**Buttons/icons on the background**

The same principles apply to icons, there must be a 4.5:1 contrast ratio.

![Screenshot of the color contrast for icons on a green background showing it passes the test with a 5.7:1 ratio](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/eJL6BrXxXhP79Kv7r37jtc/email)

## Example

![Screenshot of Warriors Welcome You with a contrast checker next to it and arrows pointing to the spots to check contrast](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/gjWtvW7AKfGV3ERovPFRu2/email)

Screenshot of a contrast checker with arrows pointing to the parts of the image with the least amount of contrast

The above example is something that requires manual checking. It not only is text on a gradient but is also an SVG overlaid on a gradient. The automated checkers are often confused by this combination and either fail it automatically or flag it for manual review.

## Task

1. Open the homepage of your website
2. Right-click and “Inspect” the page to get the inspector open and navigate to the axe DevTools from the previous week
3. Run an automated accessibility check on the entire page
4. Review for any automated contrast errors and correct
5. Close the inspector and scroll down the page in a browser looking for any text on images, any text on gradients, or any interface UI elements like icons
6. For each of the items found, use a color contrast checker from the tools below to find eye drop the spot in the foreground and background where the colors likely have the least contrast
7. If the contrast fails based on the size of the text/icon, adjust it as needed

## Considerations

- If you are planning to have white text on top of an image background my favorite way to test the extremes of contrast are to upload the same color background image as the text. This forces you to either add an alpha layer on the image to darken it or to provide a gradient that covers behind the text to allow for enough contrast.
- Because responsive websites allow elements and background images/gradients to move around on the screen, it is also important to resize the browser window to check all scenarios based on various viewport sizes.

## Tools

- [​WebAIM: Contrast Checker​](https://webaim.org/resources/contrastchecker/)
- [​Colour Contrast Analyzer (CCA)​](https://www.tpgi.com/color-contrast-checker/)
- [​Accessible Perceptual Contrast Algorithm (APCA) contrast checker​](https://www.color-contrast.dev/?txtColor=FEF3C7&bgColor=059669)

## Further resources

- [​Understanding SC 1.4.3:Contrast (Minimum) (Level AA)​](https://www.w3.org/WAI/WCAG22/Understanding/contrast-minimum.html)