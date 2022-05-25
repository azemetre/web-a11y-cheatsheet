# Web a11y Cheatsheet
#### ([cause I can't go a day without you](https://www.youtube.com/watch?v=3xDzUFNbDy0#t=1m24s))

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) ![contributor count](https://img.shields.io/github/contributors/azemetre/react-a11y-cheatsheet)
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

Accessibility standards are becoming more critical, not just legally, but are also actively becoming part of standard development, design, and product workflows.

While an immediate benefit is having a compliant site/app, other benefits include easier automation, testing, and customer support.

---

### [assistive technology](#at)
Assistive technology (AT) are the tools and equipment people use to interact with your application or site. Some examples of AT include [braille displays](https://en.wikipedia.org/wiki/Refreshable_braille_display), allowing blind users to understand what's on their screen in real time, or [VoiceOver](https://www.apple.com/accessibility/mac/vision/), converts text to speech.

Many of these technologies can change the way a website is displayed or how a user will interact. To read or learn more about assistive technology please follow the [Assistive Technology Industry Association](https://www.atia.org/).

#### Common Usage
Screen readers are a typical use case of AT.

#### [WebAIM 2021 Screen Reader Survey](https://webaim.org/projects/screenreadersurvey9/)
Surveys done by WebAIM are a treasure trove of insight when assessing what types of tools and platforms you should be targeting to make a11y compliant sites. Some of the key take aways:
* ["Respondents without disabilities tend to be more positive about recent progress (47.4% thought it has become more accessible) than those with disabilities (38.6% thought it has become more accessible)"](https://webaim.org/projects/screenreadersurvey9/#progress)
* [79.5% of respondents have blindness as a disability](https://webaim.org/projects/screenreadersurvey9/#disabilitytypes)
* [Chrome is the majority browser used for screen readers (53.6%) followed by MS Edge (18.4%)](https://webaim.org/projects/screenreadersurvey9/#browsers)
* [The top 3 screen readers actively used on desktop/laptop: JAWS at 70%, NVDA at 58.8%, and VoiceOver at 41.3%](https://webaim.org/projects/screenreadersurvey9/#used)
* [Most common browser combinations for the leading screen readers: JAWS with Chrome at 32.5%, NVDA with Chrome at 16%, VoiceOver with Safari	4.7%](https://webaim.org/projects/screenreadersurvey9/#browsercombos)
* [What is your primary mobile/tablet platform: Apple iPhone, iPad, or iPod touch at 71.9% and Android at 25.8%](https://webaim.org/projects/screenreadersurvey9/#mobileplatforms)
* [Mobile screen readers used: VoiceOver at 71.5%, TalkBack for Android at 29.1%](https://webaim.org/projects/screenreadersurvey9/#mobilescreenreaders)

While JAWS is a paid tool, usage of NVDA and VoiceOver are more than sufficient to cover the largest audience for both mobile and non-mobile platforms. This provides the most coverage for the least costs.

[NVDA is freely available on Windows](https://www.nvaccess.org/)

#### Why not focus on JAWS?

A good strategy on how to prepare for a compliant site/app is to target with tools that are freely available. This is done solely to be pragmatic.

If you are able to fully navigate your site or application with a keyboard and screen readers such as NVDA or VoiceOver you're in a good position.

When you run into accessibility violations, they are normally triaged as browser bugs. Handle the edge cases and regressions as they come in, triage accordingly and document what combination of browser and screen reader are having the issue. If an issue arises with JAWS and Firefox, now you can justify buying a JAWS license for that specific edge case.

While ideally it would be best to have sufficient user research (people with disabilities and without) and sufficient budgeting to allow a variety of hardware and software mixtures (to account for the variety of combinations) we can make due by being pragmatic in the tools and strategies we choose.

By focusing on keyboard navigation and ensuring both screen readers NVDA and VoiceOver are able to fully navigate your site/app you're in a position to prove good faith.

---

[Be aware that JAWS usage is highly regional. Australia and North America tend to have more JAWS usage versus Europe, Asia, Africa, and the Middle East which slightly favor NVDA usage.](https://webaim.org/projects/screenreadersurvey9/#primary)

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
* [EqualAccess](https://github.com/IBMa/equal-access)
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
