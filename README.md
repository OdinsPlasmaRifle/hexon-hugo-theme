# Hexon Hugo Theme

A minimal theme for multi-section documentation in [Hugo](https://gohugo.io).

![screenshot of hexon](https://github.com/odinsplasmarifle/hexon-hugo-theme/blob/master/images/screenshot.png?raw=true)

## Quick start

Navigate to your Hugo `themes` folder and install with `git`:

```sh
git clone git@github.com:OdinsPlasmaRifle/hexon-hugo-theme.git
```

or if you want to install within an existing git repository:

```sh
git submodule add git@github.com:OdinsPlasmaRifle/hexon-hugo-theme.git
```

## Usage

Take a look at the `exampleSite` folder within the theme. You can copy the whole folder's contents into your Hugo project or just the parts you want.

Once done you can run the Hugo development server:

```sh
hugo serve
```

You can then go to [localhost:1313](http://localhost:1313) to see the theme in action.

### Strcuture

Content in Hexon must follow a pre-defined structure.

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

## Customization

Hexon has many features that can be customized using the site config file.

An example configuration file can be found below:

```yaml
baseURL: "https://example.org/"
languageCode: "en-us"
title: "Hexon documentation"
theme: "hexon-hugo-theme"

params:
  logoUrl: https://example.com          # URL attached to the logo in the navbar.
  logoImage: /images/logo.png           # Image used for the logo in the navbar.
  heroImage: /images/hero.png           # Hero image used on the homepage.
  favicon: /images/favicon.png          # The site favicon

  primaryColor: "#33C3F0"               # Primary site color.
  secondaryColor: "#0FA0CE"             # Secondary site color.

  extraNavItems:						# Extra navbar links
    - title: Log in
      url: https://example.com/login

  extraFooterItems:                     # Extra footer links
    - title: Log in
      url: https://example.com/login
```

Additional customization can be done by overiding the assets, layouts and other data in the normal Hugo manner.
