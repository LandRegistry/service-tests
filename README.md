[![Build Status](https://travis-ci.org/LandRegistry/service-tests.svg)](https://travis-ci.org/LandRegistry/service-tests)

# Service Tests

Tests for Land Registry microservices.

## Installing

Install all dependencies with [Bundler](http://bundler.io/):

    bundle install

# Running the tests

Export the necessary BasicAuth credentials to your environment before you start:

    export HTTPBASICAUTH_USERNAME='redacted'
    export HTTPBASICAUTH_PASSWORD='redacted'

Run the test tasks with [Rake](https://github.com/jimweirich/rake):

    rake # defaults to 'local'
    rake features:local
    rake features:devenv
    rake features:heroku

Or to run a specific feature:

    cucumber features/sample.feature

## Fixtures

You can add fixtures to [fixtures](fixtures/), or pull it from the web.

Add your fixture mappings to the [fixture mapping configuration](config/fixtures-lookup.txt).

## Example run output

![screenshot](http://i.imgur.com/iw1NMUo.png)
