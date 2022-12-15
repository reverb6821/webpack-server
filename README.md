# What is

This is my boilerplate that I use in my regular workflow for a webpack dev server for a automatic and real-time compiling

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
│   |   ├── partials
│   |   └── pages
│   ├── styles
│   |   ├── base
│   |   ├── components
│   |   ├── layouts
│   |   ├── pages
│   |   └── styles
├── README.md
└── package.json

```

All files are in the src folder, it includes assest, css, images, js, sass and pug folders.

- assets : some static files, e.g. fonts, svg ...etc.
- js : entry point index.js is here, and you also can put other customize js files
- styles : put your sass files here, you can manage this folder structure for your own
- pug : pug template files, you can use a different layout for extends

The file in config folder are webpack 5.x config setting, to handle Pug + Sass into HTML files.

# Getting started

You can clone this repo or fork it.

If you fork it, when you create a new repo select this as starting template