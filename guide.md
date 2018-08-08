---
layout: page
title: Quickstart Guide
permalink: /guide/
---

### Submitting Builds

Submit builds to Librarian using:

```console
$ librarian submit <pathToFile> [options]
```
The `pathToFile` must be the full path to the `IPA` or `APK` file. Example: `/Users/jenkins/MyApp.ipa`, and should be accessible by Librarian.

You can pass in the following additional options along with the path of the build file.

Option | Short | Example | Description
--- | --- | --- | ---
`--branch <branch>` | `-b` | `--branch master` | git branch the build is from
`--notes <notes>` | `-n` | `--notes "Release Candidate Build"` | release notes for the build
`--public` | `-p` | Just add the flag `--public` | allow the build to be downloaded over the HTTPs tunnel (by default, builds can only be downloaded on the local network)

Librarian will autodetect the type of build `iOS / Android` using the file extension, will create a copy of the build in it's assets, and make it available for download on it's web interface.

> The Librarian server should be running while submitting a build.