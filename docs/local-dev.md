---
title: Local development
section: Publish your content
order: 3
---

## Before you start

For local development, you need to install first git, node.js and npm.

Follow the instruction on:
- Git
	+ Download the distribution for your platform from [Download git](https://git-scm.com/download/) and follow the platform specific instructions.
	+ Read the documentation for the original setup [First Time Git Setup](https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup)

- node.js and npm:
	+ Follow the instruction on [npm setup](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) to install both node.js and npm
	+ Alternatively, download the distribution for your platform from [Download node.js](https://nodejs.org/en/download) and follow the platform specific instructions.

- Should you work also on hosted site (like with Netlify) ensure your git cli configuration is working properly with Github.
	+ [git cli setup for GitHub](https://docs.github.com/en/get-started/quickstart/set-up-git)


## Install eleventy

~~~
npm install @11ty/eleventy --save-dev
~~~

## Install tailwind

https://tailwindcss.com/docs/installation


## Getting started

1. Clone this repository

```shell
git clone https://github.com/per1/11ty documentation
```

2. Go into this new folder

```shell
cd documentation
```

3. Install dependencies

```shell
npm install
```


### Development

```shell
npm run dev
```


### Production

```shell
npm run build
```


### Configuring

To change title, description, etc. update file ``metadata.json`` in ``_data`` directory.
Add your documents (pages) in ``_docs``
