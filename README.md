---

# Vanilla JS Boilerplate

> This is a starter workflow for building vanilla JavaScript applications using Sass.

It includes all the necessary scripts to develop and deploy an application on Github Pages.

The boilerplate uses SASS and follow the [7-1 architecture pattern](http://sass-guidelin.es/#architecture) and sticking to [Sass Guidelines](http://sass-guidelin.es) writing conventions.

Each folder of this project has its own `README.md` file to explain the purpose and add extra information. Be sure to browse the repository to see how it works.

## Setup

1 - Installing all the necessary dependencies

> The following dependencies will be installed.

- Automatic [Sass](https://sass-lang.com/) transpilation
- Development server powered by [live-server](https://www.npmjs.com/package/live-server) with automatic reload
- Deployments to github pages with [gh-pages](https://www.npmjs.com/package/gh-pages)
- Prefixier CSS using [Autoprefixier](https://github.com/postcss/autoprefixer)

```
npm install
```

## Scripts

### Development

Run **live-server** and **sass** in **watch** mode and start coding!

```
npm start
```

Remove **dist** folder

```
npm run clean
```

### Production

Transpile sass, add CSS prefixs and copy relevant files from **src** to **dist** to prepare your website for **deployment**.

```
npm run build
```

### Deploy to Github Pages

Deploy your code to **Github Pages**: this script creates a 'gh-pages' branch and publishes the **dist** folder. For this to work, make sure you already have a remote repository on github.

```
npm run deploy
```

## Project Structure

### `package.json` & `package-lock.json`

These files contain various information about you, your project and the project dependencies, as well as useful scripts to help you with the development process.

### `src` & `index.html`

The `src` folder contains any file you would want to add to your website before any processing is done to it. **This is the main folder you will be working in**.

`index.html` is the main page for your website which you will be working on. Feel free to add any new `html` pages you create directly in the `src` folder.

### `scripts`

The `scripts` folder will contain any `js` files you will add to your website. Eventually `index.js` is the _**main**_ script file of your project. Feel free to use this file to add any JavaScript that you want to experiment with.

### `scss` & `style.scss`

The `scss` folder already contain a sample project using the [7-1 architecture pattern](http://sass-guidelin.es/#architecture). In order to include additional styles in your project, you must import them to `main.scss`.

`main.scss` is your style _**entry point**_. Any other `scss` or `css` imported to this file can be used, and any styles written directly to this file will be applied.

### `img` or `fonts`

For the sake of organization and good project structure practices, please use these folders in order to keep your images and fonts respectively.

## FAQ

### What is this `dist` folder?

The `dist` folder will be automatically generated whenever your run the build script:

```bash
npm run build
```

This folder will contain your built project, ready to be deployed online. It is excluded from `git` tracking since it is not customary to include compiled code in a development project.
