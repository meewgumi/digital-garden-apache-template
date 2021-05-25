---
theme: Getting Started
---
## Vault
Open new folder as vault and select the main digital garden folder.

## Settings
### Files & Links
- Set default location for new notes to `_notes`
- Set default location for attachments to `assets`
- Set `Use Wikilinks` to `false`[^1]
	- Otherwise, images will be broken when you drag and drop to insert in a page
	- Don't worry, you can still create new Wikilinks manually

## Creating Wikilinks
When using Wikilinks, ensure that you're select the note in the `_notes` directory so the Jekyll build command works properly. Since we can't [ignore Obsidian folders yet](https://forum.obsidian.md/t/ignore-a-folder-of-temporary-notes/4473/8) and all images must be placed in `/assets`, unfortunately you'll just have to put up with the extra files for now.

## Suggested Plugins
### Templates
1. Under Core Plugins, enable "Templates"
2. Select `obsidian-templates` as the template folder
3. Set a hotkey for inserting a template to a file
4. Select note or page templates to insert front matter and variables


## Footnotes
[^1]: Currently, if you type the double bracket wikilink syntax within a code block, the bidirectional link generator renders it as an invalid link. Please refrain from using double brackets unless you're actually trying to link to a page.