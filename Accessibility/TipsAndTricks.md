---
title: "Tips and tricks"
manual: "Tutorial for Editors"
version: "main"
permalink: "https://docs.typo3.org/permalink/t3editors:accessibility-tips@main"
source: "Accessibility/TipsAndTricks.rst"
rendered: "2026-10-20T12:34:02+00:00"
---

# Tips and tricks {#accessibility-tips}

Use this list on a page before you publish it. Each item names the
requirement it supports. The explanations of those requirements are linked
from
[Legal requirements](https://docs.typo3.org/permalink/t3editors:accessibility-legal@main).
How to fill the fields is in
[Writing accessible text](https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text@main).

A program can find some of these failures. It cannot decide that the page
is accessible. The W3C says so in its
[introduction to evaluating accessibility](https://www.w3.org/WAI/test-evaluate/),
and it keeps a
[list of evaluation tools](https://www.w3.org/WAI/test-evaluate/tools/list/)
submitted by the providers. The W3C does not endorse the products on that
list. For a first pass a person can do without a product, use the W3C
[Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/).

## Before you publish {#accessibility-tips-before-publish}

### Read the title out of context {#accessibility-tips-title}

Open the page and read only the browser title. It should name this page.
"Home", the organization name alone, or "Page" fails that test on an inner
page. Set the page title, and the title for search engines when you use
that field, as described under
[Provide informative, unique page titles](https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text-provide-informative-unique@main).

### Walk the headings {#accessibility-tips-headings}

List the headings in order, including the levels. You should get an outline
of the page. A level jumps from 2 to 4 when a level was chosen because it
looked smaller. One topic keeps one heading. The page title may already be
the level-1 heading. Ask your integrator if you are unsure, then start the
content element headings at level 2.

### Read the links as a list {#accessibility-tips-links}

Collect every link on the page and read the texts without the sentences
around them. Each text should say where that link goes.

Change these when you find them:

-   "Click here", "here", "more", "read more", "continue".
-   A raw address as the only link text, when the page has a title you can
    use instead.
-   An empty link, including an icon or an image with no alternative text.
-   Two links with the same text that go to different places. "Download"
    twice, for two different files, needs the file name in the link.

A file link names the type: "Hut rules (PDF)".

### Cover the image {#accessibility-tips-images}

Cover the image with your hand and read the alternative text. If you still
learn what the image was there to say, the text is doing its job. If the
paragraph already says it, the image is decorative and the alternative text
should be empty.

Reject "image", "photo", "icon", a file name, and a text identical to the
caption that is already visible under the image. The
**Description** and the alternative text are different fields. The
description is often shown to everyone. The alternative text stands in for
the image.

### Play the video with the sound off {#accessibility-tips-media}

If you cannot follow a video with the sound off, the captions or the
transcript are missing. Put a transcript in the text of the content element
and give it a heading. Ask your integrator how the player on your site
takes a captions file.

Leave automatic playback off. If a clip must start by itself and it lasts
more than three seconds, the visitor needs a way to pause it or to change
its volume separately from the device.

### Check color and text saved as an image {#accessibility-tips-color}

"Required fields are shown in red" needs the word "required" as well.
A heading that is a picture, or a phone number that is a picture, should be
typed as text. A logo may stay an image. Its alternative text is the words
in the logo.

If you colored text in the editor, check the contrast.
[Success Criterion 1.4.3](https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html)
requires a contrast ratio of at least 4.5:1. Large-scale text, at least 18
point or 14 point bold, needs at least 3:1. Text that is pure decoration,
inactive, or part of a logo has no contrast requirement under that
criterion. The colors of the theme are the integrator's. Low contrast was
the most common failure in the February 2026 WebAIM report: 83.9% of home
pages, with 34 instances on an average home page.

### Label every field {#accessibility-tips-forms}

Read the form with the placeholders ignored, because placeholders vanish
while someone types. Every field needs a visible label. Say the format when
it is easy to get wrong: "Date of arrival (DD.MM.YYYY)".

Trigger an error on purpose. The message should name the field and the
change. "Invalid input" does not. The W3C example of a message that names
the problem is "The password needs to include at least one number."

### Mark a language change {#accessibility-tips-language}

The language of the page is part of the site setup. An administrator sets
it. When you edit a translation, you are already in that language. See
[Working with languages](https://docs.typo3.org/permalink/t3editors:languages@main).

A quotation or a title in another language, inside a page of one language,
needs to be marked.
[Success Criterion 3.1.2](https://www.w3.org/WAI/WCAG21/Understanding/language-of-parts.html)
is the requirement. If your rich text editor has a language option, set it
on that phrase. If it has none, ask your integrator to enable it. Until
then, avoid dropping in unmarked passages in a second language.

### Mark the header cells of a table {#accessibility-tips-tables}

A table of data needs header cells, not a bold first row. A screen reader
can then repeat the header as the reader moves across a row. The W3C
tutorial on [tables](https://www.w3.org/WAI/tutorials/tables/) shows the
patterns, including tables with two headers. A layout that only uses a
table to place two pieces of text side by side is a question for your
integrator. Prefer two paragraphs or a list when the content is not a table.

## What to hand to your integrator {#accessibility-tips-integrator}

These failures showed up often in the February 2026 WebAIM report, and you
cannot fix them in a content element:

-   Body text, buttons, and form fields in the theme whose contrast is too
    low. 83.9% of home pages had low-contrast text.
-   Buttons and icons in the template that have no accessible name. Empty
    buttons were on 30.6% of home pages.
-   A skip link, keyboard focus, and the order of the keyboard tab. Those
    belong to the template.
-   A captions control, if the media player has nowhere for you to add a
    captions file.

Send a specific page address and a specific element. "The body text on the
home page is gray on white" gives your integrator something to change.
"The site is not accessible" does not.
