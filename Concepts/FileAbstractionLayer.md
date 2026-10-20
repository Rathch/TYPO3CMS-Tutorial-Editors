---
title: "File abstraction layer (FAL)"
manual: "Tutorial for Editors"
version: "main"
permalink: "https://docs.typo3.org/permalink/t3editors:fal@main"
source: "Concepts/FileAbstractionLayer.rst"
rendered: "2026-10-20T12:56:18+00:00"
---

# File abstraction layer (FAL) {#fal}

TYPO3 has a file abstraction layer (FAL) integrated which abstracts technical
details (where the file is stored) and allows to work with different storage
forms.

FAL also allows the editors to manage meta data that can be displayed wherever
an asset is displayed. The metadata can also be used for
[copyright notices](https://docs.typo3.org/permalink/t3editors:copyright@main).

## Working with multi media: Digital asset management {#fal-working-multi-media}

Multi media **assets** (images, videos, audio, etc) are usually stored as
files on the server. Especially videos are frequently displayed from
third-party sources such as Youtube or Vimeo.

In TYPO3 you can manage all assets in the backend module
**Media** if you have sufficient permissions. See chapter
[Managing media in the TYPO3 CMS](https://docs.typo3.org/permalink/t3editors:managing-files@main).
