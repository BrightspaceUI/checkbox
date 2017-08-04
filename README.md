# d2l-checkbox
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/BrightspaceUI/checkbox)
[![Bower version][bower-image]][bower-url]
[![Build status][ci-image]][ci-url]

[Polymer](https://www.polymer-project.org)-based web component for D2L checkboxes.

![screenshot of checkbox component](/checkbox.gif?raw=true)

For further information on this and other Brightspace UI components, see the docs at [ui.developers.brightspace.com](http://ui.developers.brightspace.com/).

## Installation

`d2l-checkbox` can be installed from [Bower][bower-url]:

```shell
bower install d2l-checkbox
```

## Usage

Include the [webcomponents.js](http://webcomponents.org/polyfills/) "lite" polyfill (for browsers who don't natively support web components), then import `d2l-checkbox.html`:

```html
<head>
	<script src="bower_components/webcomponentsjs/webcomponents-lite.js"></script>
	<link rel="import" href="bower_components/d2l-checkbox/d2l-checkbox.html">
</head>
```

A `<d2l-checkbox>` custom element can now be used in your application. The label
for your checkbox should be placed inside the element:

```html
<d2l-checkbox>Label for checkbox</d2l-checkbox>
```

Many of the same attributes from native `<input type="checkbox">` are available:

```html
<d2l-checkbox checked>Checked checkbox</d2l-checkbox>
```

To hide the label when space is limited, use the `aria-label` attribute to
provide an accessible label:

```html
<d2l-checkbox aria-label="label for checkbox"></d2l-checkbox>
```

## Developing, Testing and Contributing

After cloning the repo, run `npm install` to install dependencies.

If you don't have it already, install the [Polymer CLI](https://www.polymer-project.org/2.0/docs/tools/polymer-cli) globally:

```shell
npm install -g polymer-cli
```

To start a [local web server](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#serve) that hosts the demo page and tests:

```shell
polymer serve
```

To lint ([eslint](http://eslint.org/) and [Polymer lint](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#lint)):

```shell
npm run lint
```

To run unit tests locally using [Polymer test](https://www.polymer-project.org/2.0/docs/tools/polymer-cli-commands#tests):

```shell
polymer test --skip-plugin sauce
```

To lint AND run local unit tests:

```shell
npm test
```

[bower-url]: http://bower.io/search/?q=d2l-checkbox
[bower-image]: https://badge.fury.io/bo/d2l-checkbox.svg
[ci-url]: https://travis-ci.org/BrightspaceUI/checkbox
[ci-image]: https://travis-ci.org/BrightspaceUI/checkbox.svg
