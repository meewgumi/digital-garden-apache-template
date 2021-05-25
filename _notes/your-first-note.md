---
title: Your first seed
theme: Getting Started
---

### Welcome!

This is your first note. You'll find it in the [`notes/`](https://github.com/maximevaillancourt/digital-garden-jekyll-template/tree/master/_notes) directory.

`.gitignore` is set to ignore Obsidian system files. I recommend setting Obsidian to automatically save attachments in the `/assets` folder.

### Link syntax

To link to another note, you can use multiple syntaxes. The following four use the "double-bracket" notation ([view the Markdown source file](https://github.com/maximevaillancourt/digital-garden-jekyll-template/blob/master/_notes/your-first-note.md#link-syntax) to see the underlying syntax).

- Using the note title: [[a note about cats]]
- Using the note's filename: [[cats]]
- Using the note's title, with a label: [[A note about cats|link to the note about cats using the note title]]
- Using the note's filename, with a label: [[cats|link to the note about cats using the note's filename]]

In all cases, if the double-bracket link does not point to a valid note, the double brackets will still be shown, like this: [[there is no note that matches this link]].

Alternatively, you can use regular [Markdown syntax](https://www.markdownguide.org/getting-started/) for links, with a relative link to the other note, like this: [this is a Markdown link to the note about cats](/cats){: .internal-link}. Don't forget to use the `.internal-link` class to make sure the link is styled as an internal link (without the little arrow).

Since the Web is all about HTML, you can always use plain HTML if you want, like this: <a class="internal-link" href="/cats">This is a link to the note about cats with HTML</a>.

Of course, you can also link to external websites, like this: [this is a link to Wikipedia](https://wikipedia.org/). Again, you can use plain HTML if you prefer. Footnotes are also supported and will be treated like internal links.[^1]

[^1]: This is a footnote. For more information about using footnotes, check out the [Markdown Guide](https://www.markdownguide.org/extended-syntax/#footnotes).

### Site configuration

Some behavior is configurable by tweaking the `_config.yml` file.

**`use_html_extension`**: if you use a static host that doesn't support URLs that don't end with `.html` (such as Neocities or Dreamhost), leave this as `true` in the `_config.yml` file. If you configure your `.htaccess` to remove extensions, remember to add `link` metadata for canonical URLs.

**`open_external_links_in_new_tab`**: when set to `true`, this makes external links open in new tabs. Set to `false` to open all links in the current tab.

**`baseurl`**: Set to your full web URL including `https://`

**`timezone`**: Set to your desired posting timezone so that the Last Modified At plugin displays the right date when you edit files.

### Pages
Save static pages in the root directory in `.md` format. Each page needs to have the following at the top:

```
---
layout: page
title: About
---
```

### Automatic bi-directional links

Notice in the "Notes mentioning this note" section that there is another note linking to this note. This is a bi-directional link, and those are automatically created when you create links to other notes.

### Link previews

If you're on a device with mouse support, try hovering your mouse on internal links to preview the notes: [[a note about cats]].

### Images and other Markdown goodies

Finally, because you have the full power of Markdown in this template, you can use regular Markdown syntax for various formatting options.

Lists work as expected:

- List element A
- List element B
- List element C

1. List element
2. List element
3. List element

If you'd like to quote other people, consider using quote blocks:

> Lorem ipsum dolor sit amet

And of course, images look great:

<img src="/assets/image.jpg"/>

### Code syntax highlighting

You can add code blocks with full syntax color highlighting by wrapping code snippet in triple backticks and specifying the type of the code (`js`, `rb`, `sh`, etc.):

```js
// Here's a bit of JavaScript:
console.log('hello!')
```

```rb
# And now some Ruby
def foo(bar)
  "baz"
end
```

```sh
$ cat /dev/urandom | grep "the answer to life" # shell scripts look nice too
```


### Next steps
To deploy via FTP or SSH, configure [Jekyll Build Commands](https://www.deployhq.com/guides/jekyll) and `vendor` caching on [DeployHQ](https://www.deployhq.com/r/nx7qct). Connect to your Github Repo and publish!

This digital garden template is free and open-source. It runs on Apache servers and the [Github code is available here](https://github.com/meewgumi/apache-digital-garden). This version of the code was modified by [Megumi Tanaka](https://megumi.co) in 2021.

Based on this [digital garden template](https://github.com/maximevaillancourt/digital-garden-jekyll-template), running on [Netlify](https://maximevaillancourt.com/blog/setting-up-your-own-digital-garden-with-jekyll), created by [Maxime Vaillancourt](https://github.com/maximevaillancourt).  [Buy the original creator a coffee](https://ko-fi.com/maximevaillancourt)! ☕️

Go forth, have fun, and learn new something every day! ✌️

### Footnotes
