# RedisBundle ![project status](http://stillmaintained.com/snc/SncRedisBundle.png) #

## Forked and Merged ##

We needed support for Predis 1.0, and more than one master connection. Upstream is very, very slow to merge fixes. So, we've merged a bunch of PRs from the upstream repo into this branch.

- https://github.com/snc/SncRedisBundle/pull/172
- https://github.com/snc/SncRedisBundle/pull/165


## About ##

This bundle integrates [Predis](https://github.com/nrk/predis) and [phpredis](https://github.com/nicolasff/phpredis) into your Symfony2 application.

## Branches ##

* Use version `1.0.*` or the `1.0` branch if you are using Symfony2 `2.0.*`. [![build status](https://secure.travis-ci.org/snc/SncRedisBundle.png?branch=1.0)](https://secure.travis-ci.org/snc/SncRedisBundle)
* Use version `1.1.*` or the `1.1` branch if you are using Symfony2 `>=2.1,<3.0`. [![build status](https://secure.travis-ci.org/snc/SncRedisBundle.png?branch=1.1)](https://secure.travis-ci.org/snc/SncRedisBundle)
* The `master` branch targets a new major version of this bundle and contains breaking changes. Use it at your own risk! [![build status](https://secure.travis-ci.org/snc/SncRedisBundle.png?branch=master)](https://secure.travis-ci.org/snc/SncRedisBundle)

This bundle is also available via [composer](https://github.com/composer/composer), find it on [packagist](http://packagist.org/packages/snc/redis-bundle).

## Documentation ##

[Read the documentation in Resources/doc/](https://github.com/snc/SncRedisBundle/blob/master/Resources/doc/index.md)

## License ##

See [Resources/meta/LICENSE](https://github.com/snc/SncRedisBundle/blob/master/Resources/meta/LICENSE).
