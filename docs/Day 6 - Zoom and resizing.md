Being able to increase the size of a site is paramount for anyone who has trouble reading text at the originally designed size.

There are various reasons, temporarily or permanently, that someone may want to zoom in or out to scale images and text. The web is flexible by default and ensuring your website can adapt to a visitor’s vision requirements will ensure you are not frustrating or losing visitors.

## Example

![Animation of a website being zoomed in 400% and tabbing through the elements to ensure the menu and accordions work](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/sz23HubfLke8aaDisbFMzt?w=800&fit=max)

Animation of zooming a web page and interacting with the menu and accordions

You will notice a few things in the example above that work well, the menu works as intended and a visitor can scroll through it, the accordions open and close without issue. Typically, regular static content works as expected, but when you have interactive elements that require a specific amount of space (modals, infographics, animations), that is when spacing may have unintended consequences.

A few things about the example above are not technically wrong but could make the user experience better:

1. The header scrolls with the visitor down the page, when it is zoomed in 400%, the padding is so large that it takes up almost half of the screen real estate, which leaves only a small area to view the content of the site.
2. Because of this header overlay, when an accordion is opened, the code scrolls the visitor to the top of that specific item, but it isn’t taking into account the zoomed-in header, so the content is being covered which forces the visitor to scroll up or down to start reading.

## Task

1. Load a page on your website, while holding the Command/CTRL key and clicking the + (plus) key on the keyboard
2. Zoom in to 400%
3. Check to ensure everything is still visible (nothing is overflowing the screen)
4. Ensure you’re able to use the site fully (try to click or tab to all elements and use them)
5. Visit the same page on a mobile device and pinch to zoom to the same 400%
6. Try to use the site again to use each feature/link/form

## Considerations

- Zooming in at some point may trigger the smaller screen views, this is expected
- When viewing on a mobile device the website should work in landscape and portrait orientations

## Most common fix

If your site is not zooming in at all, check the `<head>` of your page to ensure the meta viewport tag allows zooming: `<meta name="viewport" content="width=device-width, initial-scale=1">`

If you see “user-scalable=no” in the content attribute, remove it and try the task again.

## Further resources

- [​Understanding SC 1.4.4:Resize Text (Level AA)​](https://www.w3.org/WAI/WCAG21/Understanding/resize-text)
- [​Understanding SC 1.4.10:Reflow (Level AA)​](https://www.w3.org/WAI/WCAG21/Understanding/reflow.html)