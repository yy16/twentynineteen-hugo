# Twenty Nineteen Hugo

This is a Hugo port of WordPress's Twenty Nineteen theme.

## Highlights

- Accent color configurable via config.toml
- Featured images and image filter effect works
- Social menu icons all ported using Hugo's built-in menus
- Syntax highlighting included with the Monokai Light syntax theme

## Installation

From the root of your site:

`git submodule add https://github.com/jeremybise/twentynineteen-hugo.git themes/twentynineteen-hugo`

In your `config.toml`, add the following:

`theme = "twentynineteen-hugo"`

## Updating

From the root of your site:

`git submodule update --remote --merge`

## Differences from original theme

- Comment stuff has been omitted
- Author stuff has been omitted

## Content Notes

- To set a featured image for a post or page, add `image: /path/to/image.jpg` to your frontmatter.
- 

## Available Site Params

Some theme features can be configured in `config.toml`. Here are the options:

```toml
[params]
  accent_color = "#FF0000" # Set a custom accent color for links and image filters, if enabled. Defaults to blue.
  description = "This is the site tagline." # Adds tagline next to the site title.
  privacy_link = "/privacy/" # Relative URL to privacy page, if there is one. This enables a Privacy Policy link in the footer. The link doesn't display if this isn't specified.
  disable_image_filters = false # Setting to true disables the color filter feature on images. Defaults to false.
```

## Syntax Highlighting

Add pygments config to your `config.toml`:

```toml
pygmentsUseClasses=true
pygmentsCodefences=true
```

## Google Analytics

Add your Google Analytics Tracking Code ID to your `config.toml`:

```googleAnalytics = "UA-123-45"```

The asynchronous tracking script will be included on pages on the live server, but not the dev server.

## Roadmap

- [ ] Navigation menu dropdowns
- [ ] Include search via Lunr or Fuse