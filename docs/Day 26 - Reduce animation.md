Animation can bring some significant interactions on a website and can make connections between actions and their results. In addition, animations to illustrate data or points can show a story of data trends over time in a compact space.

Motion animation can be triggered by visitors, like parallax, as the visitor scrolls down the page. This movement can make some visitors ill or dizzy, and if there isn’t a way to get the information without the motion it can cause serious issues.

Visitors can adjust their system settings to prefer reduced motion so they don’t have to find and adjust motion preferences on each site they visit. This setting allows each site to detect if someone prefers reduced motion so the site can be adjusted accordingly.

For this task, turn on reduced animation for yourself:

- iOS: Settings > General > Accessibility > Reduce Motion
- macOS: System Preferences > Accessibility > Display > Reduce Motion
- Windows: Windows Settings > Ease of Access > Show Animations in Windows

## Example

![Screenshot of the MacOS Preferences pane eith accesibility options open and an arrow pointing to the reduce motion option](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/8Nr2spvmx8TM7o8ne7pToE)

MacOS accessibility options to reduce motion

## Task

1. Follow the steps above on your device to set the reduce animation setting
2. Visit your homepage
3. Interact with the page to determine if there are any animations, videos being played, or elements move
4. Move from page to page throughout your website and look for animated motion or auto-playing videos
5. If any are detected, using the considerations below, adjust the code of the page to detect and reduce the animation effect based on the visitor's settings.

## Considerations

Just because someone doesn’t have the system-wide setting selected to reduce motion, doesn’t mean the specific motion on your site may affect them. Ensuring there is a way to turn off or view the same animated information in another format on your site is still necessary.

In CSS, detecting if someone prefers reduced motion looks like this:

`@media (prefers-reduced-motion: reduce) { /* styles applied if the visitor prefers to reduce motion */ }`

In Javascript, detecting if someone prefers reduced motion looks like this:

```
const mediaQuery = window.matchMedia('(prefers-reduced-motion: reduce)'); mediaQuery.addEventListener('change', () => { console.log(mediaQuery.media, mediaQuery.matches); // Javascript applied to reduce animations });
```

More example code and considerations are provided in the resource links.

## Further resources

- [​SC 2.3.3:Animation from Interactions (Level AAA)​](https://www.w3.org/WAI/WCAG21/Understanding/animation-from-interactions.html)
- [​Technique C39:Using the CSS reduce-motion query to prevent motion​](https://www.w3.org/WAI/WCAG21/Techniques/css/C39)
- [​MDN: prefers-reduced-motion​](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion)
- [​Dev.to: prefers-reduced-motion: Sometimes less movement is more​](https://web.dev/prefers-reduced-motion/)