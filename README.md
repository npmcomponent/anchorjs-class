# Anchor/Class

The class module provides object-oriented programming techniques, including
inheritance and mixins, to the Anchor platform.

## Installation

###### Using volo

    $ volo add anchorjs/class

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
