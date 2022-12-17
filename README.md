# What is

This is my boilerplate that I use in my regular workflow for a webpack dev server for a automatic and real-time compiling

# Getting started

You can clone this repo or fork it (I suggest to fork it, it's more practical.

If you fork it, when you create a new repo select this as starting template.

I've choose to not add any CSS framework, cause I (or you) can add the favorite one (I suggest Tailwind.css).

# Project structure
```
.
├── config
│   ├── webpack.common
│   ├── webpack.dev
│   └── webpack.prod
├── src
│   ├── assets
│   |   ├── fonts
│   |   └── images
│   ├── js
│   ├── pug
│   |   ├── base
│   |   ├── layouts
│   |   ├── pages
│   |   └── partials
│   ├── styles
│   |   ├── base
│   |   ├── layouts
│   |   ├── pages
│   |   └── styles
├── README.md
└── package.json

```

All files are in the src folder, it includes assest, css, images, js, sass and pug folders.

- assets : some static files, e.g. fonts, svg ...etc.
- js : entry point index.js is here, and you also can put other customize js files
- styles : put your sass files here, you can manage this folder structure for your own.  I've opted .sass for better code readability
- pug : pug template files, you can use a different layout for extends and modulize your template. I've opted pug for better code readability.

Inside pug directory, you can find:
- base : the base of html document, the header and the body, where the layout is injected
- layouts : the core document
- pages : all the pages that are needed to be injected inside layouts (example index, about etc...)
- partials : all the reusable element (like navbar, footer, button etc...)
The file in config folder are webpack 5.x config setting, to handle Pug + Sass into HTML files.

### Builded with
#### Linters:
* [prettier](https://prettier.io/) : An opinionated code formatter.
* [eslint](https://eslint.org/) : ESLint statically analyzes your code to quickly find problems.
* [stylelint](https://stylelint.io/) : linter that helps you avoid errors and enforce conventions in your styles.
#### Styles and Template:
* [sass](https://sass-lang.com/) : Sass is the most mature, stable, and powerful professional grade CSS extension language in the world.
* [pug](https://pugjs.org/) : Pug is a high-performance template engine heavily influenced by Haml and implemented with JavaScript for Node.js and browsers.
#### Compiler and Bundler:
* [webpack](https://webpack.js.org/) : webpack is a module bundler. Its main purpose is to bundle JavaScript files for usage in a browser.
* [webpack-dev-server](https://webpack.js.org/configuration/dev-server/) : webpack-dev-server can be used to quickly develop an application.
* [webapck-merge](https://www.npmjs.com/package/webpack-merge) : Aprovides a merge function that concatenates arrays and merges objects creating a new object.
#### Webpack Plugin:
* [clean-webpack-plugin](https://www.npmjs.com/package/clean-webpack-plugin) : A webpack plugin to remove/clean your build folder(s).
* [css-loader](https://webpack.js.org/loaders/css-loader/) : The css-loader interprets @import and url() like import/require() and will resolve them.
* [sass-loader](https://www.npmjs.com/package/sass-loader) : Loads a Sass/SCSS file and compiles it to CSS.
* [pug-plugin](https://www.npmjs.com/package/pug-plugin) : enable to use Pug files in Webpack entry and generates HTML files that contain the hashed output JS and CSS filenames whose source files are specified in the Pug template.
#### Utility
* [npm-run-all](https://www.npmjs.com/package/npm-run-all) : A CLI tool to run multiple npm-scripts in parallel or sequential.

### Production

When you build, the compiled file can be hosted as static site, or if you need you can add it in public view of your app (example inside resource/static of springboot app or /public of node server).
