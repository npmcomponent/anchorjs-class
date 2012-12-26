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

Tests for Anchor/Class are executed using [Mocha](http://visionmedia.github.com/mocha/)
as a test framework with [Chai](http://chaijs.com/) assertions.

##### Dependencies

Prior to running tests, use [volo](https://github.com/volojs/volo) to fetch
dependencies from GitHub.

    $ cd tests
    $ volo add

##### Browser

To run tests in a browser, open _runner.html_:

    $ make test-browser

##### PhantomJS

To run headless tests from a terminal using [PhantomJS](http://phantomjs.org/):

    $ make test-phantomjs
