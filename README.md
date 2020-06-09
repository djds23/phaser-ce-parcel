Phaser CE with Parcel
=====================

This is a [Phaser CE](https://www.npmjs.com/package/phaser-ce) game template using [Parcel](https://parceljs.org). Most common transformations ([CoffeeScript](https://parceljs.org/coffeeScript.html), [Babel/Flow](https://parceljs.org/javascript.html), [TypeScript](https://parceljs.org/typeScript.html)) work “out of the box”.

Use
---

```sh
# If you don't have Parcel, install it:
npm install -g parcel-bundler

# Clone or download this repo.
# From the project directory, install:
npm install

# Auto-compile and run dev server:
npm run start

# Compile for production:
npm run build
```

You can edit these scripts in [package.json](./package.json) to suit your needs. See:

- [Parcel: Getting Started](https://parceljs.org/getting_started.html)
- [Parcel: Production](https://parceljs.org/production.html)
- [Parcel: CLI](https://parceljs.org/cli.html)

Game assets
-----------

Static assets used in your JavaScript must be imported:

```javascript
import space from './assets/space.png'; // -> './space.89e3a46b.png'
// OR
import images from './assets/*.png'; // -> { space: './space.89e3a46b.png', … }
```

See [LoadState](./src/LoadState.js) for an example.

If you prefer, you can [use a plugin to copy static assets](https://www.npmjs.com/search?q=parcel%20plugin%20copy) instead.

Hot reload
----------

When running the dev server the game is destroyed and then recreated after you save changes to your files. Rarely, this can fail. Just refresh the browser.

If you don't like [hot reload](https://parceljs.org/hmr.html) at all, you can turn it off:

```sh
parcel serve src/index.html --no-hmr
```

