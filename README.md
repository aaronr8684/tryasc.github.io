# Editing Guide

## Updating Page Content

Most of your updates will involve editing individual **Markdown (`.md`) files**. This covers **90%+** of the changes you'll make.

### Page Header Information

Every page starts with a **YAML front matter section**, enclosed by `---`.

#### Example:
````markdown
---
layout: page
title: TITLE TEXT
header: POST TITLE TEXT
permalink: /page_url/
---
````

#### Header Fields Explained:
- **`layout`** – Defines which template to use.
- **`title`** – Appears as the link text in the navigation menu.
- **`header`** – *(Optional)* Displays a title at the top of the page.
- **`permalink`** – Sets the page’s URL.

### Writing Content

The body of the page should be written in **Markdown** (preferred) or **HTML** (acceptable).

- **For Markdown formatting**, refer to the [Markdown Cheat Sheet](https://www.markdownguide.org/cheat-sheet/).
- **For HTML basics**, check out [W3Schools](https://www.w3schools.com/html/default.asp).

---

## Adding Updates to the Home Page

The `updates.md` file manages the **updates section** on the homepage.
- If this file is empty, the updates section is **hidden**.
- Only **updates** should be included—**do not** manually add an "Updates" header (it’s built into the template).

### Formatting Notes:
- Unlike other Markdown pages, `updates.md` **does not fully convert Markdown to HTML**, so **use minimal formatting**.
- **Links are supported** using either:
````markdown
[text](https://example.com)
````
or
````html
<a href="https://example.com">text</a>
````

- External links should **always** include `http://` or `https://`.

---

## Editing the Navigation

The navigation menu follows a fixed order:
1. **Home Page**
2. **External Links**
3. **Content Pages**

### Adding a Markdown Page to the Navbar

1. **Create the Markdown File** – Make sure the `.md` file exists before updating navigation.
2. **Edit `_config.yml`** – Locate the `header_pages:` section.
3. **Add the Page to the List** – Insert the filename in the correct order:
````yaml
header_pages:
  - filename.md
````

### Adding an External Link to the Navbar

1. **Open `static-links.html`** – This file is in the `_includes/` folder.
2. **Insert the New Link** – Use this format:
````html
<a class="page-link" href="URL">NAV TEXT</a>
````

---

## Advanced Formatting

For additional styling or layout modifications, you may need to edit files in other directories.
⚠️ **Proceed with caution**—modifying these files incorrectly can break the site’s structure.

---

This guide should help you update and manage the site’s content. If you have any questions, feel free to reach out! 🚀
