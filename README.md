# webpack-tuto
## Introduction
**Webpack** is a **module bundler**.for modern Javascript applications. It makes possible to use the NodeJS *require() and module.exports/require (or ES2015 modules with *Babel) to organize the front end code in separate files with functionality that can be implemented between them.
Webpack is configurable and flexible for creating strong development environments and doing a lot of other stuffs.
## First contact
In this examlpe we have 4 main files:
- **app.js:** This is the main Javascript file for our example. Thanks to Webpack, as mentionned early, we can import files in a modular way with `import`.
- **greeting.js:** This is the second javascript file. We just create a function that returns an HTML element (not a big deal to keep it simple).
- **webpack.config.js**: The Webpack configuration file. For this example, all what we did is defining the entry point for our application '`app.js`' and the output file which will be the ***bundle*** that will be served to the browser.
- **index.html:** Our html file that the browser will display. The important part is injecting the `bundle.js` that Webpack has created.

### Installing webpack
```$ npm install webpack -save-dev```
### Run the application
In `package.json` we added a new script to build the app which will execute webpack to read the config file.
All good now, run ```$ npm run build``` and open the html file in your browser aaaaaand that's it.
