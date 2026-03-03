If your website is sending emails, when was the last time you checked their accessibility?

Most of the same principles apply to emails as websites. The one issue most people encounter is the excessive use of tables in email since email clients do not support the recent advancements in CSS or are inconsistent with their support.

Often the visual layout is done with a bunch of nested tables. We briefly touched on tables and gave the principle that they are meant for tabular data. Email is kind of the except to this, they are often used for layouts, which can confuse screen readers.

When a screen reader starts interacting with an email with nested tables, it starts to go into table mode which will start reading the columns, rows, and headings instead of potentially the order of the content visually in the email.

## Example

![Screenshot of the accessible email results showing one error on the repetitive link labels](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/h7wx12A6WBfrpgimToRKzH?w=800&fit=max)

Email errors are grouped by headings, sections, links, images and document categories

## Task

1. Take your overall email template or the last few emails you have sent
2. View the full HTML source of the email from your email service provider (Mailchimp, Constant Contact, etc)
3. Paste the full HTML into [​https://www.accessible-email.org/​](https://www.accessible-email.org/)
4. Review any items flagged and correct

## Fixes

The most common issue, table structures used for layout, can be corrected by adding a role="presentation" attribute to the table elements, `<table role="presentation" …>`. This tells screen readers the table is only for presentation purposes and not to go into table mode when starting to read its contents. You will need to do this for each `<table>` element that is not tabular data.

## Further resources

- [​Accessibility email evaluation tool​](https://www.accessible-email.org/)
- [​W3C - Tables Tutorial​](https://www.w3.org/WAI/tutorials/tables/)
- [​How screen readers navigate data tables​](https://tink.uk/how-screen-readers-navigate-data-tables/)