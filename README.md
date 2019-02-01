# The Slate theme

[![Build Status](https://travis-ci.org/pages-themes/slate.svg?branch=master)](https://travis-ci.org/pages-themes/slate) [![Gem Version](https://badge.fury.io/rb/jekyll-theme-slate.svg)](https://badge.fury.io/rb/jekyll-theme-slate)

*Slate is a Jekyll theme for GitHub Pages. You can [preview the theme to see what it looks like](http://pages-themes.github.io/slate), or even [use it today](#usage).*

![Thumbnail of Slate](thumbnail.png)

## Usage

To use the Slate theme:

1. Add the following to your site's `_config.yml`:

    ```yml
    theme: jekyll-theme-slate
    ```

2. Optionally, if you'd like to preview your site on your computer, add the following to your site's `Gemfile`:

    ```ruby
    gem "github-pages", group: :jekyll_plugins
    ```

## Customizing

### Configuration variables

Slate will respect the following variables, if set in your site's `_config.yml`:

```yml
title: [The title of your site]
description: [A short description of your site's purpose]
```

Additionally, you may choose to set the following optional variables:

```yml
show_downloads: ["true" or "false" to indicate whether to provide a download URL]
google_analytics: [Your Google Analytics tracking ID]
```

### Stylesheet

If you'd like to add your own custom styles:

1. Create a file called `/assets/css/style.scss` in your site
2. Add the following content to the top of the file, exactly as shown:
    ```scss
    ---
    ---

    @import "{{ site.theme }}";
    ```
3. Add any custom CSS (or Sass, including imports) you'd like immediately after the `@import` line

*Note: If you'd like to change the theme's Sass variables, you must set new values before the `@import` line in your stylesheet.*

