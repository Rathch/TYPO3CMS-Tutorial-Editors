..  include:: /Includes.rst.txt

..  _accessibility-tips:

===============
Tips and tricks
===============

Use this list on a page before you publish it. Each item names the
requirement it supports. The explanations of those requirements are linked
from
`Legal requirements <https://docs.typo3.org/permalink/t3editors:accessibility-legal>`_.
How to fill the fields is in
`Writing accessible text <https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text>`_.

A program can find some of these failures. It cannot decide that the page
is accessible. The W3C says so in its
`introduction to evaluating accessibility <https://www.w3.org/WAI/test-evaluate/>`__,
and it keeps a
`list of evaluation tools <https://www.w3.org/WAI/test-evaluate/tools/list/>`__
submitted by the providers. The W3C does not endorse the products on that
list. For a first pass a person can do without a product, use the W3C
`Easy Checks <https://www.w3.org/WAI/test-evaluate/preliminary/>`__.

..  _accessibility-tips-before-publish:

Before you publish
==================

..  _accessibility-tips-title:

Read the title out of context
-----------------------------

Open the page and read only the browser title. It should name this page.
"Home", the organization name alone, or "Page" fails that test on an inner
page. Set the page title, and the title for search engines when you use
that field, as described under
`Provide informative, unique page titles <https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text-provide-informative-unique>`_.

..  _accessibility-tips-headings:

Walk the headings
-----------------

List the headings in order, including the levels. You should get an outline
of the page. A level jumps from 2 to 4 when a level was chosen because it
looked smaller. One topic keeps one heading. The page title may already be
the level-1 heading. Ask your integrator if you are unsure, then start the
content element headings at level 2.

..  _accessibility-tips-links:

Read the links as a list
------------------------

Collect every link on the page and read the texts without the sentences
around them. Each text should say where that link goes.

Change these when you find them:

*   "Click here", "here", "more", "read more", "continue".
*   A raw address as the only link text, when the page has a title you can
    use instead.
*   An empty link, including an icon or an image with no alternative text.
*   Two links with the same text that go to different places. "Download"
    twice, for two different files, needs the file name in the link.

A file link names the type: "Hut rules (PDF)".

..  _accessibility-tips-images:

Cover the image
---------------

Cover the image with your hand and read the alternative text. If you still
learn what the image was there to say, the text is doing its job. If the
paragraph already says it, the image is decorative and the alternative text
should be empty.

Reject "image", "photo", "icon", a file name, and a text identical to the
caption that is already visible under the image. The
:guilabel:`Description` and the alternative text are different fields. The
description is often shown to everyone. The alternative text stands in for
the image.

..  _accessibility-tips-media:

Play the video with the sound off
---------------------------------

If you cannot follow a video with the sound off, the captions or the
transcript are missing. Put a transcript in the text of the content element
and give it a heading. Ask your integrator how the player on your site
takes a captions file.

Leave automatic playback off. If a clip must start by itself and it lasts
more than three seconds, the visitor needs a way to pause it or to change
its volume separately from the device.

..  _accessibility-tips-color:

Check color and text saved as an image
--------------------------------------

"Required fields are shown in red" needs the word "required" as well.
A heading that is a picture, or a phone number that is a picture, should be
typed as text. A logo may stay an image. Its alternative text is the words
in the logo.

If you colored text in the editor, check the contrast.
`Success Criterion 1.4.3 <https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html>`__
requires a contrast ratio of at least 4.5:1. Large-scale text, at least 18
point or 14 point bold, needs at least 3:1. Text that is pure decoration,
inactive, or part of a logo has no contrast requirement under that
criterion. The colors of the theme are the integrator's. Low contrast was
the most common failure in the February 2026 WebAIM report: 83.9% of home
pages, with 34 instances on an average home page.

..  _accessibility-tips-forms:

Label every field
-----------------

Read the form with the placeholders ignored, because placeholders vanish
while someone types. Every field needs a visible label. Say the format when
it is easy to get wrong: "Date of arrival (DD.MM.YYYY)".

Trigger an error on purpose. The message should name the field and the
change. "Invalid input" does not. The W3C example of a message that names
the problem is "The password needs to include at least one number."

..  _accessibility-tips-tables:

Mark the header cells of a table
--------------------------------

A table of data needs header cells, not a bold first row. A screen reader
can then repeat the header as the reader moves across a row. The W3C
tutorial on `tables <https://www.w3.org/WAI/tutorials/tables/>`__ shows the
patterns, including tables with two headers. A layout that only uses a
table to place two pieces of text side by side is a question for your
integrator. Prefer two paragraphs or a list when the content is not a table.
