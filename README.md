# Parcel HTML, CSS, and JavaScript Starter Template

A blazing fast frontend development starter template, bundled using [Parcel](https://parceljs.org).

## Quick Start

To get started instantly, you can one-click deploy to Netlify below (this also creates a copy of the repository in your own GitHub account), or you can click the "Use this Template" above.

[![Deploy to Netlify](./src/assets/deploy-to-netlify.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/aileen-r/parcel-html-css-js-starter-template)

## Features

### HTML5 partials with posthtml‑include

Split your HTML pages into smaller, more manageable files with PostHTML's Include plugin for Parcel.
Usage

```html
<!-- index.html -->
<html>
  <head>
      <title>index.html</title>
  </head>
  <body>
      <include src="partials/header.html" locals='{
        "title": "Hello World"
      }'></include>
  </body>
</html>
```

```html
<!-- partials/header.html -->
<header>
  <h1>{{ title }}</h1>
</header>
```

### Modern ES6 JavaScript

Use modern JavaScript syntax and features like ES6 imports without the need for additional configuration.
Usage

```js
// index.js
import helloWorld from "./scripts/helloWorld";

helloWorld();
```

```js
// scripts/helloWorld.js

const helloWorld = () => {
  console.log("Hello world 👋");
};

export default helloWorld;
```

### CSS

A plain ol' vanilla CSS stylesheet to get you started. Check out my Parcel HTML, SASS, and JavaScript starter template if you are interested in using the CSS pre-processor SASS. Or, have a look at the [Parcel docs](https://v2.parceljs.org/) if you're interested in adding on another pre- or post-processor such as PostCSS, LESS, or Stylus.

## How to run
**Prerequisites**: You'll need [Node](https://nodejs.org) and [NPM](https://docs.npmjs.com/downloading-and-installing-node-js-and-npm) installed on your local computer.

Run

```
npm install
```
to intall dependencies, then
```
npm start
```
to start the local development server.

To build for production, run
```
npm run build
```