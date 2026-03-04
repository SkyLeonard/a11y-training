Tables are for tabular data. What is the best way to identify tabular data?

1. Think about the information in the table, would it make sense to share it in a spreadsheet?
2. Are there rows or columns with labels to identify the information in the cells?
3. Would it feel natural to read the row/column label before reading each value in the cell?

We’ve come a long way since table layouts (except for emails in some cases) but you never know when you’ll come across a content editor who has positioned content on a page in a table.

Often it is due to unintentionally trying to get content to display in a specific way within a content management system. In these cases, the constraints of the system are not encouraging accessible behavior. If you come across content that has been formatted this way it isn’t the time to vilify the behavior, it’s a great opportunity to educate content editors and to question what systems could be put in place to prevent this in the future. We want the path of least resistance to be creating content with the widest range of access possible.

## Example

![Screenshot of a web page with the inspector open with an arrow pointing from the table code to a visible table on the page](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/dqm96iNU4U1ohQuawiZf2q/email)

Example use of a table for visual display

The example above doesn’t fail the automated accessibility test, but the content is only placed in a table to display it in two columns. With CSS we can now display a list of items in two columns without a screen reader to go into table reading mode.

## Task

1. Search for any `<table>` elements on your site
2. Evaluate each table first, is the information something you would copy/paste into a spreadsheet to share?
3. If the table content is appropriate, are the headings in the appropriate spot (rows, columns, or both) and marked up as `<thead>` and `<th>` elements in HTML?
4. Does the table need a `<caption>` or `<summary>` element to describe the contents?

## Considerations

- Complex tables with header rows or columns that span multiple cells will be combined when reading the value of each cell as long as the “scope” attribute is applied.
- If you have no choice but to use tables for some visual display but do not want a screen reader to use the table mode to navigate the cells, add role=”presentation” to the table element, for example, `<table role="presentation" …>`.

## Further resources

- [​H51: Using table markup to present tabular information​](https://www.w3.org/WAI/WCAG22/Techniques/html/H51)
- [​WebAIM: Creating Accessible Tables​](https://webaim.org/techniques/tables/data)