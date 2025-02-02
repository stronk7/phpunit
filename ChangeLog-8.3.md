# Changes in PHPUnit 8.3

All notable changes of the PHPUnit 8.3 release series are documented in this file using the [Keep a CHANGELOG](http://keepachangelog.com/) principles.

## [8.3.0] - 2019-08-02

### Added

* Implemented [#3748](https://github.com/sebastianbergmann/phpunit/issues/3748): Add option to sort tests based on information from `@small`, `@medium`, and `@large`
* Added `TestCase::getActualOutputForAssertion()` as a wrapper for `TestCase::getActualOutput()` to prevent a test being marked as risky when it prints output and that output is not expected using `TestCase::expectOutputString()` or `TestCase::expectOutputRegEx()`

### Changed

* Implemented [#2015](https://github.com/sebastianbergmann/phpunit/issues/2015): Prefix all code bundled in PHAR distribution with random/unique namespace
* Implemented [#3503](https://github.com/sebastianbergmann/phpunit/issues/3503): The error handler has been refactored to not rely on global state
* Implemented [#3521](https://github.com/sebastianbergmann/phpunit/issues/3521): The `@errorHandler` annotation, which controlled a feature that was not documented and did not work correctly, does not have an effect anymore
* Implemented [#3522](https://github.com/sebastianbergmann/phpunit/issues/3522): The `TestCase::setUseErrorHandler()` method, which controlled a feature that was not documented and did not work correctly, has been deprecated and does not have an effect anymore

[8.3.0]: https://github.com/sebastianbergmann/phpunit/compare/8.2...8.3.0

