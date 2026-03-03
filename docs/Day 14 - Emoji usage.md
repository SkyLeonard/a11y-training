You likely encounter emojis in almost all digital communication you get. From text messages, social media, and even on websites. Emojis are an advancement over emoticons :) since they have built-in alt text. But with that advantage comes some disadvantages.

These general principles apply to websites, social media, or messages. It’s a good practice to use the same guidelines when creating content for any platform.

Emojis should not replace interface elements or replace words. The text “Like” or “Share” are clear labels for the actions available to the user. Replacing them with a 👍 thumbs up or 🔗 link emoji may not convey the same information to a sighted visitor and someone hearing “Thumb up" or "Link symbol" would find it hard to decipher the intent of those two links.

**General principles**

1. Emoji’s should be used sparingly
2. Use common emojis to help with interpretation
3. If an emoji could be used on a light or dark background ensure there is enough contrast
4. Use emojis at the end of sentences instead of in the middle
5. Using a skin tone variation of an emoji adds the skin tone color to the alt text that is read by a screen reader
6. An emoji may look different on various devices, be aware they may not translate the way you see them on your device

## Example

<div style="position: relative; padding-bottom: 59.23076923076923%; height: 0;"><iframe src="https://www.loom.com/embed/7908a7cb8bd341a5a7d478febaa7504f" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>

Video of a screen reader reading emoji characters on a web page

The example video above demonstrates how emojis are read in the context of the words on the page. They visually act like icons but are read aloud with the screen reader and may be distracting to the listener.

## Task

1. Search your website for any emoji usage
2. Determine if the emoji is adding value to the content of the page or if it is for visual presentation only
3. Add the “aria-hidden” attribute to the items that are for presentation only
4. Alternatively, if you do what a specific label to read for the emoji you could change the role to be an image and supply an "aria-label"

## Hide an emoji from a screen reader

`<p>Some text on the page <span aria-hidden="true">😁</span></p>`

## Replace the emoji with image properties

`<p>Some text on the page <span role=”img” aria-label=”excited emoji face”>😁</span></p>`

## Further resources

- [​Emoji names​](https://www.freecodecamp.org/news/all-emojis-emoji-list-for-copy-and-paste/)