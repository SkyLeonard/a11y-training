When most people think about web accessibility they often equate it to providing alternate text on images. The topic of alternate text could fill an entire email course or book. Today’s topic is only meant to be a prompt to get you thinking and discovering opportunities.

You can tackle the task in a few different ways. The first would be to look for any image without alt text and tackle those first. They are the ones causing the largest issue for someone who isn’t able to view images.

The second approach is to read through the alt text of all the images on a page in isolation. Comparing the image with the image itself without thinking of the surrounding context.

The third approach is to read the alt text of each image in the context of the headings, paragraphs, and links around the image to ensure the text makes sense.

Choose the approach that feels right for you. The approach I take is to close my eyes and read the text out loud. This helps me realize if there are details about the image that need to be added or removed from the alt text.

## Example

![Screenshot of Chrome with the Web Developer exttension installed with the display alt attribute optione turned on with an arrow showing the alt text displayed on an image](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/sPURsRB2Xc8SXa1ihoa6FV/email)

Screenshot of Chrome with the alt text of each image displayed on screen

## Task

1. Install the Web Developer browser extension (links below)
2. Open the homepage of your website
3. Open the extension and click one of the following. Images -> Display Alt Attributes or Outline Images With Empty Alt Attributes or Outline Images Without Alt Attributes
4. Scroll through the page and determine if any images need to be described by alternate text
5. Repeat this process for as many pages as you can in 20 minutes

## Considerations

- Decorative images do not need alt text, but they do need the alt=”” attribute defined
- If there is no ‘alt’ attribute on the `<img>` tag, a screen reader will read the filename, which typically isn’t ideal
- Alt text does not need to start with “Image of” because a screen reader will give the context that it is an image
- If there is an image with text on it, ensure the same text is in the alt attribute

## Tools

- [​Web Developer Firefox browser extension​](https://addons.mozilla.org/en-US/firefox/addon/web-developer/) - [​Chrome version​](https://chrome.google.com/webstore/detail/web-developer/bfbameneiokkgbdmiekhjnmfkcnldhhm)

## Further resources

- [​Technique H37:Using alt attributes on img elements​](https://www.w3.org/WAI/WCAG21/Techniques/html/H37.html)
- [​Technique H2:Combining adjacent image and text links for the same resource​](https://www.w3.org/WAI/WCAG21/Techniques/html/H2)