When content changes visually on a page it also needs to be announced to non-visual visitors.

Examples could be successful form submissions done in JavaScript while the page does not refresh. It could be the result of a process that is running in the background (an export is ready to download or a new notification comes in). Or something added to a shopping cart.

Sighted users may notice the alert show up on the screen or content update but someone who is using a screen reader doesn’t automatically get notified of new content being added or changed on a page.

This dynamic content can be announced with a little bit of planning and JavaScript. ARIA live regions allow for these content updates to be announced.

The element must exist first on the page: <div role="region" aria-live="polite">...</div>

As soon as content is added to the live region, it is read by the screen reader at the next pause.

## Example

[

![Screenshot of a video example of an ARIA live region in action](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/6ZiGp5ARywjKshoGBbpFL1/email)](https://www.loom.com/share/2d20df5775de4a49aeafe67beb657251)

ARIA live regions in action using VoiceOver

The example above is linked to below, this is a great opportunity to try out your screen reader skills and experience dynamic information being announced.

## Task

1. If your website has any interactive elements that change the state of the page after a user interaction or after a certain amount of time, visit one of the pages.
2. Start the screen reader of your choice
3. Interact with the page to ensure the items that trigger that content change are detected
4. Trigger an event that updates content on the page
5. Listen for those updates to be announced by the screen reader
6. If they are not, adjust the code on the website to ensure an aria-live region exists and is being updated correctly

## Considerations

- In the code above, the aria-live="polite" tells the screen reader to announce any updates at the next pause. If an alert is necessary to update the visitor immediately, use the role="alert" on the element, which assumes aria-live="assertive" and will announce any updated content immediately, interrupting any current content the screen reader is reading. Use this approach sparingly for certain alert situations.

## Further resources

- [​Understanding SC 4.1.3: Status Messages (Level AA)​](https://www.w3.org/WAI/WCAG21/Understanding/status-messages.html)
- [​ARIA22: Using role=status to present status messages​](https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA22)
- [​ARIA19: Using ARIA role=alert or Live Regions to Identify Errors​](https://www.w3.org/WAI/WCAG21/Techniques/aria/ARIA19)
- [​MDN: ARIA live regions​](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/ARIA_Live_Regions)
- [​W3C: Alert Example​](https://www.w3.org/WAI/ARIA/apg/patterns/alert/examples/alert/)