---
title: "Fonts"
type: docs
url: /fonts/
aliases: [/working-with-fonts/]
weight: 90
---

We support custom user's fonts while processing documents. To use this feature just add **fontsLocation** query parameter to resource URL. This parameter contains folder in filestorage, which will be used as fonts source. At the first time fonts will be downloaded from cloud storage and cached in memory. To reset this cache use cache resource.

- [Gets the List of Fonts](/gets-the-list-of-fonts/).
- [Reset Fonts Cache](/reset-fonts-cache/).
