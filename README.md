# Anchor/Class

The class module provides object-oriented programming techniques, including
inheritance and mixins, to the Anchor platform.

## Install

##### volo

    $ volo add anchorjs/class

For more information on using volo to manage JavaScript modules, visit [http://volojs.org/](http://volojs.org/).

## Usage

#### Inheritance

To inherit a class from a subclass, invoke `inherits()`, passing the constructor
and super constructor as arguments.

```javascript
function Cat() {
  Cat.super_.call(this);
};

clazz.inherits(Cat, Animal);
```

#### Mixins

To augment a class with functions of a mixin object, invoke `augment()`.

```javascript
var HousePet = {
  eat: function() {},
  sleep: function() {}
}

clazz.augment(Cat, HousePet);
```

## Tests

##### Browser

To run tests in a browser, execute the Make target for the desired browser:

    $ make test-chrome
    $ make test-firefox
    $ make test-safari

##### PhantomJS

To run headless tests from a terminal using [PhantomJS](http://phantomjs.org/):

    $ make test-phantomjs

## Credits

  - [Jared Hanson](http://github.com/jaredhanson)

## License

[The MIT License](http://opensource.org/licenses/MIT)

Copyright (c) 2012-2013 Jared Hanson <[http://jaredhanson.net/](http://jaredhanson.net/)>
