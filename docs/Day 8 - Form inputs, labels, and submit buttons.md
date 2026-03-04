Hope you enjoyed the start of the month last week with the fundamentals. Even if you were able to spend a few minutes on your website investigating and changing even a handful of things, those changes will have long-lasting effects and make your website better for everyone.

This week we’re going deeper into more technical concepts which may take more time to make changes. Try not to get discouraged if you’re not able to fix everything by yourself right away, this is a marathon and not a sprint. Knowing where to put time and attention will help you prioritize the rest of the year.

Today you’ll need to review any forms on your site. You could have one, you could have hundreds 😬.

Search your website for any pages with form elements, if they are native elements, they are the easiest to detect and edit. If they are embedded forms from third-party sites, it is going to be much harder to make changes since you don’t have direct control. If you do detect changes needed on third-party forms, I encourage you to start a conversation with the company to ask if they have tested their forms for accessibility. This may not result in an immediate fix, but it signals to them there are users paying attention to these details.

## Example

![Screenshot of a form with the axe DevTools window open showing an error with the form](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/udxdkojHaPsRSQZYNqKe1R/email)

Screenshot of a form with the axe DevTools window open showing an error with the form

You will notice from the bottom panel in the example, that the errors are summarized. Each error contains the exact element, an explanation, and resources to assist with a possible fix.

## Task

1. Open any page with a form element on it
2. Use the Axe browser extension to scan the page looking for form issues
3. Inspect and resolve any form-related issues
4. Submit the form to try and get it into an error state (required fields or validation issues)
5. Repeat steps 2 and 3 with the errors displayed
6. If you have a widget inside your form, calendar date picker, auto-complete, multiple selection, etc. Try to use the widget with your keyboard only

## Considerations

There are hundreds of details that could affect the basic functionality of forms and some small details that make things more usable for everyone:

- All form inputs should have labels associated with them
- All required fields ideally should have two ways of identifying their requirement, both in the label itself, for example, “Fields with asterisks (*) are required.” and in the HTML, the “required” attribute on the input field
- After submitting, errors should be summarized at the top of the form
- On error, each field should have a related (in proximity and HTML association) error message
- On error, the focus should be moved to the first field with an error
- Forms that auto-submit based on value changes have several additional considerations
- Forms should not force a user to input repetative information and provide auto-fill functiontality when possible
- Cognitive puzzles and memorization are not required authentication steps

## Tools

- [​axe DevTools browser extension​](https://www.deque.com/axe/browser-extensions/)
- [Siteimprove browser extension​](https://www.siteimprove.com/why-siteimprove/integrations/browser-extensions/)

## Further resources

- [​W3C - Forms Tutorial​](https://www.w3.org/WAI/tutorials/forms/)
- [​Techniques for WCAG 2.0 submission form​](https://www.w3.org/WAI/GL/WCAG20/TECHS-SUBMIT/)
