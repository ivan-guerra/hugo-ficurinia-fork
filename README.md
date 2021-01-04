![logo](static/img/icon.svg)

# Ficurinia

A prickly blog theme for Hugo

![](images/tn.png)

# [Demo](https://gabmus.org)

[Code for the demo website](https://gitlab.com/gabmus/gabmus.gitlab.io) (really my personal website)

# Customization

## Configuration

These are some parameters you can use in your `config.toml` to customize Ficurinia:

```toml
theme = "hugo-ficurinia"

title = "My nice blog"
copyright = "Some copyright notice"

paginate = 5  # number of articles per page in the index


[params]
    logo = "/images/mylogo.png"
    favicon = "/images/myfavicon.png"
    showTags = true  # show the Tags menu item; default true
    showRss = true  # show the link for the RSS feed; default true

    navtype = "standard"  # changes the style of the pagination, available styles are: "standard", "circle"
    fontFamily = "JetBrains Mono"  # changes the font, default "JetBrains Mono"

    # enable comments support with commento using the script from your server
    commento = "https://example.com/js/commento.js"

    # enable analytics using Plausible
    plausibleScriptUrl = "https://something.com/..."
    plausibleDomain = "gabmus.org"

    # the links array shows links with icons (if explicitly supported)
    # it's an array of arrays containing two strings: name and link
    # the supported icons are:
    #    gitlab
    #    gnome
    #    youtube
    #    email
    #    twitter
    #    instagram
    #    facebook
    #    github
    #    linkedin
    #    telegram
    #    phone
    #    rss
    links = [
        ["GitLab", "https://gitlab.com/gabmus"],
        ["GNOME", "https://gitlab.gnome.org/gabmus"],
        ["YouTube", "https://youtube.com/TechPillsNet"],
        ["Email", "mailto:gabmus@disroot.org"]
    ]

    # you can customize all of the colors in this theme
    # the values shown are the defaults
    backgroundColor = "#242629"
    foregroundColor = "white"
    dimForegroundColor = "#bababa"
    strokeColor = "#4f4f4f"
    accentColor = "#db5793"
```

## Inject custom content

Ficurinia supports injecting custom content into the theme. There are several files you can create in `layouts/partials/inject` that will be included inside the theme in different places.

| Partial | Placement |
|---------|-----------|
| `layouts/partials/inject/body.html` | Before closing the `body` tag |
| `layouts/partials/inject/content-after.html` | After a post or page content |
| `layouts/partials/inject/content-before.html` | Before a post or page content |
| `layouts/partials/inject/footer.html` | At the beginning of the footer |
| `layouts/partials/inject/head.html` | Before closing the `head` tag |
| `layouts/partials/inject/header-after.html` | Before closing the header |
| `layouts/partials/inject/header-before.html` | At the beginning of the header |

# Does *Ficurinia* mean anything?

It's Sicilian for Indian fig, also known as prickly pear cactus.
