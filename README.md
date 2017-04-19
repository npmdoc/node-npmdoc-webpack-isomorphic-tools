# npmdoc-webpack-isomorphic-tools

#### api documentation for  [webpack-isomorphic-tools (v3.0.2)](https://github.com/halt-hammerzeit/webpack-isomorphic-tools#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-webpack-isomorphic-tools.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-webpack-isomorphic-tools) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-webpack-isomorphic-tools.svg)](https://travis-ci.org/npmdoc/node-npmdoc-webpack-isomorphic-tools)

#### Transforms CSS-alike text into a React style JSON object

[![NPM](https://nodei.co/npm/webpack-isomorphic-tools.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/webpack-isomorphic-tools)

- [https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-webpack-isomorphic-tools/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Halt Hammerzeit"
    },
    "bugs": {
        "url": "https://github.com/halt-hammerzeit/webpack-isomorphic-tools/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.6.1",
        "colors": "^1.1.2",
        "fs-extra": "^0.30.0",
        "require-hacker": "^3.0.0",
        "sync-request": "^3.0.1",
        "uglify-js": "^2.7.0"
    },
    "description": "Transforms CSS-alike text into a React style JSON object",
    "devDependencies": {
        "babel-cli": "^6.10.1",
        "babel-core": "^6.10.4",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-runtime": "^6.6.0",
        "babel-preset-es2015": "^6.6.0",
        "babel-preset-stage-0": "^6.5.0",
        "chai": "^3.5.0",
        "coveralls": "^2.11.11",
        "istanbul": "^1.1.0-alpha.1",
        "json-loader": "^0.5.4",
        "minimist": "^1.2.0",
        "mocha": "^2.5.3",
        "npm-run-all": "^2.3.0",
        "rimraf": "^2.5.3"
    },
    "directories": {},
    "dist": {
        "shasum": "565cbb02af873a8924e826dda460ab6b86b87f53",
        "tarball": "https://registry.npmjs.org/webpack-isomorphic-tools/-/webpack-isomorphic-tools-3.0.2.tgz"
    },
    "gitHead": "28fa6897a288f9705bf3f361fe00838cd4fd861e",
    "homepage": "https://github.com/halt-hammerzeit/webpack-isomorphic-tools#readme",
    "keywords": [
        "react",
        "style",
        "inline",
        "css"
    ],
    "license": "MIT",
    "main": "babel-transpiled-modules/index.js",
    "maintainers": [
        {
            "name": "halt-hammerzeit"
        }
    ],
    "name": "webpack-isomorphic-tools",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/halt-hammerzeit/webpack-isomorphic-tools.git"
    },
    "scripts": {
        "build": "npm-run-all clean-for-build build-modules",
        "build-modules": "babel ./source --out-dir ./babel-transpiled-modules --source-maps",
        "clean-for-build": "rimraf ./babel-transpiled-modules/**/*",
        "prepublish": "npm-run-all build test",
        "test": "mocha --compilers js:babel-core/register --colors --bail --reporter spec test/ --recursive",
        "test-coverage": "istanbul cover node_modules/mocha/bin/_mocha -- --compilers js:babel-core/register --colors --reporter dot test/ --recursive",
        "test-travis": "istanbul cover node_modules/mocha/bin/_mocha --report lcovonly -- --compilers js:babel-core/register --colors --reporter spec test/ --recursive"
    },
    "version": "3.0.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
