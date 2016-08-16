# normalize.css

<a href="https://github.com/necolas/normalize.css"><img
  src="https://necolas.github.io/normalize.css/logo.svg" alt="Normalize Logo"
  width="80" height="80" align="right"></a>

> A modern alternative to CSS resets

## Installation

* [NPM](http://npmjs.com): `npm install --save scales-utilities-normalize`
* [Bower](http://bower.io/): `bower install --save scales-utilities-normalize`

## Usage

No other styles should come before Normalize.css.

It is recommended that you include the `_normalize.scss` file as untouched library code.

## What does it do?

* Preserves useful defaults, unlike many CSS resets.
* Normalizes styles for a wide range of elements.
* Corrects bugs and common browser inconsistencies.
* Improves usability with subtle modifications.
* Explains what code does using detailed comments.

## Browser support

* Chrome (last two)
* Edge (last two)
* Firefox (last two)
* Firefox ESR
* Internet Explorer 8+
* Opera (last two)
* Safari 6+

*[Normalize.css v1 provides legacy browser support](https://github.com/necolas/normalize.css/tree/v1) (IE 6+, Safari 4+), but is no longer actively developed.*

## Extended details

Additional detail and explanation of the esoteric parts of normalize.css.


#### `pre, code, kbd, samp`

The `font-family: monospace, monospace` hack fixes the inheritance and scaling
of font-size for preformatted text. The duplication of `monospace` is
intentional. [Source](https://en.wikipedia.org/wiki/User:Davidgothberg/Test59).

#### `sub, sup`

Normally, using `sub` or `sup` affects the line-box height of text in all
browsers. [Source](https://gist.github.com/413930).

#### `svg:not(:root)`

Adding `overflow: hidden` fixes IE9's SVG rendering. Earlier versions of IE
don't support SVG, so we can safely use the `:not()` and `:root` selectors that
modern browsers use in the default UA stylesheets to apply this style. [Source]
(https://lists.w3.org/Archives/Public/public-svg-wg/2008JulSep/0339.html).

#### `select`

By default, Chrome on OS X and Safari on OS X allow very limited styling of
`select`, unless a border property is set. The default font weight on `optgroup`
elements cannot safely be changed in Chrome on OSX and Safari on OS X.

#### `[type="checkbox"]`

It is recommended that you do not style checkbox and radio inputs as Firefox's
implementation does not respect box-sizing, padding, or width.

#### `[type="number"]`

Certain font size values applied to number inputs cause the cursor style of the
decrement button to change from `default` to `text`.

#### `[type="search"]`

The search input is not fully stylable by default. In Chrome and Safari on
OSX/iOS you can't control `font`, `padding`, `border`, or `background`. In
Chrome and Safari on Windows you can't control `border` properly. It will apply
`border-width` but will only show a border color (which cannot be controlled)
for the outer 1px of that border. Applying `-webkit-appearance: textfield`
addresses these issues without removing the benefits of search inputs (e.g.
showing past searches). Safari (but not Chrome) will clip the cancel button on
when it has padding (and `textfield` appearance).

#### `::placeholder`

In Edge, placeholders will disappear on `relative` or `absolute` positioned
`<input>` elements if you use `opacity` less than `1` due to a [bug](https://developer.microsoft.com/en-us/microsoft-edge/platform/issues/3901363/).

## Contributing

Please read the [contribution guidelines](CONTRIBUTING.md) in order to make the
contribution process easy and effective for everyone involved.


## Acknowledgements

Normalize.css is a project by [Nicolas Gallagher](https://github.com/necolas),
co-created with [Jonathan Neal](https://github.com/jonathantneal).
