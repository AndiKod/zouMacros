# zouMacros

Nunjucks macros to be imported in other projects, made for Zou!JS.

## Install

From NPM

```shell
npm i zoumacros --save-dev
```

### Modules

_...Obviously just a beginning, to start the collection._

## CDN Loader

It replace the call to the macro with the CDN links of the package. Path depends on the layout file calling it. When it comes to CSS frameworks, that's an easy quick way to prototype with and discover, yet installing the full SASS version when available a more powerfull way.

_In the head section of a layout/page:_

```
{% import '../../node_modules/zoumacros/lib/cdn.njk' as cdn; %}
{{ cdn.pkg('chota') }}
{{ cdn.pkg('hyperscript') }}
```

_...and have fun._

## Available Packages

To kick-off the list, we have:

### CSS

- [Chota](https://jenil.github.io/chota/#docs)
- [Bulma](https://bulma.io/documentation/overview/classes/)
- [BonsaiCSS](https://www.bonsaicss.com/)
- [Bootstrap](https://getbootstrap.com/docs/5.3/layout/containers/)

### Javascript

- [AlpineJS](https://alpinejs.dev/essentials/state)
- [PocketBase](https://pocketbase.io/docs/)
- [hyperscript](https://hyperscript.org/docs/#basics)
- [htmx](https://htmx.org/docs/#ajax)

For SCSS, Tailwind, TS... just go Zou!

#### Changelog

1.0.2
Hyperscript and htmX added to the CDN-loader marcro.

1.1.2
CutestrapCSS replaced by Chota in CDN-loader, as it wasn't an official CDN.
