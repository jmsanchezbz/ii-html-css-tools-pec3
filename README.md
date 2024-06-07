# UOC Boilerplate

UOC Boilerplate is a starter template for the HTML and CSS Tools courses from the [Master's Program in Multimedia Applications](https://estudis.uoc.edu/ca/masters-universitaris/aplicacions-multimedia/presentacio) and the [Master's Program in Web App and Website Development](https://estudis.uoc.edu/ca/masters-universitaris/desenvolupament-llocs-aplicacions-web/presentacio) at the [Universitat Oberta de Catalunya](https://www.uoc.edu). It aims to provide a basic, modern frontend web development starter pack based on Parcel and including a Sass compiler, an ES6 transpiler, minifiers, an image transformer, and development tools.

This is the 3.x version of UOC Boilerplate, available since the UOC 2020-2 semester.

## Requirements

[Node.js](http://nodejs.org/) >= 14.15.x

## Getting started

Clone this repository with `git clone`, or download a .zip file using the top right green button.

Using the Terminal, navigate to the project folder and run `npm install`.

## Features

- Uses [Parcel v2](https://parceljs.org) module bundler.
- NPM scripts for fast development and production build (see Commands below).

### Stylesheets

- [Sass/SCSS](https://sass-lang.com) to CSS compilation.
- Minification and optimization of CSS files on production builds with [`cssnano`](https://github.com/cssnano/cssnano) (`@parcel/optimizer-cssnano`).
- [PostCSS](https://postcss.org/) features:
  - Transpile modern CSS with [`postcss-preset-env`](https://preset-env.cssdb.org/features).
  - Automatically add CSS prefix to unsupported properties with [`autoprefixer`](https://autoprefixer.github.io/).

### HTML

- Minification and optimization of CSS files on production builds [`htmlnano`](https://github.com/posthtml/htmlnano) (`@parcel/optimizer-htmlnano`).
- [PostHTML](https://github.com/posthtml/posthtml) features:
  - Include partial HTML files with [`posthtml-include`](https://github.com/posthtml/posthtml-include).

### Scripts

- Allow for modern JavaScript (ES201x/ES8/ES7/ES6…) which is automatically transpiled to ES5 and minifed in production builds, with [Babel](https://babeljs.io/).

### Images

- Image transformation with [`@parcel/transformer-image`](https://parceljs.org/recipes/image/) (based on [`sharp`](https://sharp.pixelplumbing.com/)).

### Development

- Development server launch and live reloading on file changes.
- Friendly error reporting.

## How to use this boilerplate

Content lives inside the `src/` folder. If you do not want to change the configuration or are unsure about what you are doing, do not edit files outside the `src/` folder.

Always run the following commands during the development stage and for production builds. Please note that it is expected that all projects built with this boilerplate are compiled using `npm run build` before they are published.

### Commands

| Command         | Description                                                                                                                                                                                                                                                                                                                                                         |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `npm run dev`   | Runs a local web server for development and opens the browser to display it. Automatically compiles styles and scripts whenever a file in `src/` is changed, and live reloads the browser. This is what _must be run_ on the development stage.                                                                                                                     |
| `npm run build` | Compiles and minifies and optimizes the files in the assets folder. The generated compiled and optimized files are located in the `dist/` folder. This is what _must be run_ before publishing the project. This is also the build command to be run by external deployment services such as Netlify. The publishable files are then located in the `dist/` folder. |
| `npm run clean` | Deletes the current `/dist` folder and cache folders.                                                                                                                                                                                                                                                                                                               |
| `npm run test`  | Displays a success message if everything is working as expected.                                                                                                                                                                                                                                                                                                    |

## Need help? / Want to help out?

Feel free to create a [new issue](https://github.com/uoc-advanced-html-css/uoc-boilerplate/issues/new/) or drop me a line at jorditarrida@uoc.edu.

Are you using this Boilerplate for your projects or for educational purposes? I would love to hear about it!

## AI Generated page with chat GPT

PROMPT: Generate a web page with html and css separeated about a Cooking contest 2024 edition formed by the following elements:
- A header with two sides, left one with title Cooking contest 2024 edition, and right side with a menu with home, the contest, recipes and Contestants element where Contestants is the active item with a button like with black background, white letters and rounded corners.
- A footer with two sides as well, left side has a title Cooking contest 2024 edition with social networks icons (facebook, linkedin, youtube and instagram) links under it. The right side has a three column menus with Recipes(Cajun seafood pasta, cedar planked salmon, poulet au vinagre), Contestants (John Cooper, Marta Alonso and Mary Ann Stones) and Contest editions (2024, 2023 and 2022). Footer has a border top solid 1px grey.
- A main content with an h1 ‘Contestants’ with text under ‘This section describes the recipes of the best contestans’. Under that an image with food chef preparation full width with rounded borders and margins on both sides. Under the image there is an h2 with ‘The recipes’ and under the text ‘These are the recipes of the best contestatnts’. Below that there are three cards with the name of the recipe at the top, below an image of the chef with clip-shape circle at the left and the name of the chef and under a critic of the recipe.

Titles and h1.. are black and text is grey, as well as social network icons