---
theme: 
title: 
---

## Pages vs Notes
Site content is separated into two main categories:
1. **Pages** are static pages such as `about.md`, saved in the root directory
2. **Notes** are your connected knowledge, saved in `_notes` directory

Both notes and pages support wikilinks. When you build your site, these markdown files are converted to html.

## Note Features
Since the notes are set up as a Jekyll collection rather than a post item, you cannot use built in category or tag features. The advantage of this is being able to name your note anything you want, rather than adhering to Jekyll's requirement to add the date to a post filename.

More info in [[Note Formatting]]

## Assets
All assets must be saved in the `assets` directory or they wil not be built by Jekyll.