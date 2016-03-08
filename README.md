React with react-router-V2
==============================
React : 0.14.7 

Initialising the application
 - npm init
 - install the respective packages
 - add this to package.json
 "scripts": {
     "2js": "babel --presets react,es2015 js --out-dir buildReact",
     "pack": "webpack buildReact/app.js build/bundle.js"
   }
 - change the 'main' from 'index.js' to 'app.js'
 - load the dependencies : flux,react,react-dom,react-router,underscore ( npm install react --save )
 - load the dev dependencies : babel-cli,babel-preset-es2015,babel-preset-react,css-loader,style-loader,webpack ( npm install webpack --save-dev )


Uses
 - [Babel][2]
 - [Webpack][3]
 - [react-router][1]

Installing [react-router][1] is as below
 npm install react-router --save

This is for [react-router 2.0][1]. Two things are must here.
 1. Provide the history property to the Router object.
 2. Provide contextTypes property to the components.

The first one is necessary as with version 2, [react-router][1] does not create any default history property. The second one is used to get the context. Since all the methods are now called through router object, which is available in context object.






[1]: https://github.com/rackt/react-router
[2]: https://babeljs.io/
[3]: https://webpack.github.io/
