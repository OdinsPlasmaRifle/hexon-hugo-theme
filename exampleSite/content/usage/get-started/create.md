---
date: 2018-09-17T15:21:22+02:00
title: Create
description: Create a hexon content directory.
weight: 2
---

The Hexon `content` directory must follow a pre-defined structure.

In short, the `content` directory should contain a list of nested sections and sub-sections with weighted pages:

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

The above folder structure would create 3 menu items:

- Section 1
- Section 2
- Section 3

The title of each of these menu items is dictated by the `title` in the section's root `_index.md`. The order that the menu items appear is dictated by a `weight` variable in the `_index.md`. An example of this can be seen below:

```md
---
date: 2018-09-17T15:21:22+02:00
title: Section 1
description: Example section page.
weight: 1
---
```

Each section can then be seperated into further sub-sections and pages (that follow the same principles). This can be seen best by taking a look at the `exampleSite` in the theme.
