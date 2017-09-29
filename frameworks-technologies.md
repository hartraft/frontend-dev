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

###JS Module Loaders (runtime):
Loads modules and dependencies in the correct order at runtime.
* [RequireJS](http://requirejs.org/) :loader for modules in AMD format.
* [SystemJs](https://github.com/systemjs/systemjs) :loader for modules in AMD,CommonJS, UMD.

JS Module bundlers (compile time):
Bundlers essentially concat all the JS needed for a module and handles treeshaking (removing unnecessary dependencies). It also sees any dependency issues on compile time.
* Browserify :bundler for CommonJS modules
* Webpack :bundler for AMD,CommonJS,ES6 modules
* Rollup.js :bundler for AMD,UMD,CommonJS,ES6 modules (mainly described in angular.io docs)
