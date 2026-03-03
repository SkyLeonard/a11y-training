The order of the content in the source code should be the same as the visual presentation. This may feel like a no-brainer, but if a visitor is tabbing through the focusable elements it should not jump around the page.

For example, the logo followed by the navigation visually on the page, in the HTML DOM, should follow each other. The tabindex has two goals, to make an element focusable and to place an element in the tab order. If you are changing the tabindex, it is a signal that you should investigate the DOM order of the page elements.

When there are columns or aside content next to a main area, this is where your insight of which items should be focused first, the content in the main area or the aside? This is a judgment call based on the content and then to ensure the DOM matches the ideal order.

## Example

![Screenshot of a web page after running the taba11y plugin which visually draws lines between tabbable elements and assigns each a number in the overall order](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/tmdvM988gjxJ6tdpG35U1S)

Screenshot after running the taba11y plugin to visually show the tab order of elements on a web page

In the example above, the tabindex shows what looks like a logical order but you may be surprised by some elements, the live chat here is one of those. It is visually stuck to the bottom right corner of the screen and it is last in the tab order. This may be ideal, but depending on your context, you may want it directly after the main content or after the main menu.

## Task

1. Visit the homepage of your website
2. Scroll through the page at each viewport size and take note of the order of elements
3. Run the taba11y browser extension to visually view the tab order of the page
4. View the source of the page
5. Determine if the DOM order matches the visual order
6. If not, using CSS techniques, could the DOM order be moved without changing the visual layout?
7. Repeat these steps on each unique layout on your website

## Considerations

- CSS updates like Grid can make it easy to move visual elements around the screen at different viewpoints. This can help ensure content is in the right order visually and encourages a DOM order that makes the most sense to a user and search engine.
- Third-party scripts that inject functionality into the page may not give you the option to inject the content it produces into a specific position on the page. These types of scripts may require additional development to move them into the correct place for your visitors.

## Further resources

- [​SC 1.3.2:Meaningful Sequence (Level A)​](https://www.w3.org/WAI/WCAG21/Understanding/meaningful-sequence)
- [​Browser extension - taba11y - Chrome webstore​](https://chrome.google.com/webstore/detail/taba11y/aocppmckdocdjkphmofnklcjhdidgmga)