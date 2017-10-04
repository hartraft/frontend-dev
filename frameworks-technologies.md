# Listing of different frameworks that i'm learning
This is a personal list to help keep a track of the diverse number of frameworks / technologies in JS. 
Reading [Learning JS in 2016](https://hackernoon.com/how-it-feels-to-learn-javascript-in-2016-d3a717dd577f) has led to this list as a braindump

JS Preprocessors:
* [Babel](https://babeljs.io/)
* TypeScript

Template / markup preprocessors:
* ![Haml logo](http://haml.info/images/haml.png) http://haml.info/
* [Jade] => renamed to [Pug](https://pugjs.org/api/getting-started.html)

CSS Preprocessors:
* Sass
* Less

Haven't used before:
* Stylus
* CoffeeScript
* Slim

### JS Module Loaders (runtime):
Loads modules and dependencies in the correct order at runtime.
* [RequireJS](http://requirejs.org/) :loader for modules in AMD format.
* [SystemJs](https://github.com/systemjs/systemjs) :loader for modules in AMD,CommonJS, UMD.

### JS Module bundlers (compile time):
Bundlers essentially concat all the JS needed for a module and handles treeshaking (removing unnecessary dependencies). It also sees any dependency issues on compile time.
* Browserify :bundler for CommonJS modules
* Webpack :bundler for AMD,CommonJS,ES6 modules
* Rollup.js :bundler for AMD,UMD,CommonJS,ES6 modules (mainly described in angular.io docs)


## ES6 / ES2015
From the [rollup site](https://rollupjs.org/#tree-shaking)
> the ES6 revision of JavaScript includes a syntax for importing and exporting functions and data so they can be shared between separate scripts. The specification is now fixed, but it is not yet implemented in browsers or Node.js.

### CommonJS, the entire tool or library must be imported:
```javascript
// import the entire utils object with CommonJS
var utils = require( 'utils' );
var query = 'Rollup';
// use the ajax method of the utils object
utils.ajax( 'https://api.example.com?search=' + query ).then( handleResponse );
```

### ES6 modules, instead of importing the whole utils object, we can just import the one ajax function we need:
```javascript
// import the ajax function with an ES6 import statement
import { ajax } from 'utils';
var query = 'Rollup';
// call the ajax function
ajax( 'https://api.example.com?search=' + query ).then( handleResponse );
```
