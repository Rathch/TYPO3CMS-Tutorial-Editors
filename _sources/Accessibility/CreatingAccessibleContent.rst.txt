..  include:: /Includes.rst.txt

..  _accessibility-creating-accessible-content:
..  _accessibility-writing-accessible-text:

===========================
Creating accessible content
===========================

..  _accessibility-content-clear-text:
..  _accessibility-writing-clear-language:

Write clear text and instructions
=================================

Clear wording helps readers understand what a page offers and what to do
next. This particularly benefits people with cognitive or learning
disabilities and people unfamiliar with the subject.

Start with the main message. Use familiar words, explain necessary
specialist terms and expand unfamiliar abbreviations. Keep paragraphs
focused on one idea.

**Instead of:**

    Submission of the requested documentation is a prerequisite for further
    processing.

**Write:**

    Send us the listed documents so we can process your application.

Use the editor's list functions for related items and ordered steps. Avoid
arranging text with repeated spaces or empty paragraphs.

Refer to controls by their labels:

    Choose "Submit application".

This is more reliable than "Click the green button on the right", which
depends on seeing its color and position.

Further examples are available in
`WAI's Writing for Web Accessibility <https://www.w3.org/WAI/tips/writing/>`__.

..  _accessibility-content-titles-and-headings:

Give pages meaningful titles and headings
=========================================

..  _accessibility-content-page-title:
..  _accessibility-writing-accessible-text-provide-informative-unique:

Identify the page
-----------------

The browser title helps people distinguish open tabs and recognize a page
when using assistive technology. It should identify the page's topic or
purpose.

"Accessible travel to the conference" is more informative than
"Information".

TYPO3's page and SEO settings influence the browser title. Your site may
also add the organization's name. The
`TYPO3 SEO documentation <https://docs.typo3.org/permalink/t3editors:seo>`__
explains the title fields.

..  _accessibility-content-headings:
..  _accessibility-writing-accessible-text-headings-convey-meaning:

Express the content hierarchy
-----------------------------

People scan headings to find relevant sections. Screen reader users can also
navigate directly between headings.

Use actual heading formats. Making a paragraph large or bold does not
provide the same structure.

Choose levels according to how sections relate:

..  list-table:: Heading levels for one page
    :header-rows: 1
    :widths: 20 80

    *   -   Level
        -   Heading
    *   -   H1
        -   Visit the conference
    *   -   H2
        -   Travel
    *   -   H3
        -   Public transport
    *   -   H3
        -   Parking
    *   -   H2
        -   Accessibility at the venue

When opening a subsection, normally move down one level. Returning from H3
to H2 starts a new section and is expected.

Consider headings from the template, content elements and rich text editor
together. Check whether the template already supplies the main heading, and
avoid repeating the same heading in a content element and its text.

Do not choose a different level merely to obtain a preferred font size. See
the
`WAI headings tutorial <https://www.w3.org/WAI/tutorials/page-structure/headings/>`__
for examples.

..  _accessibility-content-links:
..  _accessibility-writing-accessible-text-make-link-text:

Make links understandable
=========================

People need to understand what a link offers before following it. Some move
between links using the keyboard or use a screen reader's list of links.

Prefer descriptive wording:

..  list-table:: Link text that names the destination
    :header-rows: 1
    :widths: 40 60

    *   -   Less helpful
        -   More helpful
    *   -   Click here
        -   Travel directions
    *   -   Download
        -   Conference program
    *   -   More
        -   Accessibility at the venue

Descriptive wording also helps when a link is encountered without the
surrounding paragraph. WCAG allows some link purposes to be understood from
associated context, so "Read more" is not automatically a failure.
Nevertheless, naming the destination is usually clearer. See
`WAI's explanation of link purpose <https://www.w3.org/WAI/WCAG22/Understanding/link-purpose-in-context.html>`__.

For downloads, name the document. File format and size are useful additional
information:

    Conference program (PDF, 1 MB)

See
`Creating a link in TYPO3 <https://docs.typo3.org/permalink/t3editors:rte-linking>`__
for the editing steps.

..  _accessibility-content-images:
..  _accessibility-writing-accessible-text-write-meaningful-text:

Describe images according to their purpose
==========================================

Alternative text makes relevant image information available as text, speech
or Braille. Decide what the image contributes at its particular location.

..  _accessibility-content-images-informative:

Informative images
------------------

Describe the information that would otherwise be lost.

On a page explaining access to a venue, "Building exterior" is too general.
A useful alternative might be:

    Step-free entrance via the ramp beside the main stairs.

On another page, the same photograph may serve a different purpose and need
different wording.

Keep the description focused. Avoid file names, keyword lists and
unsupported interpretations. Usually, there is no need to begin with
"Image of".

There is no universal character limit that makes an alternative text
appropriate. Use enough detail to communicate the relevant information. For
a complex chart, provide a short alternative and explain the findings and
necessary values in accessible text or a data table.

The
`WAI Images Tutorial <https://www.w3.org/WAI/tutorials/images/>`__
explains the different image purposes.

..  _accessibility-content-images-decorative:

Decorative images
-----------------

An image may add visual interest without contributing information, or repeat
information already fully available nearby.

These images should be marked as decorative so assistive technologies can
skip them.

In TYPO3, leaving an alternative text field blank may cause an existing
value to be inherited. Use your project's agreed method for decorative
images. If you are unsure, ask your technical team how to ensure that no
alternative text is output for that use.

For the technical distinction between an empty alternative and a missing
one, see
`WAI's guidance on decorative images <https://www.w3.org/WAI/tutorials/images/decorative/>`__.

..  _accessibility-content-images-links:

Images used as links
--------------------

When an image is the only content of a link, its alternative should identify
the destination or action. A linked program cover might need "Conference
program", rather than a description of its colors.

If descriptive text and an image form the same link, and the image adds no
information, an empty image alternative avoids repetition. See
`WAI's functional image examples <https://www.w3.org/WAI/tutorials/images/functional/>`__.

..  _accessibility-content-images-reuse:

Reusing images in TYPO3
-----------------------

TYPO3 can inherit alternative text from file metadata and allows it to be
overridden for an individual use. Review inherited text whenever you reuse
an image.

A caption supplies visible context; a credit identifies the source. Neither
automatically replaces an appropriate alternative, and unnecessary
repetition should be avoided.

The
`TYPO3 image documentation <https://docs.typo3.org/permalink/t3editors:images>`__
explains the metadata settings.

..  _accessibility-content-images-text:

Keep important text available as text
-------------------------------------

Do not publish dates, prices, instructions or other essential information
only inside a picture.

For example, if you upload a conference poster, also provide its relevant
information as normal page content. This allows readers to enlarge and adapt
the text. A long alternative text is not a substitute for a usable event
description.

Some images of text, such as logos, have legitimate exceptions. See
`WAI's explanation of images of text <https://www.w3.org/WAI/WCAG22/Understanding/images-of-text.html>`__.

..  _accessibility-content-tables:

Keep tables simple and structured
=================================

Tables communicate relationships between data. Someone reading individual
cells with a screen reader needs to know which row and column headings
apply.

Use the available table functions to identify header cells. Making the first
row bold only changes its appearance.

Keep the structure as simple as the information permits. Avoid merged cells
or multiple layers of headings where a simpler presentation would work.
Consider whether smaller tables or an explanatory paragraph would be
clearer.

Use layout components, rather than tables, to position unrelated content
side by side. If the editor cannot represent the required structure, ask for
support.

The
`WAI tables tutorial <https://www.w3.org/WAI/tutorials/tables/>`__
explains these relationships with examples.

..  _accessibility-content-documents:

Provide accessible documents
============================

A clear download link does not make the linked file accessible. Uploading a
document to TYPO3 does not repair its headings, reading order or image
alternatives.

Before publishing, confirm that the document has been prepared and checked
for accessibility. If another team supplies it, make accessibility part of
the request rather than discovering the problem after publication.

Where practical, publish information directly as web content. A downloadable
version may still be useful.

Use your project's guidance for the document format and involve the
responsible team when specialist checking or repair is needed. The German
`BFIT-Bund guidance on accessible documents <https://www.bfit-bund.de/DE/Publikation/handreichung-barrierefreie-dokumente>`__
provides an additional starting point.

..  _accessibility-content-media:
..  _accessibility-writing-captions:

Plan accessible audio and video
===============================

Plan media alternatives when creating or commissioning a recording. What you
need depends on the information conveyed and whether the content is recorded
or live.

..  list-table:: Media alternatives to plan before publication
    :header-rows: 1
    :widths: 45 55

    *   -   Content
        -   What to plan
    *   -   Prerecorded audio, such as a podcast
        -   A transcript containing speech and meaningful sounds.
    *   -   Prerecorded video with meaningful audio
        -   Captions containing speech, relevant sounds and speaker changes where necessary.
    *   -   Prerecorded video without audio
        -   An equivalent text description or an audio track explaining the visual information.
    *   -   Prerecorded video with sound and important visual information
        -   A description of visual information that is not already communicated through the audio. At WCAG level AA, required audio description cannot be replaced by a transcript alone.
    *   -   Live video with meaningful audio
        -   Live captions where required by the project's accessibility target. Plan this before the event.

Some criteria include exceptions for recordings explicitly provided and
labeled as alternatives to existing text. Check the specific requirements
before relying on an exception.

Include essential visual information in the original narration where
possible:

    "Use the step-free entrance on the north side of the building" gives
    more information than "Use this entrance".

Check automatically generated captions, especially names and specialist
terms. Also check that the actual player makes captions, descriptions and
transcripts available.

The
`WAI media planning guide <https://www.w3.org/WAI/media/av/planning/>`__
distinguishes requirements by media type and WCAG level.

..  _accessibility-content-forms:
..  _accessibility-writing-instructions:

Write clear form labels and feedback
====================================

If you create forms, give fields labels that explain what information is
needed. Identify required fields consistently and explain formats that users
cannot reasonably infer.

Placeholder text should not replace a proper label: it disappears during
entry and may not provide a reliable field name.

Write errors that help people recover:

    Enter your arrival date in the format DD.MM.YYYY.

This is more useful than "Invalid input". Give buttons labels that describe
the action, such as "Send inquiry" or "Save changes".

The component must also associate labels, instructions and errors correctly
with the controls. See
`WAI's form instructions <https://www.w3.org/WAI/tutorials/forms/instructions/>`__.

..  _accessibility-content-language-and-formatting:

Use language, color and formatting purposefully
===============================================

Use the project's agreed styles. Avoid introducing local formatting simply
to make a page look different.

Do not rely on color alone. Label cancelled dates "Cancelled" rather than
only coloring them red. If you choose text colors or place text over
images, check their contrast.

Correct language information helps screen readers pronounce content. Use the
appropriate language version of the page and mark passages in another
language using the editor's language function.

Proper names, technical terms and words already adopted into the surrounding
language do not generally need separate language marking. If a required
language setting is unavailable, ask your technical team for a solution. See
`WAI's guidance on language changes <https://www.w3.org/WAI/WCAG22/Understanding/language-of-parts.html>`__.
