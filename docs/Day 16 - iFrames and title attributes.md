Gone are the days of developing websites in frames as a primary source of content within a site. But frames are still everywhere on the web, they help inject content (Google Tag Manager) and multimedia content like videos or podcasts.

A screen reader or assistive device doesn’t know the difference between a container with content in it and one to inject functionality. To ensure the content of an iframe is correctly identified it should have a “title” attribute on the iframe element.

Unfortunately, some of the most common embedded media sites do not automatically include a title attribute in their default embed code. This responsibility falls to the person embedding the code to provide a title that makes sense in the context of the page.

## Example

![Screenshot of a web page with the Soundcloud embed and axe devtools open showing an error for the missing title attribute](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/qEosbqDsq4HaKsgQNzH9S6/email)

Screenshot of the axe DevTools detecting the Soundcloud iframe missing a title attribute

The example above is the default Soundcloud embed of an audio player. The iframe itself fails the automated test because it doesn’t have a title attribute.

## Task

1. Search your website for any iframe elements
2. Either inspect each element or run the axe DevTools on each page to check if the iframes pass the test
3. Read each title attribute to ensure it makes sense in the context of the page

## Considerations

- Without a title attribute, a screen reader may read “frame”, the filename, or the full URL of the frame
- Like headings, links, and regions, screen readers can pull up a list of frames on the page, ensure the tile also makes sense outside the context of the page content
- Ensure the frame titles are unique, multiple of the same titles can be confusing to a visitor
- If an iframe is only used to inject additional code or isn’t relevant to the end-user (example: Google Tag Manager), hide it from a user by adding `aria-hidden="true"` to the `<iframe>` tag

## Further resources

- [​Technique H64:Using the title attribute of the iframe element​](https://www.w3.org/WAI/WCAG21/Techniques/html/H64)