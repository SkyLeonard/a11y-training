When items are pressed on a website we want the site to react as quickly as possible to ensure the visitor isn’t waiting or questioning if the site is working. We also want to make sure the action we think the visitor is taking is actually the one they intend.

It may seem logical to hook the action to activation as soon as the visitor presses on an element. But what if that press-down was by mistake, is there a way to cancel it?

The best way to ensure a visitor’s press event is intended for a target is to activate the event on click-up. If the press and then depress events happen on the same element there is a higher likelihood it was a purposeful event.

In cases where this is not possible, having a confirmation dialog or an option to undo an action or movement of an item on the page could be a substitute for accidental actions.

## Example

![Animated gif of menu item clicks and click and moves to illustrate the link activation doesn't happen until click up](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/5QPLXP5fsQsLCJwFqHnz4t/email)

Example of menu item activation isn't activated until the press is released

The example above illustrates the activation of menu items only on the mouse-up event at the same location as the down event.

## Task

1. Start on your homepage
2. Using a mouse start clicking down on actionable elements, while pressed, move the cursor and then release the mouse. Ensure the item is not activated, or if there is activation, the action can be undone
3. Do this throughout the website in as many unique areas as possible
4. Move to a mobile device that uses touch events
5. Visit the homepage again and repeat the process. This time, press down with your finger and then move it before releasing

## Considerations

- There are exceptions with situations of games or other situations. For example, a card sorting activity where the visitor would be clicking and holding to pick up a card, move it, and then releasing to drop the card in a new spot. In situations like this, having the ability to undo an action would accomplish the same goal.
- Because there may be a few milliseconds between the down press and up event, the code in the background can still be pre-loading the page on the down event, but not actually activate the change of state until the up event happens.

## Further resources

- [​SC 2.5.2:Pointer Cancellation (Level A)​](https://www.w3.org/WAI/WCAG21/Understanding/pointer-cancellation)