---
date: 2018-07-09 09:00:00 -0500
title: "Accessibility for front-end developers"
deck: ""
summary: ""
guide: accessibility-for-teams
primary_image: accessibility-for-teams-guide
summary_box: true
topics:
  - accessibility
  - product-and-project-management
  - user-experience
layout: single
---

## Getting started

Accessible front-end development ensures people with different abilities can access, understand, and navigate web content, regardless of how they're accessing it. Front-end developers collaborate with other members of a cross-functional team to implement a robust user experience.

**How to use this guide:**

- We recommend conducting accessibility testing throughout the design and development processes.
- A good place to start testing is on high-touch pages, critical user paths, and site-wide templates.
- If you have project-specific questions, ask your agency’s accessibility team.

## Keyboard access

Can you reach anything that’s interactive using the tab key?

### Why it's important

- Maria has tendonitis and is unable to use a mouse; instead, she uses the keyboard to navigate the web.

### Steps to take

1. Use the keyboard to navigate through the page using the `tab` key.
2. Make sure you can reach all interactive elements and trigger them with the `spacebar`, `enter` key, or arrow keys.
  - Use semantic HTML elements that are accessible by default (For example: buttons, labeled inputs, etc.). If you must use divs for interactions, ensure they are focusable and labeled appropriately.
3. Check to see that focus is always visible and appears in logical order.
4. Make sure that no content gets focused offscreen or is hidden from view.
5. Check to see that the page includes a skip navigation link (if navigation is present before the main content). This will allow users to skip past navigation to reach the page’s main content.

### Resources

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [2.1 Keyboard Accessible (Guideline)](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=128%2C14&currentsidebar=%23col_overview#keyboard-operation)
- [2.1.1 Keyboard](https://www.w3.org/WAI/WCAG20/quickref/#keyboard-operation-keyboard-operable)
- [2.1.2 No Keyboard Trap](https://www.w3.org/WAI/WCAG20/quickref/#keyboard-operation-trapping)
- [2.4.3 Focus Order](https://www.w3.org/WAI/WCAG20/quickref/#navigation-mechanisms-focus-order)
- [2.4.7 Focus Visible](https://www.w3.org/WAI/WCAG20/quickref/#navigation-mechanisms-focus-visible)

Video tutorial:

- How I do an accessibility check

{{< youtube id="cOmehxAU_4s" title="How I do an accessibility check" >}}


## Screen reader

Can you use a screen reader to access the page content?

### Why it's important

- Devonte is blind and uses a screen reader to navigate the web.

### Steps to take

1. Use a screen reader to make sure you can land on controls and that they’re announcing things as they should.
2. Determine whether the HTML document has a language attribute so that screen readers will read it with the correct accent and pronunciation. For example: `<html lang="en">`.
3. If forms are present, make sure the screen reader reads labels and instructions.
4. Make sure that all links are properly descriptive. For example, the link text "Read More" provides no context about where the user will go if they click it, while "Read more about dinosaurs" describes what’s on the other side of the link.

### Use VoiceOver screen reader on Mac

- **Turn VoiceOver on**: command (⌘) + F5
- **Go into web area**: control + alt + shift + down arrow (⬇)
- **Navigate right**: control + alt + right arrow (➡️️)
- **Navigate by heading**: control + alt + command (⌘) + H
- **Click**: control + alt + spacebar

Use rotor to browse pages. The rotor lists common elements like <i>headings</i>, <i>links</i>, and <i>images</i>, and lets you navigate directly to the element of your choosing.

- **Turn on rotor**: control + alt + U
- **Navigate rotor**: left and right, up and down arrows

### Resources

- [Download NVDA screen reader (NV Access)](https://www.nvaccess.org/download/)

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [1.3.1 Info and Relationships](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=128%2C14&currentsidebar=%23col_overview#content-structure-separation-programmatic)

Video tutorials:

- Screen Reader Basics: VoiceOver

{{< youtube id="5R-6WvAihms" title="Screen Reader Basics: VoiceOver" start_time="145" >}}

- Video tutorial: How I do an accessibility check (screen reader)

{{< youtube id="cOmehxAU_4s" title="How I do an accessibility check (screen reader)" start_time="145" >}}


## Headings

Are you using accurate headings on your page?

### Why it's important

- Lalit is blind and uses a screen reader to navigate the web. She hears an outline of the page's main ideas, then backtracks to read the parts she's most interested in.

### Steps to take

1. Headings briefly describe the section it introduces. Headings represent an outline of the content.
2. Use `h1`–`h6` to define your section headings, where `h1` is the highest section level and `h6` is the lowest.
3. Avoid skipping heading levels: Always start with `h1`, use `h2` next, and so on.
4. Use only one `h1` per page for the page title.

{{< note >}}
While HTML5 allows you to reset headings to `h1` on new section elements, some screen reader users will have difficulty discerning the structure of pages with multiple h1s. For this reason, it’s best to include only one h1 per page.
{{< /note >}}

### Resources

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [2.4.6 Headings and Labels](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=128%2C14&currentsidebar=%23col_overview#navigation-mechanisms-descriptive)

Video tutorials:

- Using headings

{{< youtube id="ZHWcs5d9IqA" title="Using Headings" >}}

- How I do an accessibility check (page structure)

{{< youtube id="cOmehxAU_4s" title="How I do an accessibility check (screen reader)" start_time="381" >}}


## Page structure

Are you using semantic elements and roles?

### Why it's important

- Carlos is low-sighted and navigates pages by jumping to the page section he wants to get to.

### Steps to take

1. Use sectioning elements to create a broad outline of your page content; examples of these elements include `header`, `nav`, `main`, and `footer`. Use content sectioning elements like `section`, `article`, and `aside` to organize the document content into logical pieces.
2. Add `role="banner"` to your masthead and `role="contentinfo"` to your page footer once per page to define landmark elements.

### Resources

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [1.3.1 Info and Relationships](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=14%2C128&currentsidebar=%23col_overview#content-structure-separation-programmatic)
- [2.4.1 Bypass Blocks](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=14%2C128&currentsidebar=%23col_overview#navigation-mechanisms-skip)

Video tutorial:

- Landmarks

{{< youtube id="bww3IaktlRY" title="Landmarks" start_time="12" >}}


## Images

Do images have good alt text?

### Why it's important

- Carmen’s page didn’t load all the way and didn’t get to download the images. 
- Amanda is blind and has to read the alt text to understand the contents of the image. 
- John is looking for information with a search engine and needs help being directed to the right content (descriptive alt text will improve search).

### Steps to take

1. Include meaningful information describing each image in the alt text.
2. Use null (empty) alt text when text describing the image is already on the page (`alt=""`).
3. Don’t start the alt text with _Image of_ or _Photo of_ – the screen reader already announces that images are images.
4. If the image is decorative and you don’t want the screen reader to announce it at all, use null (empty) alt text (`alt=""`) or CSS background images.

### Resources

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [1.1 Text Alternatives (Guideline)](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=14%2C128&currentsidebar=%23col_overview&tags=images%2Cimages-of-text%2Ctext-alternatives#text-equiv)
- [1.1.1 Non-text Content](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=14%2C128&currentsidebar=%23col_overview#text-equiv-all)
- [1.4.5 Images of Text](https://www.w3.org/WAI/WCAG20/quickref/#qr-visual-audio-contrast-text-presentation)


## Color and contrast

### Why it's important

Is there enough contrast between text and its background color?

- Rohit has low vision and needs content to have enough contrast to read it. 
- Esther is red-green colorblind and can’t make sense of information conveyed with color alone.

### Steps to take

1. Use a [color contrast](http://webaim.org/resources/contrastchecker/) tool and test that the contrast between the text and background is greater than or equal to 4.5:1.
2. Use an [automated tool](http://wave.webaim.org/) to quickly scan for color contrast problems.
3. Don’t use color alone to convey meaning. Use icons, text, and other visual elements to reinforce the meaning of the content.

### Resources

- [WebAIM Color Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [Accessible Colors](http://accessible-colors.com/)

Web Content Accessibility Guidelines (WCAG) 2.0 references:

- [1.4.3 Contrast (Minimum)](https://www.w3.org/WAI/WCAG20/quickref/?showtechniques=128%2C14&currentsidebar=%23col_overview#visual-audio-contrast-contrast)

Video tutorials:

- Meeting contrast requirements

{{< youtube id="gH1JieTZQ1k" title="Meeting Contrast Requirements" >}}

- How I do an accessibility check (contrast)

{{< youtube id="cOmehxAU_4s" title="How I do an accessibility checks" start_time="516" >}}


## Automated testing

Did your accessibility testing tools provide accurate results?

### Why it's important

Including automated accessibility testing throughout the development process can help quickly catch [many accessibility errors](https://accessibility.blog.gov.uk/2017/02/24/what-we-found-when-we-tested-tools-on-the-worlds-least-accessible-webpage/), but can’t guarantee that your site is accessible. 

Always combine automated testing with ongoing manual testing. Manual testing is the most reliable method to assess accessibility.

### Steps to take

1. **Quick check**: Use a tool to quickly check for common errors in your browser. You can use [HTML CodeSniffer](http://squizlabs.github.io/HTML_CodeSniffer/), [aXe](https://chrome.google.com/webstore/detail/axe/lhdoppojpmngadmnindnejefpokejbdd?hl=en-US), [Lighthouse Accessibility Audit](https://developers.google.com/web/tools/lighthouse/), [Accessibility Insights](https://accessibilityinsights.io/), or [WAVE](http://wave.webaim.org/extension/).
2. **Build process**: Integrate a tool like [axe-core](https://github.com/dequelabs/axe-core), [jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y), [Lighthouse Audits](https://github.com/GoogleChrome/lighthouse/blob/master/docs/readme.md#using-programmatically), or [AccessLint.js](https://github.com/accesslint/accesslint.js/tree/master) into your project to programmatically add accessibility tests and catch errors as you build out your website.
3. **Continuous integration**: Use a tool like [AccessLint](https://www.accesslint.com/) to find accessibility issues in your GitHub pull requests.
4. **Simulate impairments**: Use tools to simulate color blindness, low vision, zoom, low contrast, high contrast, and more.

### Resources

- [GOV.UK: What we found when we tested tools on the world’s least-accessible webpage](https://accessibility.blog.gov.uk/2017/02/24/what-we-found-when-we-tested-tools-on-the-worlds-least-accessible-webpage/)

Video tutorial:

- How I do an accessibility check (tools and extensions)

{{< youtube id="cOmehxAU_4s" title="How I do an accessibility checks" start_time="537" >}}

---

**Disclaimer**: All references to specific brands, products, and companies are used only for illustrative purposes and do not imply endorsement by the U.S. federal government or any federal government agency.
