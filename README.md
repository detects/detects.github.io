
# Detects

An GitHub organization of browser detects,
each within their own repository,
designed to be used with [normalize](https://github.com/normalize).
Visit https://github.com/detects for a list of all detects.

This organization is designed to be a more modular [Modernizr](https://github.com/Modernizr/Modernizr),
with each detect being its own module without using any global singleton.

## Usage

You can either use any as script tags:

```html
<script src="https://nlz.io/github/detects/css-calc/*/index.js"></script>
```

Or as ES6 modules:

```js
import 'https://nlz.io/github/detects/css-calc/*/index.js'
```

You may also point to these detects using any other GitHub proxy:

```html
<script src='https://cdn.rawgit.com/detects/css-calc/1.0.0/index.js'></script>
```

Keep in mind versioning.

## Design

Each are designed to be their own self-enclosed script,
allowing either `<script>` or module usage.
When creating a detect, assume that they are executed within a global scope.

Classes are also added to `<html>`,
prefixed with a `no-` if the feature is not supported,
just like Modernizr.

## Forks

Some detects will simply be forked from other detects.
See https://github.com/detects?query=+only%3Aforks+ for a full list.

There are a couple reasons for forks.
One of the major reasons is a lack of git tags.

## Contributing

If you wish to contribute, please let [me](https://twitter.com/jongleberry) know!
I only create the detects I specifically need.
