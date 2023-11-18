# zouMacros

Nunjucks macros to be imported in other projects, made for Zou!JS.

## Install

From NPM

```shell
npm i zoumacros --save-dev
```

### Modules

_...obviously just a beginning, to start the collection._

## CDN Loader

It replace the call to the macro with the CDN links of the package. Path depends on the layout file calling it. When it comes to CSS frameworks, that's an easy quick way to prototype with and discover, yet installing the full SASS version when available a more powerfull way.

Anyway, have fun.

```
{# some .njk layout, in the head section #}

{% import '../../node_modules/zoumacros/lib/cdn.njk' as cdn; %}
{{ cdn.pkg('bulma') }}
{{ cdn.pkg('alpinejs') }}
```

## Available Packages

To kick-off the list, we have:

### CSS

- [Bulma](https://bulma.io/documentation/overview/classes/)
- [BonsaiCSS](https://www.bonsaicss.com/)
- [Cutestrap](https://www.cutestrap.com/)
- [Bootstrap](https://getbootstrap.com/docs/5.3/layout/containers/)

### Javascript

- [AlpineJS](https://alpinejs.dev/essentials/state)
- [PocketBase](https://pocketbase.io/docs/)
- [hyperscript](https://hyperscript.org/docs/#basics)
- [htmx](https://htmx.org/docs/#ajax)

For SCSS, Tailwind, TS... just go Zou!

#### Changelog

1.0.2
Hyperscript and htmX added
