---
title: "Check before publishing"
manual: "Tutorial for Editors"
version: "main"
permalink: "https://docs.typo3.org/permalink/t3editors:accessibility-tips@main"
source: "Accessibility/CheckBeforePublishing.rst"
rendered: "2026-11-06T10:57:15+00:00"
---

<a id="accessibility-check-before-publishing"></a>

# Check before publishing {#accessibility-tips}

Review the actual page in preview, then check the published result. Backend
fields alone do not show whether the website outputs everything correctly.

These checks are an editorial first review. They do not replace a full
accessibility evaluation.

<a id="accessibility-check-review"></a>
<a id="accessibility-tips-before-publish"></a>
<a id="accessibility-tips-title"></a>
<a id="accessibility-tips-headings"></a>
<a id="accessibility-tips-links"></a>
<a id="accessibility-tips-images"></a>
<a id="accessibility-tips-media"></a>
<a id="accessibility-tips-color"></a>
<a id="accessibility-tips-forms"></a>

## Review your content {#accessibility-tips-tables}

| Check | What to do |
| --- | --- |
| **Title and wording** | Read the browser title. Does it identify this page? Check whether the main message and instructions are clear. |
| **Headings** | Review the headings and levels together, including those supplied by content elements. Do they express the intended sections and subsections? |
| **Links** | Follow the links. Check whether their wording matches the destination and whether the correct document version opens. |
| **Images** | Compare each alternative text with the image's purpose. Check how decorative images are handled; visual appearance alone cannot reveal this. |
| **Text in images** | Check whether essential poster text, dates or instructions are also available as normal page content. |
| **Documents and media** | Confirm that accessible documents and necessary media alternatives are available. Play the recording and check the alternatives in the actual player. |
| **Forms** | Review labels without relying on placeholders. In preview or a test environment, trigger validation errors and check whether the messages help with correction. |
| **Presentation** | Enlarge the page and view it at a narrow width. Look for clipped or obscured content and information conveyed only by color. |

For explanations and examples, refer to
[Creating accessible content](https://docs.typo3.org/permalink/t3editors:accessibility-creating-accessible-content@main).

## Use tools for specific questions {#accessibility-check-tools}

### Inspect information that is not normally visible {#accessibility-check-wave}

[WAVE](https://wave.webaim.org/)
can reveal accessibility information and flag potential problems. For
example, use it to inspect the alternative text output for an image, then
decide whether that text conveys the intended information.

WAVE cannot make that editorial judgment. Its indicators need
interpretation, and an absence of reported errors is not proof of
accessibility. The
[WAVE help](https://wave.webaim.org/help)
explains the results.

### Check colors you select {#accessibility-check-contrast}

The
[WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)
compares foreground and background colors and reports contrast results for
different text categories.

Use it when you control those colors. Text over photographs or changing
backgrounds needs additional care; checking one color pair may not represent
the whole image.

### Learn further initial checks {#accessibility-check-easy-checks}

The
[WAI Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/)
explain first checks for titles, headings, images, keyboard access and other
aspects. Some require tools or additional knowledge. They cover only part of
a complete evaluation.

## Report problems you cannot resolve {#accessibility-check-report}

Include:

-   The page URL or TYPO3 page identifier.
-   The affected content element or component.
-   What you observed and what you expected.
-   The steps needed to reproduce the problem.

Report recurring problems so they can be addressed centrally. When updating
content, also revisit its links, descriptions and media alternatives.
