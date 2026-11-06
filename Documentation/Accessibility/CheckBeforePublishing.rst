..  include:: /Includes.rst.txt

..  _accessibility-check-before-publishing:
..  _accessibility-tips:

=======================
Check before publishing
=======================

Review the actual page in preview, then check the published result. Backend
fields alone do not show whether the website outputs everything correctly.

These checks are an editorial first review. They do not replace a full
accessibility evaluation.

..  _accessibility-check-review:
..  _accessibility-tips-before-publish:
..  _accessibility-tips-title:
..  _accessibility-tips-headings:
..  _accessibility-tips-links:
..  _accessibility-tips-images:
..  _accessibility-tips-media:
..  _accessibility-tips-color:
..  _accessibility-tips-forms:
..  _accessibility-tips-tables:

Review your content
===================

..  list-table:: Checks before you publish a page
    :header-rows: 1
    :widths: 28 72

    *   -   Check
        -   What to do
    *   -   **Title and wording**
        -   Read the browser title. Does it identify this page? Check whether the main message and instructions are clear.
    *   -   **Headings**
        -   Review the headings and levels together, including those supplied by content elements. Do they express the intended sections and subsections?
    *   -   **Links**
        -   Follow the links. Check whether their wording matches the destination and whether the correct document version opens.
    *   -   **Images**
        -   Compare each alternative text with the image's purpose. Check how decorative images are handled; visual appearance alone cannot reveal this.
    *   -   **Text in images**
        -   Check whether essential poster text, dates or instructions are also available as normal page content.
    *   -   **Documents and media**
        -   Confirm that accessible documents and necessary media alternatives are available. Play the recording and check the alternatives in the actual player.
    *   -   **Forms**
        -   Review labels without relying on placeholders. In preview or a test environment, trigger validation errors and check whether the messages help with correction.
    *   -   **Presentation**
        -   Enlarge the page and view it at a narrow width. Look for clipped or obscured content and information conveyed only by color.

For explanations and examples, refer to
`Creating accessible content <https://docs.typo3.org/permalink/t3editors:accessibility-creating-accessible-content>`_.

..  _accessibility-check-tools:

Use tools for specific questions
================================

..  _accessibility-check-wave:

Inspect information that is not normally visible
------------------------------------------------

`WAVE <https://wave.webaim.org/>`__
can reveal accessibility information and flag potential problems. For
example, use it to inspect the alternative text output for an image, then
decide whether that text conveys the intended information.

WAVE cannot make that editorial judgment. Its indicators need
interpretation, and an absence of reported errors is not proof of
accessibility. The
`WAVE help <https://wave.webaim.org/help>`__
explains the results.

..  _accessibility-check-contrast:

Check colors you select
-----------------------

The
`WebAIM Contrast Checker <https://webaim.org/resources/contrastchecker/>`__
compares foreground and background colors and reports contrast results for
different text categories.

Use it when you control those colors. Text over photographs or changing
backgrounds needs additional care; checking one color pair may not represent
the whole image.

..  _accessibility-check-easy-checks:

Learn further initial checks
----------------------------

The
`WAI Easy Checks <https://www.w3.org/WAI/test-evaluate/preliminary/>`__
explain first checks for titles, headings, images, keyboard access and other
aspects. Some require tools or additional knowledge. They cover only part of
a complete evaluation.

..  _accessibility-check-report:

Report problems you cannot resolve
==================================

Include:

*   The page URL or TYPO3 page identifier.
*   The affected content element or component.
*   What you observed and what you expected.
*   The steps needed to reproduce the problem.

Report recurring problems so they can be addressed centrally. When updating
content, also revisit its links, descriptions and media alternatives.
