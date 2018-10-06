[![Build Status](https://travis-ci.org/skumarsahistory/laraveltest.svg?branch=master)](https://https://travis-ci.org/skumarsahistory/laraveltest)

# laravel bolier plate with phpunit, jshint and codesniffer

## what does this do?
It will spin up a virtual machine inside travis and perform the following operations before we run any tests (via the before_script).

        Installs a linux operating system
        Installs PHP 7.2
        Runs composer on laravel and copies over the .env file
        Installs PHPCodeSniffer
        Updates Node to 7.7.1 and Npm to the latest version
        Installs JSHint
## Once the virtual machine is setup it will:

        Runs our unit tests and output a report on code coverage (should always be 100% right?)
        Runs PHPCodeSniffer and reports on any undocumented code or violations in coding standard (Laravel follows the PSR-2 coding standard and the PSR-4 autoloading standard)
        Compiles our assets (JS, SASS, CSS etc) using Laravel Mix
        Tests for any Javascript violations

