<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

[circleci-image]: https://img.shields.io/circleci/build/github/nestjs/nest/master?token=abc123def456
[circleci-url]: https://circleci.com/gh/nestjs/nest

  <p align="center">A progressive <a href="http://nodejs.org" target="_blank">Node.js</a> framework for building efficient and scalable server-side applications.</p>
    <p align="center">
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/v/@nestjs/core.svg" alt="NPM Version" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/l/@nestjs/core.svg" alt="Package License" /></a>
<a href="https://www.npmjs.com/~nestjscore" target="_blank"><img src="https://img.shields.io/npm/dm/@nestjs/common.svg" alt="NPM Downloads" /></a>
<a href="https://circleci.com/gh/nestjs/nest" target="_blank"><img src="https://img.shields.io/circleci/build/github/nestjs/nest/master" alt="CircleCI" /></a>
<a href="https://coveralls.io/github/nestjs/nest?branch=master" target="_blank"><img src="https://coveralls.io/repos/github/nestjs/nest/badge.svg?branch=master#9" alt="Coverage" /></a>
<a href="https://discord.gg/G7Qnnhy" target="_blank"><img src="https://img.shields.io/badge/discord-online-brightgreen.svg" alt="Discord"/></a>
<a href="https://opencollective.com/nest#backer" target="_blank"><img src="https://opencollective.com/nest/backers/badge.svg" alt="Backers on Open Collective" /></a>
<a href="https://opencollective.com/nest#sponsor" target="_blank"><img src="https://opencollective.com/nest/sponsors/badge.svg" alt="Sponsors on Open Collective" /></a>
  <a href="https://paypal.me/kamilmysliwiec" target="_blank"><img src="https://img.shields.io/badge/Donate-PayPal-ff3f59.svg"/></a>
    <a href="https://opencollective.com/nest#sponsor"  target="_blank"><img src="https://img.shields.io/badge/Support%20us-Open%20Collective-41B883.svg" alt="Support us"></a>
  <a href="https://twitter.com/nestframework" target="_blank"><img src="https://img.shields.io/twitter/follow/nestframework.svg?style=social&label=Follow"></a>
</p>
  <!--[![Backers on Open Collective](https://opencollective.com/nest/backers/badge.svg)](https://opencollective.com/nest#backer)
  [![Sponsors on Open Collective](https://opencollective.com/nest/sponsors/badge.svg)](https://opencollective.com/nest#sponsor)-->

## Description

[Nest](https://github.com/nestjs/nest) framework TypeScript starter repository.

## Installation

```bash
$ npm install
```

## Running the app

```bash
# development
$ npm run start

# watch mode
$ npm run start:dev

# production mode
$ npm run start:prod
```

## Test

```bash
# unit tests
$ npm run test

# e2e tests
$ npm run test:e2e

# test coverage
$ npm run test:cov
```

## Support

Nest is an MIT-licensed open source project. It can grow thanks to the sponsors and support by the amazing backers. If you'd like to join them, please [read more here](https://docs.nestjs.com/support).

## Stay in touch

- Author - [Kamil Myśliwiec](https://kamilmysliwiec.com)
- Website - [https://nestjs.com](https://nestjs.com/)
- Twitter - [@nestframework](https://twitter.com/nestframework)

## License

Nest is [MIT licensed](LICENSE).


## Source
Udemy course
NestJS: The Complete Developer's Guide
Section6

This app is na true full application that really does anything. Instead, it is a very quick little side project, and the entire goal of this side project
is to get a really good understanding of how modules and dependency injection work together.

So the app is not really a lot of point to it.
It's just a simple demonstration.

It's a very small project that is going to kind of imitate a computer.
So every computer that you've ever used has a couple of different components inside of it.
A typical computer will have a CPU for processing data and a hard disk of sorts for storing data.
Both these devices are powered by a power supply.
So a power supply is what supplies electricity.
A typical computer will also have some other very common components inside of it, such as networking capabilities and Ram. So a form of memory and so on.
But we're not going to worry about those.

We're just going to model a very simple computer that is going to have a CPU, a disk and a power supply.
So let me show you how we are going to model this thing and how dependency injection is going to come into play.

In this project we make a separate module that serves or kind of models each different part of a computer.
So at the lowest level, we create the power module.
Inside the power module is a service called the Power Service.
The power service has a single method called supply power.
Then we create a module and a disk module which both have a service of their own.
A CPU and a disk can only work if they have power.
So we need to make sure that both the CPU module and the disk module have access to some code that we put together inside the power module.
Once we've got the CPU and the disk stuff put together, we're then going to make use of both those modules inside of our topmost module which calls the computer module.
So we have a very strict hierarchy here of modules.
The computer module depends upon CPU and disk and CPU and disk in turn depend upon the power module.
And in each of these different modules, there's exactly one service or controller for that matter,
that's going to rely upon some other service.
So that's the general goal.
Along the way, we're going to get a better idea of what modules are, why we use them,
and a really good idea of some rules around dependency injection.




