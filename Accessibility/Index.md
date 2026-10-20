---
title: "Accessibility for editors"
manual: "Tutorial for Editors"
version: "main"
permalink: "https://docs.typo3.org/permalink/t3editors:accessibility-overview@main"
source: "Accessibility/Index.rst"
rendered: "2026-10-20T12:56:18+00:00"
---

# Accessibility for editors {#accessibility-overview}

People with disabilities can use a page when they can perceive the content,
operate it, and understand it. The
[W3C Web Accessibility Initiative](https://www.w3.org/WAI/)
publishes the guidelines that describe those requirements. You publish the
words, images, media, and forms. Several of the failures that show up most
often on the web sit in exactly that content.

## What the figures say about your part of the work {#accessibility-statistics}

Two public scans measure how often pages fail checks that a program can
run. A program cannot see every barrier. The W3C states that
[no tool alone can decide whether a site meets the guidelines](https://www.w3.org/WAI/test-evaluate/).
The figures below are the failures the scans could count. They are a floor,
and they already show where an editor changes the result.

### One million home pages {#accessibility-statistics-webaim}

In February 2026, WebAIM checked the home pages of the top 1,000,000 sites
and published the results in
[The WebAIM Million](https://webaim.org/projects/million/).
95.9% of those home pages had at least one automatically detected failure
of the Web Content Accessibility Guidelines (WCAG) 2. The average home page
had 56.1 such errors. 96% of all detected errors fell into six types. The
same six types have led the list for seven years. WebAIM writes that
addressing these few types would significantly improve accessibility across
the web. Five of them show up in the content and the theme:

| Failure | Home pages | Where you can change it in TYPO3 |
| --- | --- | --- |
| Low contrast text | 83.9% | The colors usually come from the theme. If body text is hard to read, ask your integrator. If you set a text color yourself, that color is yours to correct. |
| Missing alternative text for images | 53.1% | You write it, on the file and again for the place where the image is used. |
| Missing form input labels | 51% | You write the label when you build the form. |
| Empty links | 46.3% | You write the link text. A linked image with no alternative text is an empty link too. |
| Empty buttons | 30.6% | Buttons in the theme are the integrator's. A control you add needs a name a reader can follow. |

The report gives a closer count for the items you type in:

-   16.2% of all images had no alternative text. 10.8% of the images that
    did have alternative text used a file name, a filler such as "image",
    or the same text as the image beside them. More than one in four images
    had one of these problems. 45% of the images with no alternative text
    were links, so the link had no usable name. One in four linked images
    had no alternative text.
-   15.2% of home pages had ambiguous link text such as "click here",
    "more", or "continue". Those pages had 5.3 such links on average.
-   Skipped heading levels, such as a heading of level 2 followed by a
    heading of level 4, appeared on 41.8% of home pages. 18.1% had more
    than one heading of level 1.

Home pages that the same study classified as TYPO3 CMS had 38.5 detected
errors on average, compared with 56.1 for all home pages. WebAIM notes that
a higher or lower count next to a technology cannot always be attributed to
that technology. A lower average does not make the content accessible. The
alternative text, the headings, and the link text are still written per page.

### A second scan of page content {#accessibility-statistics-audioeye}

[AudioEye's accessibility statistics](https://www.audioeye.com/post/accessibility-statistics/)
report a separate scan of about 400,000 pages across about 15,000 sites.
In that scan the average page had 297 accessibility issues, and 2% of the
sites passed 70% of the WCAG criteria the scan could test. AudioEye is a
vendor. Treat the article as that company's reading of its own scan, and
use the WebAIM report when you want a method you can read in full.

On images and links, the AudioEye article reports:

-   38% of images had missing alternative text, and 60% of images had no
    alternative text. 93% of domains had at least one page with an
    inaccessible image.
-   64% of pages had links that were not clear to people with disabilities,
    about five such links on a page. 80% of sites had at least one page
    with an inaccessible link.
-   In AudioEye's 2023 index, cited in the same article, 1 in 4 forms were
    missing descriptive labels.

The article lists both image figures. It does not define how "missing
alternative text" differs from "no alternative text", so this manual keeps
them as two reported figures.

Read together, the two scans point at the same editorial work. Alternative
text, link text, headings, and form labels are fields you fill in. Contrast
of the theme and empty buttons in the template are set elsewhere. Ask your
integrator about those.

## Where to go next {#accessibility-where-next}

**[Legal requirements](https://docs.typo3.org/permalink/t3editors:accessibility-legal@main)**

Which rules name WCAG, what the European directives cover, and
which questions to take to your organization. This chapter is not
legal advice.

**[Writing accessible text](https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text@main)**

Page titles, headings, link text, alternative text, captions, and
plain language, with a TYPO3 field for each one.

**[Tips and tricks](https://docs.typo3.org/permalink/t3editors:accessibility-tips@main)**

A check you can run on a page before you publish it.

**[Sources and further reading](https://docs.typo3.org/permalink/t3editors:accessibility-sources@main)**

The guidelines, the writing guide, the tool list, and the studies
cited in this chapter.
