# Ruby

A multi-column [Ghost](https://github.com/TryGhost/Ghost) theme with a unique card layout. Make your publication more organized with cards and widgets.

**Demo: https://ruby.ghost.io**

# Instructions

1. [Download this theme](https://github.com/TryGhost/Ruby/archive/main.zip)
2. Log into Ghost, and go to the `Design` settings area to upload the zip file

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/), [Yarn](https://yarnpkg.com/) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's root directory:

```bash
# Install
yarn

# Run build & watch for changes
yarn dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/ruby.zip`, which you can then upload to your site.

```bash
yarn zip
```

# Contribution

This repo is synced automatically with [TryGhost/Themes](https://github.com/TryGhost/Themes) monorepo. If you're looking to contribute or raise an issue, head over to the main repository [TryGhost/Themes](https://github.com/TryGhost/Themes) where our official themes are developed.

# Copyright & License

Copyright (c) 2013-2023 Ghost Foundation - Released under the [MIT license](LICENSE).

# Code Injection

Site header

<style>
  
a.m-icon-button {
  display: none;
}
.m-heading {
    margin: 40px auto 40px;
    text-align: center;
}

.gh-article-meta {
    align-items: center;
    /* display: none; */
    gap: 8px;
    margin-left: 6px;
    margin-top: 20px;
}

.gh-article-image {
    grid-column: wide;
    margin-top: 40px;
    display: none;
}
  
</style>

Site footer

<style>

  .m-footer-copyright {
    display: none;
  }
    
  [data-theme=dark] {
    --footer-background-color: #111;
  }
  
  [data-theme=light] {
    --footer-background-color: #343a40;
  }
  
  .gh-footer-copyright {
      display: none;
  } 
  
</style>