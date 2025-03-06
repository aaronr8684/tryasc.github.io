# Editing Guide

## Page content

To edit content for each page/post, just edit the corresponding *.md file. This is 90%+ of what you will be doing

### Header info

Each page contains header info surrounded by a set of `---`.

```markdown
---
layout: page
title: TITLE TEXT
header: POST TITLE TEXT
permalink: /page_url/
---
```

- `layout` - This is the template that will be used.
- `title` - This is the text that will be used for the link in the website header
- `header` - OPTIONAL: If present, it will be displayed at the top of the page/post
- `permalink` - url to use for the page

### Content
The rest of the page can be a mix of text formatted with markdown (preferred) and html (acceptable)

For markdown, see [this cheat sheet](https://www.markdownguide.org/cheat-sheet/)

For HTML, you can reference [W3Schools](https://www.w3schools.com/html/default.asp)

## Editing the navigation

Editing the navigation is a little more complicated than adding content. The nav bar always has the order of home first followed by external links and ending with content pages.

### Add markdown file to nav bar (new content)

1. __Add the markdown file__ - Before you edit the navigation, make sure you have created the new markdown file (*.md) already. Content is optional at this point

2. __Add the markdown to the navigation list__ - In the `_config.yml` file, find the `header_pages:` section.

3. __Add the markdown filename to the list__ - Add the file to the list in the order you want them to show up using the format `- filename.md`

### Add external link to nav bar

1. __Open the `static-links.html` file__ - It can be found in the `_includes\` folder.

2. __Add the link__ - Use the format `<a class="page-link" href="url">NAV TEXT</a>`

## Advanced formatting

Additional formatting and style changes can be done in the various other folders and files, but this should be considered advanced and can break the dynamic formatting if not done correctly. Proceed with caution.
