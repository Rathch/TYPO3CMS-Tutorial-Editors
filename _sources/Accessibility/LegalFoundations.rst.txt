..  include:: /Includes.rst.txt

..  _accessibility-legal:

==================
Legal requirements
==================

This page is not legal advice. The law that applies depends on the country,
on whether the organization is a public body, and on what the site sells or
provides. Ask the person responsible for the site which standard you must
meet. The W3C states the same limit on its own list of laws: it does not
make regulations, the list is not complete, and the entries are not legal
advice.

..  _accessibility-legal-wcag:

The guidelines laws point to
============================

The technical requirements usually point at the
`Web Content Accessibility Guidelines (WCAG) 2.1 <https://www.w3.org/TR/WCAG21/>`__,
or at a later edition. WCAG 2.1 is a W3C Recommendation. It is written as
testable statements, independent of a particular technology. Content that
conforms to WCAG 2.1 also conforms to WCAG 2.0. The W3C encourages the use
of the most current version when a policy is written or updated.
`WCAG 2.2 <https://www.w3.org/TR/WCAG22/>`__
is that later Recommendation.

WCAG groups the requirements into four principles. The wording below is a
short reading of those principles for an editor. The normative text is the
Recommendation.

*   **Perceivable.** People can take in the information. Text alternatives,
    captions, and contrast belong here.
*   **Operable.** People can use the page. Headings, page titles, and link
    text belong here, as does keyboard access, which is mostly the template.
*   **Understandable.** People can follow the page. The language, the
    labels, and the error messages belong here.
*   **Robust.** Assistive technologies can read the page. That is mostly
    the template and the code.

Each requirement has a level: A, AA, or AAA. Your organization names the
level that applies to the site. The
`W3C list of web accessibility laws and policies <https://www.w3.org/WAI/policies/>`__
shows which WCAG edition each listed policy refers to.

..  _accessibility-legal-eu:

European Union
==============

Two European directives cover a large part of what an editor publishes.
Each member state writes them into national law, so the national text is
the one that binds the organization.

`Directive (EU) 2016/2102 <https://eur-lex.europa.eu/eli/dir/2016/2102/oj>`__
is the directive on the accessibility of the websites and mobile
applications of public sector bodies. The
`W3C policy list <https://www.w3.org/WAI/policies/>`__
records it as an accessibility law for the public sector, based on
WCAG 2.1.

`Directive (EU) 2019/882 <https://eur-lex.europa.eu/eli/dir/2019/882/oj>`__,
the European Accessibility Act, sets accessibility requirements for
specified products and services. Member states had to adopt the national
measures by 28 June 2022 and apply them from 28 June 2025. The
`EUR-Lex summary of the Act <https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=legissum:4403933>`__
lists what is covered. For an editor, the relevant services include
e-commerce, consumer banking, e-books, and parts of passenger transport
such as websites, mobile services, and electronic tickets. The Act also
covers products such as computers, smartphones, e-readers, and certain
self-service terminals.

The Act does not cover every website. The summary names these exclusions,
among others:

*   Microenterprises that provide services.
*   Pre-recorded video and office files published before 28 June 2025.
*   Content of a website or app that is an archive, meaning it is not
    updated or edited after 28 June 2025.
*   Third-party content that the organization does not fund, develop, or
    control.

The Act itself is a list of accessibility requirements for those products
and services. It is not a sentence that says "use this WCAG version". The
version and the level come from the national law and from the standard
that law names. Ask which ones apply to your site.

..  _accessibility-legal-national:

Other countries
===============

Outside that European frame, and for the national text inside it, use the
`W3C list of web accessibility laws and policies <https://www.w3.org/WAI/policies/>`__.
The list has a last-updated date on each country. It includes, among many
others, non-discrimination laws and public-sector rules in the United
States, the United Kingdom, Canada, Australia, and Switzerland. If your
country is missing, or the entry looks old, the national authority is the
source to follow. The W3C asks to be told about additions and corrections.

..  _accessibility-legal-editor:

What this asks of an editor
===========================

A template can be accessible and the published page can still fail, because
the failure is in a field you control. These requirements from WCAG 2.1 are
the ones that match that work. The links go to the W3C explanation of each
requirement.

..  list-table:: WCAG 2.1 requirements an editor can meet in the content
    :header-rows: 1
    :widths: 28 12 60

    *   -   Requirement
        -   Level
        -   What you provide
    *   -   `Non-text content (1.1.1) <https://www.w3.org/WAI/WCAG21/Understanding/non-text-content.html>`__
        -   A
        -   Alternative text that carries the information of the image, or an empty alternative text when the image is decorative.
    *   -   `Audio-only and video-only (1.2.1) <https://www.w3.org/WAI/WCAG21/Understanding/audio-only-and-video-only-prerecorded.html>`__
        -   A
        -   A transcript for prerecorded audio, and a text alternative or audio alternative for prerecorded video that has no sound.
    *   -   `Captions (prerecorded) (1.2.2) <https://www.w3.org/WAI/WCAG21/Understanding/captions-prerecorded.html>`__
        -   A
        -   Captions for prerecorded video that has speech or meaningful sound.
    *   -   `Info and relationships (1.3.1) <https://www.w3.org/WAI/WCAG21/Understanding/info-and-relationships.html>`__
        -   A
        -   Headings, lists, and table headers marked as such, so the structure is in the content.
    *   -   `Use of color (1.4.1) <https://www.w3.org/WAI/WCAG21/Understanding/use-of-color.html>`__
        -   A
        -   Instructions that still work when the reader cannot see the color.
    *   -   `Contrast (minimum) (1.4.3) <https://www.w3.org/WAI/WCAG21/Understanding/contrast-minimum.html>`__
        -   AA
        -   Text you color yourself meets the contrast ratio. Theme colors belong to the integrator.
    *   -   `Images of text (1.4.5) <https://www.w3.org/WAI/WCAG21/Understanding/images-of-text.html>`__
        -   AA
        -   Real text for a sentence, a heading, or a price. A logo may stay an image.
    *   -   `Page titled (2.4.2) <https://www.w3.org/WAI/WCAG21/Understanding/page-titled.html>`__
        -   A
        -   A title that describes the topic of that page.
    *   -   `Link purpose in context (2.4.4) <https://www.w3.org/WAI/WCAG21/Understanding/link-purpose-in-context.html>`__
        -   A
        -   Link text that says where the link goes.
    *   -   `Headings and labels (2.4.6) <https://www.w3.org/WAI/WCAG21/Understanding/headings-and-labels.html>`__
        -   AA
        -   Headings and form labels that describe the topic or the field.
    *   -   `Language of page (3.1.1) <https://www.w3.org/WAI/WCAG21/Understanding/language-of-page.html>`__
        -   A
        -   The language of the page. An administrator sets this for the site. You choose the right translation when you edit one.
    *   -   `Language of parts (3.1.2) <https://www.w3.org/WAI/WCAG21/Understanding/language-of-parts.html>`__
        -   AA
        -   A phrase in another language is marked, when the editor allows it.
    *   -   `Labels or instructions (3.3.2) <https://www.w3.org/WAI/WCAG21/Understanding/labels-or-instructions.html>`__
        -   A
        -   A label on every field, and instructions where the format is not obvious.

How to write those fields is covered in
`Writing accessible text <https://docs.typo3.org/permalink/t3editors:accessibility-writing-accessible-text>`_.
A pass you can do on a finished page is in
`Tips and tricks <https://docs.typo3.org/permalink/t3editors:accessibility-tips>`_.
