# RedisBundle ![project status](http://stillmaintained.com/snc/SncRedisBundle.png) #

## Forked and Fixed ##

We needed support for Predis 1.0, and more than one master connection. Upstream is very, very slow to merge fixes, and the current upstream master version has some potentially catastrophic bugs. So, we've merged a bunch of PRs from the upstream repo into this branch. Here are the details:

* [snc/SncRedisBundle#165](https://github.com/snc/SncRedisBundle/pull/165)
  * Fixes multiple connections with same alias overwriting other connections' parameters
  * Required to have any more than a single client with replication (because an alias of 'master' is required for replicated clients)
* [snc/SncRedisBundle#172](https://github.com/snc/SncRedisBundle/pull/172)
  * Adds support for Predis 1.0.x
* [snc/SncRedisBundle#186](https://github.com/snc/SncRedisBundle/pull/186)
  * Fix for [snc/SncRedisBundle#185](https://github.com/snc/SncRedisBundle/issues/185), which otherwise causes the database number to be ignored when using multiple persistent connections to the same host
* [snc/SncRedisBundle#187](https://github.com/snc/SncRedisBundle/pull/187)
  * Upgrades PHPUnit to stable
  * Inclues PHPUnit in the composer autoloader for ease of development
* [vend:feature-lower-loglevel](https://github.com/snc/SncRedisBundle/compare/705abcc...vend:feature-lower-loglevel)
  * Not opened as a PR, because it would require rebasing
  * Makes usage of the logger compatible with PSR3
* [vend/SncRedisBundle#2](https://github.com/vend/SncRedisBundle/pull/2)
  * Fixes memory leak in data collector/logger for production environments

We plan to say up to date with changes upstream. If you'd like to use this fork as a stable base for further development, you can suggest PRs for us to merge. (Either opening them here, or just by linking us to the upstream PR.)

## About ##

This bundle integrates [Predis](https://github.com/nrk/predis) and [phpredis](https://github.com/nicolasff/phpredis) into your Symfony2 application.

## Branches ##

* The `master` branch is the main supported branch. It is aliased as 2.0.x-dev and tagged as versions in the 3.0 range (to prevent version conflicts). It targets Predis 1.0 and newer versions of Symfony (at least >= 2.1.x).

## Documentation ##

[Read the documentation in Resources/doc/](https://github.com/snc/SncRedisBundle/blob/master/Resources/doc/index.md)

## License ##

See [Resources/meta/LICENSE](https://github.com/snc/SncRedisBundle/blob/master/Resources/meta/LICENSE).
