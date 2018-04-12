# AngularPugDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 1.6.7.

## Development server

Adding pug to Angular 5

1. Install module using
npm install -D pug pug-ng-html-loader

2. Run the command ng-eject
	This opens the webpack.config.js

3. Add the code under module.exports - 	
  // Comment: Should be added in nearby line number 410
 
 module.exports = {
  module: {
    rules: [
      {
        test: /\.(pug|jade)$/,
        use: ['pug-ng-html-loader']
      }
    ]
  }
}

this part should be added before 
  module: {
    plugin: [
      {
       ...
	   }
    ]
  }
}

4. Rename .html component to .pug

5. Change templateUrl to .html

6. Run by using the following command - 
	npm run start


## Code Integration

The above code has been integrated in 

Angular CLI: 1.6.7 (e)
Node: 8.9.0
OS: win32 x64
Angular: 5.2.9
... animations, common, compiler, compiler-cli, core, forms
... http, language-service, platform-browser
... platform-browser-dynamic, router

@angular/cli: 1.6.7
@angular-devkit/build-optimizer: 0.0.42
@angular-devkit/core: 0.0.29
@angular-devkit/schematics: 0.0.52
@ngtools/json-schema: 1.1.0
@ngtools/webpack: 1.9.7
@schematics/angular: 0.1.17
typescript: 2.5.3
webpack-dev-server: 2.11.2
webpack: 3.10.0
