# Dopamine

A fork of the [Dope](https://dope.ghost.io) Ghost blogging theme for the Inkling Interactive marketing website.

This is the original tagline:

> A unique tag-based theme to arrange your publications into collections. Keep organized and let your readers explore
> your publications with ease. Completely free and fully responsive, released under the MIT license.

# Installation

1. Download the repository as a `.zip` file.
2. Log into Ghost, and go to the `Design` settings area to upload the zip file.

# Development

Styles are compiled using Gulp/PostCSS to polyfill future CSS spec. You'll need [Node](https://nodejs.org/),
[Yarn](https://yarnpkg.com/) (or NPM) and [Gulp](https://gulpjs.com) installed globally. After that, from the theme's 
root directory:

```bash
npm install
npm run dev
```

Now you can edit `/assets/css/` files, which will be compiled to `/assets/built/` automatically.

The `zip` Gulp task packages the theme files into `dist/<theme-name>.zip`, which you can then upload to your site.

```bash
yarn zip
```

# PostCSS Features Used

- **Autoprefixer**: Don't worry about writing browser prefixes of any kind, it's all done automatically with support for
  the latest 2 major versions of every browser.

# Copyright & License

Copyright (c) 2013-2020 Ghost Foundation - Released under the [MIT license](LICENSE).
