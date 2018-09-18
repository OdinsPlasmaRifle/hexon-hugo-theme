---
date: 2018-09-17T15:21:22+02:00
title: Create
description: Create a hexon content directory.
weight: 2
---

Use the following directory structure for your Hexon content:

```
content
	- _index.md
	- section 1
		- _index.md
		- subsection 1
			- _index.md
			- example.md
			- example2.md
		- subsection 1
			- _index.md
			- example.md
	- section 2
		- _index.md
		- subsection 1
			- _index.md
			- example.md
	- section 3
		- _index.md
		- subsection 1
			- _index.md
			- example.md
```

In short, make sure you divide your content up into sections and subsections. Hexon relies on this format to correctly display menus, navbars and other pages.

The weighting included in the `_index.md` files is important as it allows you to customize the order that the sections, sub sections and pages are displayed.