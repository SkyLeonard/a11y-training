Until this point, the topics and tasks have been content-related and editable within a standard content management system. Today the checks and fixes get a little more complicated. The goal of the tasks is to discover gaps and to be able to create tasks to provide fixes. Those fixes may be design or programming-related and may require others to assist depending on your knowledge/access/systems.

Building from the previous days, now that someone is on your site, imagine if they can’t use a mouse (or *gasp* they _choose_ not to use a mouse). They navigate around the site using the keyboard only.

The primary principle today is to ensure every area of your website is accessible (a visitor can get to every page and piece of functionality) using only their keyboard. This may seem like something that should automatically be possible but you would be surprised by code behind the scenes that can cause:

1. Clickable elements to be skipped
2. Elements to be out of order
3. Elements selected without a visible indicator
4. Keyboard selection to be trapped in a section

## General principles of keyboard navigation

1. The “Tab” key moves forward between actionable items
2. The “Shift+Tab” moves backward between items
3. The “Enter” or “Space” key should activate the selected item
4. The left, right, up, and down arrow keys are used to interact with some elements (we won’t get into those details just yet here but those could be tabbed typed interfaces)
5. The “Esc” key should close a modal in addition to being able to click a “Close” type link
6. Each element with focus should have a visual indicator that it is selected (we will get into contrast later on, but for now as long as there is _some_ sort of visual difference that is enough)
7. Hidden elements should not be focusable
8. The order of actionable items should be logical (usually following the visual order of the page)

## Task

1. Load a page in a browser and click the “Tab” key to focus on the first element
2. Is it the element you expected?
3. Are you able to visually see where the focus is selected?
4. Tab to the next element and repeat steps 2-3 for each element on the page
5. When you reach the bottom of the page, hold the “Shift” key while clicking the “Tab” key and each element should be re-selected in reverse order until you return to the top of the page
6. Now that you’ve made it to all selectable items on the page, for each element, hit the “Enter” or “Space” button to activate the element, does it do (or go to) what you expect? If an element is interactive you may have to hit the arrow keys to move between elements (tabs or accordions). If an element provides an overlay, are you able to click the “Esc” key to get back to the element you were on before the overlay took over?
7. Repeat this for as many pages as you can in 20 minutes making notes or taking screenshots of all actionable elements that are not visible, not selectable, or are not dismissible with the “Esc” key.

## Example

![Animation of tabbing through a website to show each active link with a selected state that provides enough contrast to identify at a glance](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/tiuoDXid5b8NNx6jrqqPtL/email)

GIF of tabbing through a web page to show the visual indicator of each element

Notice in the example above that each element is visibly selected with enough prominence to where it stands out and there is no guessing which element is selected. In addition, there isn’t a single focus state style, the style is based on the element and surrounding context, if the background is light the focus ring is dark, if the background is dark the focus ring is light, and even on the social icons in the footer, they reverse color to provide enough visible focus.

These types of fixes require a front-end developer to make special considerations and may take several rounds of fixes, tests, and adjustments. This is an ongoing process as new elements are added to your site, be patient and work toward progress, not perfection.

## Extra benefits

- Being able to complete tasks without having to move your hands between different devices (keyboard, mouse, etc) increases the speed at which tasks can be completed
- In general, screen readers navigate web pages as we navigated above, selecting each element one-by-one in the tab order of the page. There are exceptions but the more usable a site is using the keyboard only, the more likely a screen reader will have a similar experience.

## Further resources

- [​Understanding SC 3.2.1:On Focus (Level A)​](https://www.w3.org/WAI/WCAG21/Understanding/on-focus.html)
- [​Understanding SC 2.4.7:Focus Visible (Level AA)​](https://www.w3.org/WAI/WCAG21/Understanding/focus-visible.html)