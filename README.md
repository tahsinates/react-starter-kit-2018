Used Packages;

webpack: We need Webpack to bundle our code.

webpack-cli: We will be using some CLI features of Webpack to make our lives easier while writing some scripts.

webpack-dev-server: I will create a server using the webpack-dev-server package. This is only meant to be used in the development environment, and not for production. This means while developing and working on my code, I don’t need a separate server like NodeJS to setup manually.

webpack-merge: To divide our configuration into chunks.

webpack-visualizer-plugin: To see a visual representation of each of our bundle size — how much space they are taking and what are their dependencies.

style-loader: This adds CSS to the DOM by injecting a < script /> tag in the header

sass-loader: For SCSS support

node-sass: A dependency for sass-loader

css-loader: To convert our .scss files into .css

mini-css-extract-plugin: This plugin extracts CSS into separate files. It creates a CSS file per JS file which contains CSS.

uglifyjs-webpack-plugin: To minify JavaScript code for production

optimize-css-assets-webpack-plugin To minify CSS code for production

html-webpack-plugin: This does more then generate an HTML file, it supports on demand .css and .js files automatically added to your HTML files on demand

copy-webpack-plugin: Copies files/folders to your build folder.

babel-loader: This is the loader that helps webpack compile .js files

@babel/core: Babel core compiler, this is a dependency that lets you use babel-loader

@babel/preset-react Babel preset for React code

@babel/preset-env: Babel preset that allows you to use the latest JavaScript

@babel/pollyfill: Babel includes a polyfill that includes a custom regenerator runtime and core-js. This will emulate a full ES2015+ environment. This means support for async/await type of cool syntax sugar.

@babel/plugin-proposal-class-properties: Coverts your class syntax into a function for browsers that don’t support class syntax

@babel/plugin-proposal-export-namespace-from Supports syntax like import * as ns from '../path/to/module';

@babel/plugin-proposal-throw-expressions New syntax to throw exceptions from within an expression context.

@babel/plugin-syntax-dynamic-import This is what helps with code splitting. Webpack ships with code splitting by default (Since webpack 1). But when you want to code split in webpack while you are using babel, then you need to use this plugin.

<<<<<<< HEAD
Package.json configuration info:

webpack-dev-server serves a webpack app and updates the browser on changes.
--mode development tells webpack to compile the code in development mode. This is basically to make the compilation time faster.
--config config/webpack.base.config.js So by default if you have webpack.config.js file in your root app folder, you don’t have to supply the --config flag to it. But since I want to explicitly add all my webpack related configurations in the config folder, I pass in --config option that tells webpack where to look for the configuration
--open command opens the browser, when webpack is done with its compilation.
--hot flag tells webpack to actively watch for code changes in the src folder. If any changes happen, it reloads the browser.
--history-api-fallback This option enables History API Fallback support in webpack-dev-server, effectively asking the server to fallback to index.html in the event that a requested resource cannot be found.
--env.PLATFORM & --env.VERSION are custom flags that I pass in my configuration (more on this later).
=======

URL : https://medium.freecodecamp.org/how-to-combine-webpack-4-and-babel-7-to-create-a-fantastic-react-app-845797e036ff
>>>>>>> 6da8973429d717ab4167fec5e1d20c4de59f5b6b

