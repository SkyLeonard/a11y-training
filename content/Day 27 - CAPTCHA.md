Getting information from visitors is a routine task and it's important to ensure the visitors filling out forms are humans and not machines. With the goal of blocking bots from filling out forms, often the solution is to challenge the visitor to prove they are human.

There is an exemption for the WCAG requirements for the content of the CAPTCHA. WCAG still requires that alternative text identify the graphical object as a CAPTCHA. Conformance with all other WCAG guidelines also remains critical for web accessibility.

The common CAPTCHA is to type in a jumbled set of letters, which is a barrier to people who are not able to visually see the image. Non-English speaking visitors will have a hard time distinguishing jumbled characters. The average time it takes to complete a CAPTCHA is 32 seconds, which when added up is a lot of time that could be spent on other productive activities.

Another common option is non-visual CAPTCHAs, the downside is the amount of shared personal information with a third party.

## Example

![Screenshot of a Google CAPTCHA asking to click on images of traffic lights. The Audio option is also selected with an arrow to the player forms.](https://embed.filekitcdn.com/e/qH3zYM66ACnU9H1etxAaxA/8emtLZhfR77pSKfxDvdvRJ)

Google's CAPTCHA which provides multiple ways to challenge a visitor is human

The example above is Google’s CAPTCHA v2 which starts hidden and does the check behind the scenes, if the check fails or isn’t possible, a visual check is presented. An audio alternative is available which also allows downloading the audio to allow a visitor to play the audio through their audio player of choice to replay, slow down, or direct the audio to their preferred output device.

## Task

1. Search your website for any forms where user input is required
2. Determine if a CAPTCHA is required for submission
3. If so, can it be completed with a keyboard only?
4. Can it be completed as an audio alternative?
5. Is there a time limit or another constraint that should be communicated to the visitor?
6. Are there any alternative ways to detect a human or bot?

## Considerations

- The goal is to separate humans from machines. Question if a CAPTCHA is needed at all. If the verification of some other information is possible, for example, email with a required unique URL to complete the account setup.
- Having an internal review process that requires, or allows, for the moderation of user-provided content before the content is displayed online.
- Honeypots are hidden fields from screen readers but scripts will see the field. Because scripts will want to fill out all fields, if a submission has this field filled out, it has a high likelihood of not being human.

## Further resources

- [​Inaccessibility of CAPTCHA​](https://www.w3.org/TR/turingtest/)
- [​Captcha Alternatives and thoughts​](https://www.w3.org/WAI/GL/wiki/Captcha_Alternatives_and_thoughts)