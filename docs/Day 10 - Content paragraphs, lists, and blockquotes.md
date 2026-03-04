Let's focus on the structure of the main content area (where a visitor would jump to after clicking the “Skip to main content” link). We previously investigated the headings on the page, now let's extend our review to the paragraphs, lists, and quotes that make up the bulk of the page content.

The main principle when looking at the content structure is to start with sections of the page broken up by headings that describe the content below it. If there are sub-sections within that heading, additional headings of the next level are used to denote the relationship between the interior sections and the above heading.

Below each heading may be a combination of paragraphs, lists, blockquotes, code snippets, and a handful of other [​block-level elements​](https://developer.mozilla.org/en-US/docs/Web/HTML/Element#text_content). Let’s spend a few minutes ensuring the correct types of elements are being used throughout the main content area of the page.

The goal today is to strip away all the visual style of your pages and get down to only the structure of the content. Think about it purely as a written document that can only communicate the intent of the content by the HTML elements. A paragraph of text, a list of items, a quote with attribution, description lists, etc.

You may have some table elements in your content, we won’t dive into table structure yet, but the one thing you will want to ensure is you’re using a table for tabular data only. A quick test to confirm this is to copy/paste the table into a spreadsheet, without any of the surrounding text, would the table make sense on its own with the rows/columns/headings? If not, it should probably be converted to another HTML element.

## Example

![Screenshot of a web page with all style removed and images turned off to see the pure document structure based on the HTML elements used](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/2bWTX9adiDjTfnL2NDYeq3/email)

Screenshot of web page with all styles removed to view only the document structure

You may notice in the example it is hard to see the entire page overview. You may have to CTRL/Command + -(minus) to zoom out to see the entire page structure at a glance. You may also have to scroll past standard template items like menus or icons at the top of the page.

## Task

1. Open up the homepage, or any page on your website
2. Open the Web Developer browser extension, under CSS, and choose “Disable All Styles”.
3. The page will now be completely linear with the default browser style applied to all HTML elements
4. You may have to choose the option to "Disable Images" (or replace them with their alt text) in the extension since they may now span the entire width of your browser
5. Look at the content structure (now separated from the layout) and ensure it flows from section to section down the page. The heading levels, paragraphs, lists, and quotes should be read from top to bottom in a narrative structure.

## Considerations

- There are three major types of lists, ensure you’re using the right list type in each case. Unordered lists are for a related set of items but do not require each item to have a specific sequence (ex: menu items). Ordered lists are for a related set of items that have a specific sequence (ex: steps to enroll). Description lists are lists where each item contains a term and a description.
- Website navigation is usually structured as nested unordered lists

## Tools

- ​[​Web Developer Firefox browser extension​](https://preview.convertkit-mail2.com/click/dpheh0hzhm/aHR0cHM6Ly9hZGRvbnMubW96aWxsYS5vcmcvZW4tVVMvZmlyZWZveC9hZGRvbi93ZWItZGV2ZWxvcGVyLw==) - [​Chrome version​](https://preview.convertkit-mail2.com/click/dpheh0hzhm/aHR0cHM6Ly9jaHJvbWUuZ29vZ2xlLmNvbS93ZWJzdG9yZS9kZXRhaWwvd2ViLWRldmVsb3Blci9iZmJhbWVuZWlva2tnYmRtaWVraGpubWZrY25sZGhobQ==)

## Further resources

- [​WCAG Content Structure​](https://www.w3.org/WAI/tutorials/page-structure/content/)
- [​Technique H48:Using ol, ul and dl for lists or groups of links​](https://www.w3.org/WAI/WCAG22/Techniques/html/H48)
- [​H42: Using h1-h6 to identify headings​](https://www.w3.org/WAI/WCAG22/Techniques/html/H42)