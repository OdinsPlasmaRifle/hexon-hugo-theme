---
date: 2018-09-17T15:21:22+02:00
title: Customize
description: Customize the hexon theme.
weight: 3
---

There are a range of customizable values that can be defined in your Hugo config file. An example config can be found below:

```
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