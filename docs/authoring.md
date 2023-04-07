---
title: How to create your own content?
section: Authoring
order: 5
---

## Authoring

In order to have a new page, create new markdown files in /docs.

Documents are written in markdown, following [CommonMark spec](http://spec.commonmark.org/) and must have a `.md` extension.

Simply add/modify files and it will appear in your documentation menu bar.

1. Create a new file
2. Edit your front matter with :
	- `title` : the title of your page
	- `section` : the section from the menu bar where this page should be listed
	- `order` : the order in the menu from the side bar
~~~
	---
	title: How to create your own content?
	section: Authoring
	order: 5
	---

## Title

Your content goes here

~~~

If you keep the main page, your own content should start with an `order: 2` page.
For your content, we suggest to start your title at level 2 eg. with markdown header `##`.
The template already add the `title` from the front matter as Header 1.

That's it !

