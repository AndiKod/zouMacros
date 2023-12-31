# zouMacros

Nunjucks macros to be imported in other projects, made for [Zou!JS](https://zoujs.vercel.app).

## Install

From NPM

```shell
npm i zoumacros --save-dev
```

### Modules

_...Obviously just a beginning, to start the collection._

## CDN Loader

It replace the call to the macro with the CDN links of the package. Path depends on the layout file calling it. When it comes to CSS frameworks, that's an easy quick way to prototype with and discover, yet installing the full SASS version when available a more powerfull way.

_In the head section of something like src/layouts/base.nkj:_

```
{% import '../../node_modules/zoumacros/lib/cdn.njk' as cdn; %}

{{ cdn.pkg('alpinejs') }}
```

_...and have fun._

## Available Packages

To kick-off the list, we have:

### CSS

- [chota](https://jenil.github.io/chota/#docs)
- [bulma](https://bulma.io/documentation/overview/classes/)
- [bonsai](https://www.bonsaicss.com/)
- [bootstrap](https://getbootstrap.com/docs/5.3/layout/containers/)
- [purecss](https://purecss.io/)
- [openprops](https://open-props.style/)
- [openprops-normalize](https://codepen.io/argyleink/pen/KKvRORE)
- [openprops-buttons](https://codepen.io/argyleink/pen/KKvRORE)
- [openprops-masks](https://open-props.style/#masks)
- [openprops-corners](https://open-props.style/#masks)

### Javascript

- [alpinejs](https://alpinejs.dev/essentials/state)
- [pocketbase](https://pocketbase.io/docs/)
- [hyperscript](https://hyperscript.org/docs/#basics)
- [htmx](https://htmx.org/docs/#ajax)

For SCSS, Tailwind, TS... just go Zou!

## Embed YouTube Video

It replace the shortcode with a responsive, container's full width iframe with the video corresponding to the provided ID.


_Anywhere in the template, generally on top:_

```
{% import '../../node_modules/zoumacros/lib/embed.njk' as embed; %}
```

_In the place where you want to place the video:_

```
{{ embed.yt('6-MlH1t8t9I') }}
```


#### Changelog

1.0.2: 
Hyperscript and htmX added to the CDN-loader marcro.

1.1.2: 
CutestrapCSS replaced by Chota in CDN-loader, as it wasn't an official CDN.

1.2.0: 
PureCSS & OpenProps familly added in CDN-loader

1.3.0:
Initiate a new Macro (embed) with YouTube videos. 
  