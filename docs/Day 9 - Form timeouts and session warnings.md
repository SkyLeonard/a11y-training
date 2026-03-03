If you have any forms or processes that are time sensitive are you giving your users a heads up that their time is about to expire? Or if there is a complicated form, is there a way to save progress? Or perhaps an auto-save process and let the user know?

You may not have any forms that meet this criteria but it is a good idea to continue to review forms from yesterday with timing in consideration. If the user fills out a form but there is an error, if they leave their device for an hour and then come back to correct and submit the form, does it still work? Do they have to re-enter any information or does it error? If there are errors, are they clear?

If the user is logged in, does it automatically log them out after a certain amount of time? Does it give them a warning and a chance to cancel? If they were filling out a form when they where being logged out, is the form information preserved?

## Example

![Screenshot of a modal warning the user their session is about to expire with a countdown and buttons to continue or log out](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/iVpEdViVzDsZhgZqver1WJ/email)

Screenshot of an alert model warning before automatically logging out

In the example above, the notice warns the user about the time left to complete their task. This appears after 20 minutes of inactivity, if they choose to stay on the website, their session is restarted for another 20-minute timeout. If they choose to leave, if possible, save their progress so when they do return they do not have to recreate it.

## Task

1. Find a page on your website that has a form
2. Start filling out the form and leave it for 10 minutes, (or longer)
3. Submit the form, does it submit successfully? If not, is the error clear? Is the data from the form preserved?

## Considerations

Even if you don’t have forms with timeouts, forms with textarea elements may require someone to type in more than a few sentences of content. Consider using local storage to save their information in case something happens and they have to leave the page. When they return later it would improve their experience to have that information automatically restored so they don’t have to re-type it in.

## Further resources

- [​Understanding SC 2.2.6:Timeouts (Level AAA)​](https://www.w3.org/WAI/WCAG21/Understanding/timeouts.html)