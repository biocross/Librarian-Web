---
layout: page
title: Quickstart Guide
permalink: /guide/
---

Welcome to Librarian's web interface! Your builds will be listed here to be downloaded.
It's currently showing sample data, but you can start submitting your real builds to librarian using the command:

~~~~
librarian submit <pathToIPA> [branch] [release_notes]
~~~

where,

* `pathToIPA` is the path to the IPA file
* `branch` is the git branch the build is from (**Optional**)
* `release_notes` are the release notes for the build (**Optional**)
