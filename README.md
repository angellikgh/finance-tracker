# finance-tracker

[![MIT license](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE.md)
[![dependencies Status](https://david-dm.org/inpercima/finance-tracker/status.svg)](https://david-dm.org/inpercima/finance-tracker)
[![devDependencies Status](https://david-dm.org/inpercima/finance-tracker/dev-status.svg)](https://david-dm.org/inpercima/finance-tracker?type=dev)

A simple finance tracker to manage incomes and expenses.

This project was generated with [swaaplate](https://github.com/inpercima/swaaplate) version 0.3.0-SNAPSHOT.

## Prerequisites

### Node, npm or yarn

* `node 8.11.3` or higher in combination with
  * `npm 5.6.0` or higher or
  * `yarn 1.7.0` or higher, used in this repository

### Angular CLI

* `angular-cli 7.1.4` or higher

## Getting started

```bash
# clone project
git clone https://github.com/inpercima/finance-tracker
cd finance-tracker

# install tools and frontend dependencies
cd client
yarn
```

## Usage

### Recommendation

It is recommanded to use a server to get full access of all angular.
You can do this for example with `yarn serve:mock`.
For the other options your app should run on a server which you like.

### DevMode with mock data

Start in a separate terminal a server with mock data, reachable on [http://localhost:3000/](http://localhost:3000/).

```bash
yarn run:mock
```

Chose one of the following to work in devMode with mock data.

```bash
# build, reachable on http://localhost/app/path/to/dist/
yarn build:mock

# build and starts a server, rebuild after changes, reachable on http://localhost:4200/
yarn serve:mock

# build, rebuild after changes, reachable on http://localhost/app/path/to/dist/
yarn watch:mock
```

### DevMode with real data, if present

```bash
# build, reachable on http://localhost/app/path/to/dist/
yarn build:dev

# build, rebuild after changes, reachable on http://localhost/app/path/to/dist/
yarn watch:dev
```

### ProdMode

```bash
# build in prodMode, compressed
yarn build:prod
```

### Tests

```bash
# test
ng test

# e2e
ng e2e
```

## Configuration

### General

All options have to bet set in the environment files but some of them do not need to be changed.
All defaults refer to the development environment file (`environment.ts`).
All deviations are described in addition as `mock` and `production`.

### Table of contents

* [activateLogin](#activateLogin)
* [api](#api)
* [apiSuffix](#apiSuffix)
* [appname](#appname)
* [defaultRoute](#defaultRoute)
* [production](#production)
* [redirectNotFound](#redirectNotFound)
* [showFeatures](#showFeatures)
* [showLogin](#showLogin)
* [theme](#theme)

### `activateLogin`

Defines whether a login will be used or not.

* default: `true`
* type: `boolean`
* values: `true`/`false`

### `api`

Defines the URL to the backend.

* default: `./api/` | mock: `http://localhost:3000/` | production: `./api/`
* type: `string`

### `apiSuffix`

Defines a suffix for the api to the backend.

* default: EMPTY
* type: `string`

### `appname`

Applicationwide title of the app, displayed in title and toolbar.

* default: `finance-tracker`
* type: `string`

### `defaultRoute`

The main route and the redirect route after login if no route is stored.

* default: `overview`
* type: `string`

### `production`

Defines whether the app is in production or not.

* default: `false` | mock: `false` | production: `true`
* type: `boolean`
* values: `true`/`false`

### `redirectNotFound`

Defines whether the 404 route will redirect to the default route or not.

* default: `false`
* type: `boolean`
* values: `true`/`false`

### `showFeatures`

Defines whether feature routes will be displayed or not.

* default: `true`
* type: `boolean`
* values: `true`/`false`

### `showLogin`

Defines whether login route will be displayed or not.

* default: `false`
* type: `boolean`
* values: `true`/`false`

### `theme`

Name of a build-in theme from angular-material.

* default: `pink-bluegrey`
* type: `string`
* values: `deeppurple-amber`/`indigo-pink`/`pink-bluegrey`/`purple-green`

Note: This option must also be changed in the angular.json if you want to change it.
