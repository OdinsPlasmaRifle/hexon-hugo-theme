---
date: 2018-09-17T15:21:22+02:00
title: Customize
description: Customize the hexon theme.
weight: 3
---

Hexon has many features that can be customized using the site's config file.

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

  extraNavItems:            # Extra navbar links
    - title: Log in
      url: https://example.com/login

  extraFooterItems:                     # Extra footer links
    - title: Log in
      url: https://example.com/login
```

Additional customization can be done by overiding the assets, layouts and other data in the normal Hugo manner.
