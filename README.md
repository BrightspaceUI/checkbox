# d2l-checkbox
[![Bower version][bower-image]][bower-url]
[![Build status][ci-image]][ci-url]

[Polymer](https://www.polymer-project.org)-based web component and [Sass](http://sass-lang.com/) mixins for D2L checkboxes.

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
	<script src="../../webcomponentsjs/webcomponents-lite.js"></script>
	<link rel="import" href="../d2l-checkbox/d2l-checkbox.html">
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

[bower-url]: http://bower.io/search/?q=d2l-checkbox
[bower-image]: https://img.shields.io/bower/v/d2l-checkbox.svg
[ci-url]: https://travis-ci.org/BrightspaceUI/checkbox
[ci-image]: https://travis-ci.org/BrightspaceUI/checkbox.svg?branch=master
