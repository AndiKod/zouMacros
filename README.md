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

It replace the call to the macro with the CDN links of the package. Path depends on the layout file calling it.

```
{# some .njk layout, in the head section #}

{% import '../../node_modules/zoumacros/lib/cdn.njk' as cdn; %}
{{ cdn.pkg('bulma') }}
{{ cdn.pkg('alpinejs') }}
```

To kick-off the list, we have:

- Bulma
- BonsaiCSS
- Cutestrap
- Bootstrap

- AlpineJS
- PocketBase
