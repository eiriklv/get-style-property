# getStyleProperty - quick & dirty CSS property testing

[Original by @kangax](https://github.com/kangax/cft/blob/gh-pages/getStyleProperty.js) :heart_eyes: :zap: :star2:. See [perfectionkills.com/feature-testing-css-properties/](http://perfectionkills.com/feature-testing-css-properties/)

``` js
var transformProp = getStyleProperty('transform');
// returns WebkitTransform on Chrome / Safari
// or transform on Firefox, or MozTransform on old firefox

// then you can use it when setting CSS
element.style[ transformProp ] = 'translate( 12px, 34px )';

// or simply check if its supported
var supportsTranforms = !!transformProp;
```

## Install with package manager

Install with [Bower](http://bower.io) :bird:

``` bash
bower install get-style-property
```

Or [Component](http://github.com/component/component)

``` bash
component install desandro/get-style-property
```

## MIT License

getStyleProperty is released under the [MIT License](http://desandro.mit-license.org/).
