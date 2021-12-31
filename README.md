# Web a11y Cheatsheet
#### ([cause I can't go a day without you](https://www.youtube.com/watch?v=3xDzUFNbDy0#t=1m24s))

![MIT license badge](https://img.shields.io/github/license/azemetre/react-a11y-cheatsheet) ![contributor count](https://img.shields.io/github/contributors/azemetre/react-a11y-cheatsheet)
---
Cheatsheet for Web developers getting started with a11y.

a11y is a [numeronym](https://en.wikipedia.org/wiki/Numeronym) for accessibility. Pretty neat.

WIP for now, but the need is real.

---
Table of contents:
* [prerequisites](#prereqs)
* [why a11y?](#why)
* [assistive technology](#at)
* [extensions, plugins, and tooling](#tools)
* [free resources](#freeresources)
* [paid resources](#paidresources)
* [glossary](#glossary)
---

### [prerequisites](#prereqs)

Before getting started it's recommended you are familiar the following, this is introduce the concepts of how HTML and JavaScript can impact a11y:
* [semantic HTML](https://developer.mozilla.org/en-US/docs/Glossary/Semantics#Semantics_in_HTML)
* [browser events](https://developer.mozilla.org/en-US/docs/Web/Guide/Events/Event_handlers)
* [the accessibility tree](https://developers.google.com/web/fundamentals/accessibility/semantics-builtin/the-accessibility-tree)
* [how accessibility trees inform assistive tech](https://hacks.mozilla.org/2019/06/how-accessibility-trees-inform-assistive-tech/)

---

### [why a11y](#why)

---

### [assistive technology](#at)
Assistive technology (AT) are the tools and equipment people use to interact with your application or site. Some examples of AT include [braille displays](https://en.wikipedia.org/wiki/Refreshable_braille_display), allowing blind users to understand what's on their screen in real time, or [VoiceOver](https://www.apple.com/accessibility/mac/vision/), converts text to speech.

Many of these technologies can change the way a website is displayed or how a user will interact. To read or learn more about assistive technology please follow the [Assistive Technology Industry Association](https://www.atia.org/).

#### Common Usage
Screen readers are a typical use case of AT.

#### [WebAIM 2019 Screen Reader Survey](https://webaim.org/projects/screenreadersurvey8/)
Surveys done by WebAIM are a treasure trove of insight when assessing what types of tools and platforms you should be targeting to make a11y compliant sites. Some of the key take aways:
* 71.% of respondents exclusively rely on screen reader audio for their usage.
* For all major platforms (Desktop, Laptop, Mobile device/Tablet) more respondants use screen readers, ranging from 67% to 86%.
* The top 3 screen readers actively used on desktop/laptop: NVDA at 72%, JAWS at 61%, and VoiceOver at 47%,
* Most common screen reader and browser combinations: JAWS with Chrome at 21%, NVDA with Firefox at 19%, NVDA with Chrome at 18%, JAWS with Internet Explorer at 11%, VoiceOver with Safari at 9%
* What is your primary mobile/tablet platform: Apple iPhone, iPad, or iPod touch at 69% and Android at 27%
* Mobile screen readers used: VoiceOver at 71%, TalkBack for Android at 33%

While JAWS is a paid tool, usage of NVDA and VoiceOver are more than sufficient to cover the largest audience for both mobile and non-mobile platforms. This provides the most coverage for the least costs.

[NVDA is freely available on Windows](https://www.nvaccess.org/)

#### How to set up various voice over tools, enable keyboard accessibility, and keyboard shortcuts
[NVDA Keyboard Shortcuts](https://dequeuniversity.com/screenreaders/nvda-keyboard-shortcuts)

[Talkback Gestures on Android](https://dequeuniversity.com/screenreaders/talkback-shortcuts)

[VoiceOver Keyboard Shortcuts on a Mac](https://dequeuniversity.com/screenreaders/voiceover-keyboard-shortcuts)

[VoiceOver Gestures on iOS](https://dequeuniversity.com/screenreaders/voiceover-ios-shortcuts)

[Enabling Keyboard Accessibility on a Mac](https://dequeuniversity.com/mac/keyboard-access-mac)

---

### [extensions, plugins, and tooling](#tools)

#### Chrome Extensions
* [axe - Web Accessibility Testing](https://chrome.google.com/webstore/detail/axe-web-accessibility-tes/lhdoppojpmngadmnindnejefpokejbdd)
* [Accessibility Insights for Web](https://chrome.google.com/webstore/detail/accessibility-insights-fo/pbjjkligggfmakdaogkfomddhfmpjeni)
  * [Accessibility Insights for Web Overview](https://accessibilityinsights.io/docs/en/web/overview)
* [HTML5 Outliner](https://chrome.google.com/webstore/detail/html5-outliner/afoibpobokebhgfnknfndkgemglggomo)
* [Color Contrast Analyzer](https://chrome.google.com/webstore/detail/color-contrast-analyzer/dagdlcijhfbmgkjokkjicnnfimlebcll)

#### Firefox Extensions
* [WAVE Accessibility Tool](https://addons.mozilla.org/en-US/firefox/addon/wave-accessibility-tool/)
* [axe - Web Accessibility Testing](https://addons.mozilla.org/en-US/firefox/addon/axe-devtools/)
* [a11y-outline](https://addons.mozilla.org/en-US/firefox/addon/a11y-outline/)

### Plugins
* [eslint-plugin-jsx](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y#readme)
* [storybook-addon-a11y](https://github.com/storybookjs/storybook/tree/next/addons/a11y)

#### Automated Tooling
* [axe-core](https://github.com/dequelabs/axe-core)
* [jest-axe](https://github.com/nickcolley/jest-axe)
* [cypress-axe](https://github.com/avanslaars/cypress-axe)
* [axe-playwright](https://github.com/abhinaba-ghosh/axe-playwright)
* [jest-puppeteer-axe](https://github.com/WordPress/gutenberg/tree/master/packages/jest-puppeteer-axe)
* [axe-puppeteer](https://github.com/dequelabs/axe-puppeteer)
* [react-axe](https://github.com/dequelabs/react-axe)
* [tota11y](https://github.com/Khan/tota11y)
* [lighthouse](https://github.com/GoogleChrome/lighthouse)

---

### [free resources](#freeresources)

#### Sites
* [Learn Accessibility by MDN](https://developer.mozilla.org/en-US/docs/Learn/Accessibility)
* [Microsoft Inclusive Design Methodology](https://www.microsoft.com/design/inclusive/)
* [Inclusive Design Principles](https://inclusivedesignprinciples.org/)
* [Gov.uk Accessible Design System](https://design-system.service.gov.uk/accessibility/)
* [Gov.uk Accessible Service Manual](https://www.gov.uk/service-manual/helping-people-to-use-your-service/making-your-service-accessible-an-introduction)
* [accessibilitysupported/a11ysupport.io](https://github.com/accessibilitysupported/a11ysupport.io)
* [w3c/silver](https://github.com/w3c/silver)

##### Blogs
* [Inclusive Components](https://inclusive-components.design/)
* [Accessibility in Government](https://accessibility.blog.gov.uk/)
* [a11y with Lindsey ](https://www.a11ywithlindsey.com/blog)
* [Journey of a Disabled Web Developer](https://ashleemboyer.com/)

##### Posts
* [Firefox Dev Tools - Accessibility Inspector](https://developer.mozilla.org/en-US/docs/Tools/Accessibility_inspector)

#### Books
* [Microsoft Inclusive Toolkit Manual (PDF)](https://download.microsoft.com/download/b/0/d/b0d4bf87-09ce-4417-8f28-d60703d672ed/inclusive_toolkit_manual_final.pdf)

#### Courses
* [Develop Accessible Web Apps with React by Erin Doyle - egghead.io](https://egghead.io/courses/develop-accessible-web-apps-with-react)

---

### [paid resources](#paidresouces)

#### Courses
* [Accessibility in JavaScript Applications by Marcy Sutton - frontendmasters.com](https://frontendmasters.com/workshops/javascript-accessibility/)
* [Deque University Full Curriculum - dequeuniveristy.com](https://dequeuniversity.com/curriculum/packages/full)
* [Start Building Accessible Web Applications Today by Marcy Sutton - egghead.io](https://egghead.io/courses/start-building-accessible-web-applications-today)

#### Books
* [Inclusive Components: The Book by Heydon Pickering](http://book.inclusive-components.design/)
* [The Bootcampers Guide To Web Accessibilty by Lindsey Kopacz](https://a11y-with-lindsey.ck.page/products/pre-order-the-bootcampers-guide-to-web)

**PLEASE NOTE:** I do not know or work with the above people or organizations, simply recommending good resources.

### [glossary](#glossary)

<details><summary>glossary</summary>
  
* **a11y** (accessibility)
  * a11y is a [numeronym](https://en.wikipedia.org/wiki/Numeronym) for accessibility
* **assistive technology**
  * the tools and equipment people use to interact with your application or site. examples include: screen readers, screen magnification software, or alternative input displays suchas head pointers, motion tracking, or large-print and tactile keyboards
* **accessibility tree** (accessibility object model)
  * contains accessiblity-related information for most HTML elements.
</details>

---
