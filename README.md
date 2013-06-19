# Anchor/Class

The class module provides object-oriented programming techniques, including
inheritance and mixins, to the Anchor platform.

## Install

##### component

    $ component install anchorjs/class

##### volo

    $ volo add anchorjs/class

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

## Compatibility

[![browser support](https://ci.testling.com/anchorjs/class.png)](http://ci.testling.com/anchorjs/class)

##### component

This module uses the [AMD](https://github.com/amdjs/amdjs-api) format.  To
include in component builds, use [component-amd](https://github.com/jaredhanson/component-amd):

    component build -u component-amd

## Tests

To run tests in a browser, execute the Make target for the desired browser:

    $ make test-chrome
    $ make test-firefox
    $ make test-safari
    
Headless tests can be executed directly from a terminal:
    
    $ make test-phantomjs

## Credits

  - [Jared Hanson](http://github.com/jaredhanson)

## License

[The MIT License](http://opensource.org/licenses/MIT)

Copyright (c) 2012-2013 Jared Hanson <[http://jaredhanson.net/](http://jaredhanson.net/)>
