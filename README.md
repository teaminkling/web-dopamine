# Dopamine

A fork of the [Dope](https://dope.ghost.io) Ghost blogging theme for the Inkling Interactive marketing website.

This is the original tagline:

> A unique tag-based theme to arrange your publications into collections. Keep organized and let your readers explore
> your publications with ease. Completely free and fully responsive, released under the MIT license.

## Installation

Make sure you're using a production-ready version of Node (LTS).

1. Download the repository as a `.zip` file.
2. Log into Ghost, and go to the `Design` settings area to upload the zip file.

## Development

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
npm run zip
```

## Automatic Deployment

Go into your repository settings and set:

```yaml
api-url: ${{ secrets.GHOST_ADMIN_API_URL }}
api-key: ${{ secrets.GHOST_ADMIN_API_KEY }}
```

You will get a new deployment every time you tag and push `v<semver>` e.g., `v1.2.3`.

## PostCSS Features Used

- **Autoprefixer**: Don't worry about writing browser prefixes of any kind, it's all done automatically with support for
  the latest 2 major versions of every browser.

## Copyright & License

Copyright (c) 2013-2020 Ghost Foundation - Released under the [MIT license](LICENSE).
