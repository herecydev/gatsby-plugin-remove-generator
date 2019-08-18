[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-green.svg?style=flat-square&logo=Github)](http://makeapullrequest.com)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg?style=flat-square)](https://github.com/tgallacher/gatsby-plugin-remove-generator/graphs/commit-activity)
![NPM version](https://img.shields.io/npm/v/gatsby-plugin-remove-generator.svg?style=flat)
![NPM license](https://img.shields.io/npm/l/gatsby-plugin-remove-generator.svg?style=flat)
[![Build Status](https://travis-ci.com/tgallacher/gatsby-plugin-remove-generator.svg?branch=master)](https://travis-ci.com/tgallacher/gatsby-plugin-remove-generator)

## Description

Gatsby plugin to remove the "generator" `<meta>` tag from your Gatsby site.

### Background

Gatsby auto injects a `<meta>` tag in the `<head>` of your site that indicates the Gatsby version used to build your site, for example.

```html
<meta name="generator" content="Gatsby 2.13.2" />
```

This is too much detail, for my taste, and also has potential security implications.

## Install

To add to your Gatsby setup, simply install

```sh
yarn add gatsby-plugin-remove-generator
```

and add to your config file:

> Note: The generator is only injected during a production build and so this plugin will only affect a production build.

```js
// gatsby-config.js
module.exports = {
  ...
  plugins: [
    'gatsby-plugin-remove-generator',
  ]
};
```
