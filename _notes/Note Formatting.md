---
theme: Getting Started
---

## Front Matter
At the top of each new note, you must include the triple dashes that make up Jekyll Front Matter.

````
---
---
````

## Note Title
The title of the `.md` file will automatically become the note title heading, rendered as an `<h1>`. Keeping this in mind, start your note content from `<h2>` or `##`.

### Title Override
Use variable `title:` in the front matter to create a note title that is different from the filename. 

```
---
title: A note about cats
---
```

In the example above, the filename is `cats.md` but the longer title shows up in the note's heading and `<title>`. See it live at [[cats]].

## Themes (aka Categories)
On the [[archive]] page, I've set it to automatically display all notes and their themes (if any). Think of a theme like a category without the chronological blog connotation. Inspired by [Low Tech Mag's Archive Page](https://solar.lowtechmagazine.com/archives.html).

Themes will also display underneath note title, if they are not null. Eventually I want to make a theme page to view all notes with common themes.