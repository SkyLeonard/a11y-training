Ensuring the visual elements of your page are clickable is just as important as ensuring they have enough contrast and are in a consistent place. The minimum amount of space required for an element to be clickable is 24x24 pixels.

This ensures the elements are touchable and clickable in several scenarios. This could include various screen sizes, zoom, or difficulty with motor movement. It ensures items are not accidentally clicked when adjacent to other elements.

## Example

![Two screenshots next to each other to compare the hamburger icon in a website, the icon itself is too small, but the clickable area around it is expanded to meet the minimum size requirements](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/rsDLGDpEh7U31f3bSPukB5/email)

Using CSS, the clickable areas of elements can be expanded.

In the example above, it shows the icon itself isn’t large enough to meet the 24x24 px size requirements. To ensure the target size is large enough, the clickable space in the style is expanded to include space around the icon.

## Task

1. Open the homepage of your website
2. Open the inspector and select the axe DevTools
3. Run a test on the entire page
4. Read through the results to ensure there are no target size errors
5. Change the window size or use the device toolbar to simulate a smaller screen
6. Run the test again and look for results
7. If there are any icons or text that appear too small, inspect those elements to view their visible size including any padding

## Considerations

There are a few exceptions to consider where targets smaller than 24x24 may be acceptable: 

- If targets are positioned so that a 24 pixel diameter circle is centered on the bounding box of each, the circles do not intersect another target or the circle for another undersized target
- If the same function can be achieved by a different conforming element on the page
- The target is in a sentence or its size is otherwise constrained by the line-height of non-target text
- The user has control over the target size of the element
- The target is legally mandated


## Browser extensions

- [​axe DevTools browser extension​](https://www.deque.com/axe/browser-extensions/)
- [Siteimprove browser extension​](https://www.siteimprove.com/why-siteimprove/integrations/browser-extensions/) (Filter to A, AA and ARIA conformance)

## Further resources

- [​Understanding SC 2.5.8:Target Size (Minimum) (Level AA)​](https://www.w3.org/WAI/WCAG22/Understanding/target-size-minimum.html)
- [​Understanding SC 2.5.5:Target Size (Level AAA)​](https://www.w3.org/WAI/WCAG22/Understanding/target-size-enhanced.html)
- [​Axe DevTools browser extension​](https://www.deque.com/axe/devtools/)
