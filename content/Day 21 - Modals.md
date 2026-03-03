We're not talking about the old-school pop-ups that open in a new chromeless window or try to hide behind your browser in years past, we're talking about any type of modal or dialog that may present user information on your site.

Modals are separate than the main content of the document and are identified by role="dialog". There are two considerations when using modals, the first is a proper label, and the second is keyboard focus.

Labeling the modal can be accomplished by pointing the aria-labelledby attribute to the ID of the H1 or text that would represent the title inside the modal. If there is a longer description, the aria-describedby attribute should be used to reference the longer description.

Javascript is required for effective focus management, this requires:

- A modal should have at least one focusable item, which at least closes the modal.
- When opened, the focus should be moved to the first focusable element within the modal.
- While open, the keyboard focus should remain within the modal only and should not escape to the rest of the page contents until the modal is closed.
- When the modal is closed, the focus should be returned back to where it was before the modal opened.

Another type of modal is the ‘toast message’ that may appear in the corner of a website and alert the visitor of a status message. These are considered non-modal dialogs and in the further resources below, a blog post goes into further detail about non-modal considerations.

## Example

[

![Screenshot of a Loom video which uses Safari and VoiceOver to walk thruogh a modal example](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/qkeeBne3gjzXKMP1yMQiyw/email)](https://www.loom.com/share/2a51463ae97a49f3bbab7010564908ee)

Video of a modal in action using Safari and VoiceOver screen reader

The example video shows a modal that meets all the criteria outlined for the announcement of it, keyboard trapped and then focus returned to the previous location after closing.

## Task

1. Find a page or area of your website that includes a modal
2. First using your keyboard only, activate the modal
3. Determine where the focus has moved, ensure it is on the first focusable element in the modal
4. Interact with the modal, use the Close/OK/Cancel button, and try the Escape key to ensure the modal closes in each case
5. Ensure the focus was returned to the page where it was before the modal opened
6. Now repeat steps 2-5 using a screen reader

## Considerations

- When closing, the focus should be restored back to the element the last focused element, typically the item that activated the dialog.
- The Escape key should close the modal in addition to any other cancel or close button
- Although keyboard users may be trapped in a modal until they escape, screen readers have a virtual cursor that may be able to navigate with elements behind the modal.

## Further resources

- [​Understanding SC 2.1.2:No Keyboard Trap (Level A)​](https://www.w3.org/WAI/WCAG21/Understanding/no-keyboard-trap.html)
- [​MDN: ARIA: dialog role​](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/dialog_role)
- [​Designing Toast Messages for Accessibility​](https://scribe.rip/designing-toast-messages-for-accessibility-fb610ac364be)