# Docker PHP CI

<!-- [![docker pull quay.io/pantheon-public/php-ci](https://img.shields.io/badge/image-quay-blue.svg)](https://quay.io/repository/pantheon-public/php-ci) -->

This is the source Dockerfile for the [pantheon-public/php-ci](https://quay.io/repository/pantheon-public/php-ci) docker image.

## Usage
In CircleCI 2.0:
```
  docker:
<<<<<<< HEAD
    - image: mrobit/php-ci:2.x
=======
    - image: quay.io/pantheon-public/php-ci:latest
>>>>>>> 281af183977640fb4454130da6f3fab1199b6cb8
```
## Image Contents

- [PHP 7.2](https://github.com/drupal-docker/php/tree/master/7.2)
- [Terminus](https://github.com/pantheon-systems/terminus)
- [circle-cli](https://github.com/circle-cli/circle-cli) test tool
- Node.js
- Yarn

Note that this image does not include any Terminus extensions. See [build-tools-ci image](https://github.com/pantheon-systems/docker-build-tools-ci) for a more complete Docker image pre-populated with a number of useful Terminus plugins. To test a Terminus plugin, use [pantheon-public/terminus-plugin-test](https://quay.io/repository/pantheon-public/terminus-plugin-test).

