---

# Sassy CSS Boilerplate

An HTML CSS boilerplate with built-in sass support:

## Get Started

- [Setup](#setup)
- [Scripts](#scripts)
- [Project Structure](#project-structure)

## Setup

1. create a folder for your project

1. create README.md file

1. you need to run

```
npm init
```

in order to create `package.json` file

1. Edit `package.json` to add you project's name

   `package.json`

   ```json
   {
     "name": "[project name]",
     ...
     "author": "[your name]"
   }
   ```

1. create `.gitignore` and skip this folders

```
dist/

src/styles/

node_modules/
```

1. create folder `src`

1. create your project folders inside `src` folder, you will need (scss,img,scripts) folders and `index.html` file

1. Edit `src/index.html` to add your projects name

   ```html
   ...
   <head>
     ...
     <title>[project name]</title>
   </head>
   ...
   ```

1. Start a new git repository and make an initial commit. This will make sure that you can work on your project with git.

   ```
   git init
   git add . && git commit -m "Initial commit"
   ```

   PS: Remember to push to Github

1. Install the dependencies

   ```
   npm install
   ```

## Scripts

### Development

Run **live-server** and **sass** in **watch** mode and start coding!

```
npm start
```

### Production

Transpile sass and copy relevant files from **src** to **dist** to prepare your website for **deployment**.

```
npm run build
```

PS: Remember to push to Github

### Deploy to Github Pages

Deploy your code to **Github Pages**: this script creates a 'gh-pages' branch and publishes the **dist** folder. For this to work, make sure you already have a remote repository on github.

```
npm run deploy
```

## Project Structure

Any project created with this boilerplate will follow the structure below:

```
Project
│   README.md
│   package.json
|   package-lock.json
└───src
│   │   index.html
│   └───styles
|   └───scss
|   |   └───style.scss
│   └───scripts
|   └───img
└───dist
```

### `README.md`

The README should contain a brief description of your project, feel free to delete this guide or rename it to add your own description.

### `package.json` & `package-lock.json`

These files contain various information about you, your project and the project dependencies, as well as useful scripts to help you with the development process. Please do not edit these files for the time being, except where you're asked to. In the future, you will learn more about project dependencies.

### `src` & `index.html`

The `src` folder contains any file you would want to add to your website before any processing is done to it. **This is the main folder you will be working in**.

`index.html` is the main page for your website which you will be working on. Feel free to add any new `html` pages you create directly in the `src` folder.

### `scripts`

The `scripts` folder will contain any `js` files you will add to your website. Eventually `index.js` is the _**main**_ script file of your project. Feel free to use this file to add any JavaScript that you want to experiment with. You will learn more about JavaScript in the browser in the future.

### `scss` & `style.scss`

The `scss` folder will contain any `scss` or `css` files (depending on your preference). In order to include additional styles in your project, you must import them to `style.scss`.

`style.scss` is your style _**entry point**_. Any other `scss` or `css` imported to this file can be used, and any styles written directly to this file will be applied.

### `img` or `fonts`

For the sake of organization and good project structure practices, please use these folders in order to keep your images and fonts respectively.

### `dist`

The `dist` folder will be automatically generated whenever your run the build script:

```bash
npm run build
```

This folder will contain your built project, ready to be deployed online. It is excluded from `git` tracking since it is not customary to include compiled code in a development project.

### links

- Automatic [Sass](https://sass-lang.com/) transpilation
- Development server powered by [live-server](https://www.npmjs.com/package/live-server) with automatic reload
- Deployments to github pages with [gh-pages](https://www.npmjs.com/package/gh-pages)