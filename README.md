<section align="center" style="display: flex; flex-direction: column">
  <h1>Emmy.js</h1>
  <div>
    <img alt="npm" src="https://img.shields.io/npm/v/emmy-dom"/>
    <img alt="npm" src="https://img.shields.io/npm/dt/emmy-dom"/>
    <img alt="NPM" src="https://img.shields.io/npm/l/emmy-dom"/>
    <img alt="GitHub last commit (by committer)" src="https://img.shields.io/github/last-commit/eanorambuena/Emmy.js"/>
    <img alt="npm package minimized gzipped size (select exports)" src="https://img.shields.io/bundlejs/size/emmy-dom"/>
  </div>
  <i>A tiny simple frontend framework for building web applications.</i>
</section>
<hr />

## Why Emmy.js?
Emmy.js is a tiny simple frontend framework for building web applications. It is based on the [Web Components](https://developer.mozilla.org/en-US/docs/Web/Web_Components) standard.
It is specially designed for building web applications with server-side frameworks like Ruby on Rails, Django, Laravel, etc.

<hr />

## _Experimental_ `npx create-emmy`
[create-emmy](https://www.npmjs.com/package/create-emmy) is a command line tool that allows you to create a new emmy.js project.
It is still in an experimental phase, so it is not recommended to use it in production, but you can try it out and give us your feedback. [More info](https://github.com/emmyjs/create-emmy#readme)

## Frameworks Guides
For your specific framework, see the following guides:
1. [Ruby on Rails](docs/0.0.2/guides/ruby-on-rails.md)

## Quick Start
### Using CDN
Just add the following script tag to your HTML file:

```html
<script src="https://cdn.jsdelivr.net/npm/emmy-dom@latest" type="module"></script>
```

Then, use the `emmy-dom` package in your JavaScript files:

```javascript
import { LightComponent, launch } from "emmy-dom";

class MyComponent extends LightComponent {
    constructor() {
        super();
        render(`<div>Hello World!</div>`);
    }
}

launch(MyComponent);
```

### Using npm
First install the package:

```bash
npm install emmy-dom
```

Then, use the `emmy-dom` package in your JavaScript files:

```javascript
import { LightComponent, launch } from "emmy-dom";

class MyComponent extends LightComponent {
    constructor() {
        super();
        render(`<div>Hello World!</div>`);
    }
}

launch(MyComponent);
```

## Release 0.0.3
It includes the following features:
1. [Component Class](docs/0.0.2a1/component-class.md)
2. [LightComponent Class](docs/0.0.2a1/light-component-class.md)
3. [Launch Function](docs/0.0.2a1/launch-function.md)
4. [Emmy Router](docs/0.0.3a1/emmy-router.md)
5. **BREAKING CHANGE**: Remove `git clone` support. Now you can use `npx create-emmy` to create a new emmy.js project.

[Release Notes](docs/releases.md)
