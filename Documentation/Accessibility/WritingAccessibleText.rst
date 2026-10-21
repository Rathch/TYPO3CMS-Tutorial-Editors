..  include:: /Includes.rst.txt

..  _accessibility-writing-accessible-text:

=======================
Writing accessible text
=======================

The W3C collects the writing practices on
`Writing for Web Accessibility <https://www.w3.org/WAI/tips/writing/>`__.
The sections below follow that page and name the TYPO3 field for each
practice. The examples are illustrations of the wording. They are not
records from a particular site.

..  _accessibility-writing-accessible-text-provide-informative-unique:

Provide informative, unique page titles
=======================================

`Success Criterion 2.4.2 <https://www.w3.org/WAI/WCAG21/Understanding/page-titled.html>`__
requires a title that describes the topic or purpose of the page. A person
using a screen reader hears the title first. The same title is the label of
the browser tab, so a row of tabs stays usable when several pages of the
site are open.

Set the :guilabel:`Page title` in the
`page properties <https://docs.typo3.org/permalink/t3editors:pages-properties-titles>`_.
If the page has a
`Title for search engines <https://docs.typo3.org/permalink/t3editors:title-for-search-engines>`_,
that value is the document title. When it is empty, TYPO3 uses the page
title. By default the site name is added as a suffix, separated by a dash.
An integrator can change that pattern. Ask when you need the title to follow
a fixed order.

Put the part that distinguishes this page first. The W3C's own examples use
a page name, then the organization, and they include the step when a page
is one step of a process.

..  list-table:: Page titles, following the W3C examples
    :header-rows: 1
    :widths: 40 60

    *   -   Situation
        -   Title
    *   -   A page whose title is only the organization
        -   Camino
    *   -   The page name first, then the organization
        -   Pilgrim stories - Camino
    *   -   One step of a process
        -   Book a bed (step 1 of 3) - Camino

"Camino" on its own fits the home page. It does not tell anyone which inner
page is open. "Page 3" and "News" have the same problem when the site has
many news pages: add the topic, for example "Route closed in March - News".

..  _accessibility-writing-accessible-text-headings-convey-meaning:

Use headings to convey meaning and structure
============================================

`Success Criterion 2.4.6 <https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html>`__
asks for headings that describe the topic. Screen reader users jump from
heading to heading. A heading that exists only because it looks larger is
missing from that list, and a heading that was styled to look small is
still announced as a heading. The W3C tutorial on
`headings <https://www.w3.org/WAI/tutorials/page-structure/headings/>`__
shows a heading outline.

Almost every content element can have a heading. When your permissions
allow it, set the level under :guilabel:`Headlines > Type`. Pick the level
from the outline of the page. A subsection sits one level under the section
it belongs to.

The
`rich text editor <https://docs.typo3.org/permalink/t3editors:rte>`_
can insert headings too. Use those for the structure inside the text. Use
the content element heading for the title of the element. Two headings with
the same wording, one on the element and one inside the text, give the
reader the same entry twice.

In the WebAIM Million report of February 2026, skipped heading levels were
present on 41.8% of home pages, and 18.1% had more than one level-1 heading.
How your site turns the page title into a heading depends on the site
package. Ask your integrator whether the page title is already the level-1
heading. If it is, the first content element heading is level 2.

Example. A page "Pilgrim stories" contains one story and a practical note:

*   Level 1: Pilgrim stories. This may already be the page title.
*   Level 2: The night at the mountain hut.
*   Level 3: How to get there.
*   Level 2: What to pack.

A level-4 heading directly under the page title leaves a gap. The size of
the type is a design decision. If a level-2 heading looks too large, ask
your integrator to adjust the stylesheet. Changing the stored level to
level 4 would break the outline.

..  _accessibility-writing-accessible-text-make-link-text:

Make link text meaningful
=========================

`Success Criterion 2.4.4 <https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html>`__
requires that the purpose of a link can be determined from the link text,
together with its context. People who list all the links on a page hear the
link text alone. "Click here" and "Read more" then become a list of links
that all sound the same. In the February 2026 WebAIM report, 15.2% of home
pages had link text of that kind.

When you
`create a link in the rich text editor <https://docs.typo3.org/permalink/t3editors:rte-linking>`_,
write the words that say where the link goes, select those words, and then
open the link dialog. If you insert a link without selecting text, TYPO3
uses the title of the link, or the title of the target. Read that inserted
text. A page title can be a good link name. A file name such as
``scan-final-v3.pdf`` is a poor one.

The W3C contrasts a link that says "click here" with a sentence that names
the destination. The same pattern:

*   Weak: For the route, click here.
*   Clear: Read the route over the pass.

When the target is a file, include the type and, if you know it, the size.
The W3C example is "Proposal Documents (RTF, 20MB)". A TYPO3 equivalent is
"Route description (PDF, 1 MB)".

A heading of a content element can itself be the link. The heading text is
then the link text, so the heading has to name the destination.

A linked image uses the alternative text as its accessible name when the
image has no other text. In the WebAIM report, 45% of images with no
alternative text were links. Write the alternative text as the name of the
destination: "Route description (PDF)", for a linked cover image.

..  _accessibility-writing-accessible-text-write-meaningful-text:

Write meaningful text alternatives for images
=============================================

`Success Criterion 1.1.1 <https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html>`__
requires a text alternative for non-text content. The W3C's writing guide
puts it this way: the alternative text provides the information or the
function of the image. A decorative image needs no alternative text. The
W3C tutorial on
`images <https://www.w3.org/WAI/tutorials/images/>`__
separates informative, decorative, and functional images. A short practical
guide is `Alt-texts: The Ultimate Guide <https://axesslab.com/alt-texts/>`__,
from Axess Lab.

In the :guilabel:`Media` module, edit the
`file metadata <https://docs.typo3.org/permalink/t3editors:file-metadata>`_
and fill in the alternative text there. That text is the default wherever
the file is used. When you place the image in a content element, you can
`override the alternative text <https://docs.typo3.org/permalink/t3editors:override-image-metadata>`_
for that one use. A portrait in the media library might have the alternative
text "Portrait of the hut warden". On a page about winter opening hours, the
same file might need "Hut warden at the counter where winter hours are posted".

The W3C shows the difference with a photo of someone charging a phone. The
weak alternative text is "Charging phone". The useful one describes the step
the photo is there to teach: "Plug cable into the bottom edge of the phone."
The same test, applied to a route page:

*   Weak: hut.jpg
*   Weak: image
*   Useful, when the photo carries the information: Wooden signpost for the
    mountain hut, 2 hours.
*   Empty, when the photo only decorates a paragraph that already says all
    of this.

Describe the information. Skip "image of" and "photo of". The screen reader
already announces that it is an image.

An alternative text is usually not visible on the page. The
:guilabel:`Description` is a different field. Themes often show the
description under the image, where everyone can read it. The alternative
text replaces the image for someone who cannot see it. The description adds
something for everyone. They should not be copies of each other when the
description is visible, or the reader hears the same sentence twice.

For a decorative image, leave the alternative text empty so assistive
technologies can skip it. If your installation will not store an empty
value, ask your integrator how decorative images are marked.

Text that matters belongs in the text field.
`Success Criterion 1.4.5 <https://www.w3.org/WAI/WCAG21/Understanding/images-of-text.html>`__
requires real text when the same visual result can be achieved with text.
A heading saved as a picture, or a price saved as a picture, cannot be
resized as text and has no alternative unless you write one. A logo is an
allowed exception. Its alternative text is the name in the logo.

..  _accessibility-writing-captions:

Provide transcripts and captions
================================

The W3C writing guide asks for a transcript of audio-only content, such as
a podcast, and captions for video that has a soundtrack. The transcript and
the captions include the spoken words and the sounds that carry meaning.
The W3C examples of those sounds are "door creaks" and, in a video
transcript, a description of an action such as someone leaving the room.
The requirements are
`Audio-only and video-only (1.2.1) <https://www.w3.org/WAI/WCAG21/Understanding/audio-only-and-video-only-prerecorded.html>`__
and
`Captions, prerecorded (1.2.2) <https://www.w3.org/WAI/WCAG21/Understanding/captions-prerecorded.html>`__.

You can place the transcript in the text of a
`Text & Media <https://docs.typo3.org/permalink/t3editors:media>`_
element, next to the video. Give it a heading, for example "Transcript", so
it can be found from the heading list.

Example, a short clip in which a warden speaks and a door closes::

    Warden: The pass is closed until Friday.
    [The hut door closes.]
    Warden: Use the valley path.

How captions are attached depends on the player your site uses. The core
manual for editors does not document a captions field on the media element.
Ask your integrator which file to upload, or which field the player reads.
A transcript in the text still helps when the captions file is missing, and
it helps people who cannot play the video.

`Success Criterion 1.4.2 <https://www.w3.org/WAI/WCAG21/Understanding/audio-control.html>`__
requires a way to pause or stop audio that plays automatically for more
than three seconds, or a volume control independent of the system volume.
Leave :guilabel:`Autoplay` off unless you have that control. The setting is
described in
`Configure the video <https://docs.typo3.org/permalink/t3editors:configure-the-video>`_.

..  _accessibility-writing-instructions:

Provide clear instructions
==========================

`Success Criterion 3.3.2 <https://www.w3.org/WAI/WCAG21/Understanding/labels-or-instructions.html>`__
requires labels or instructions when the content asks the user for input.
The W3C example of an instruction that states the rule is: "Password should
be at least six characters with at least one number (0-9)." An error should
say what is wrong. The W3C examples are "The username 'superbear' is already
in use." and "The password needs to include at least one number."

When you build a form in the
`Forms module <https://docs.typo3.org/permalink/t3editors:mail-form>`_,
the label is the accessible name of the field. "Name" is weaker than
"Your name" only in tone. "Field 1" is a failure. Placeholder text inside
the field disappears while the person types, so it does not replace the
label.

State the format next to the field when a reader cannot guess it:

*   Date of arrival (DD.MM.YYYY)
*   Phone number, including the country code

If the form shows an error, write the message so it names the field and the
change. "Check your input" leaves the reader to try every field.
"Date of arrival uses the form DD.MM.YYYY" names the fix.

..  _accessibility-writing-clear-language:

Keep content clear and concise
==============================

The W3C recommends short sentences, familiar words, abbreviations expanded
on first use, and lists where a list is the structure of the information.
The criteria behind that advice include
`Unusual words (3.1.3) <https://www.w3.org/WAI/WCAG21/Understanding/unusual-words.html>`__,
`Abbreviations (3.1.4) <https://www.w3.org/WAI/WCAG21/Understanding/abbreviations.html>`__,
and
`Reading level (3.1.5) <https://www.w3.org/WAI/WCAG21/Understanding/reading-level.html>`__.
Reading level is level AAA. Clear sentences still help at every level. The
W3C page links onward to guidance for people with cognitive and learning
disabilities, under the heading "Use clear and understandable content".

Expand an abbreviation the first time you use it: "Web Content
Accessibility Guidelines (WCAG)". A second mention can be "WCAG" alone.

Example. A sentence written to sound official:

"Utilization of the contact form is mandatory for the submission of all
inquiries pertaining to group visits."

The same instruction:

"To ask about a group visit, use the contact form."

A list is easier to scan than a sentence of options. "You can get there by
bus, by the valley path, or by booking the hut taxi" can be three items
when each option needs its own detail.

`Success Criterion 1.4.1 <https://www.w3.org/WAI/WCAG21/Understanding/use-of-color.html>`__
says that color is not the only means of conveying the information. "Fields
in red are required" excludes a reader who cannot see the red. Add the word
"required" to the label.

`Success Criterion 1.3.1 <https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html>`__
requires the structure to be in the markup. In the rich text editor, use
the list buttons for a list, and mark the header row when you insert a
table. A bold first row that is not a header is only bold. The W3C tutorial
on `tables <https://www.w3.org/WAI/tutorials/tables/>`__ shows header cells.
