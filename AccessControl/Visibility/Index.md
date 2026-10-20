---
title: "Elements visibility"
manual: "Tutorial for Editors"
version: "main"
permalink: "https://docs.typo3.org/permalink/t3editors:visibility@main"
source: "AccessControl/Visibility/Index.rst"
rendered: "2026-10-20T12:34:02+00:00"
---

# Elements visibility {#visibility}

When an element is hidden, be it a page, a content element or a news item, it
will not display in the frontend. You can, however, preview it in the backend.

In the Core, and in extensions that follow best practice, all options related
to visibility are controlled in the **Access** tab of the [page
properties](https://docs.typo3.org/permalink/t3editors:pages-properties@main).

## Publication dates {#visibility-dates}

You can specify a period of time for content to be visible. This might be
useful for seasonal announcements or festive periods.
Any page or content element with a defined **Publish Date**
will not be visible before that date. If it has an **Expiration
Date**, it will be hidden from that point onward.

![The publication dates of a page](../../Images/GeneratedScreenshots/AccessControl/PublicationDate.png)

When you set a publication date in the future then try to navigate to that
page, you are redirected to the home page.

When you enable the **Extend to Subpages** setting, the
publication date (and other access restrictions) also apply
to all child pages of the current page. This makes it possible
to apply restrictions to a whole branch of the page tree.
