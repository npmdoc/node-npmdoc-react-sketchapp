# npmdoc-react-sketchapp

#### api documentation for  [react-sketchapp (v0.10.0)](https://github.com/airbnb/react-sketchapp)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-sketchapp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-sketchapp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-sketchapp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-sketchapp)

#### A React renderer for Sketch.app

[![NPM](https://nodei.co/npm/react-sketchapp.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-sketchapp)

- [https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jon Gold",
        "url": "http://jon.gold"
    },
    "bugs": {
        "url": "https://github.com/airbnb/react-sketchapp/issues"
    },
    "contributors": [
        {
            "name": "Ben Wilkins"
        },
        {
            "name": "Leland Richardson"
        }
    ],
    "dependencies": {
        "css-layout": "^1.1.1",
        "error-stack-parser": "^2.0.0",
        "invariant": "^2.2.2",
        "murmur2js": "^1.0.0",
        "normalize-css-color": "^1.0.1",
        "sketch-constants": "^1.0.2",
        "sketchapp-json-flow-types": "^0.0.3",
        "sketchapp-json-plugin": "^0.0.3"
    },
    "description": "A React renderer for Sketch.app",
    "devDependencies": {
        "@jongold/eslint-config-sketch": "^1.0.0-2",
        "babel-cli": "^6.18.0",
        "babel-core": "^6.0.0",
        "babel-eslint": "^7.1.0",
        "babel-jest": "^18.0.0",
        "babel-plugin-transform-flow-strip-types": "^6.18.0",
        "babel-polyfill": "^6.20.0",
        "babel-preset-es2015": "^6.18.0",
        "babel-preset-react": "^6.16.0",
        "babel-preset-stage-0": "^6.16.0",
        "eslint": "^3.9.1",
        "eslint-config-airbnb": "^12.0.0",
        "eslint-plugin-import": "^1.16.0",
        "eslint-plugin-jsx-a11y": "^2.2.3",
        "eslint-plugin-react": "^6.4.1",
        "flow-bin": "^0.36.0",
        "flow-copy-source": "^1.1.0",
        "gitbook-cli": "^2.3.0",
        "jest-cli": "^18.1.0",
        "lint-staged": "^3.4.0",
        "pre-commit": "^1.2.2",
        "prettier-eslint-cli": "^3.1.2",
        "react": "^15.4.1",
        "react-test-renderer": "^15.4.1",
        "rimraf": "^2.5.4"
    },
    "directories": {},
    "dist": {
        "shasum": "3a7cfb830f2f91e2f0ef4474b37ea7c7335dc21b",
        "tarball": "https://registry.npmjs.org/react-sketchapp/-/react-sketchapp-0.10.0.tgz"
    },
    "gitHead": "b4cff0bf45ed59b23bfd57f466a1fb6c2aed9177",
    "homepage": "https://github.com/airbnb/react-sketchapp",
    "keywords": [
        "sketch",
        "sketchapp",
        "react",
        "reactjs",
        "renderer"
    ],
    "license": "MIT",
    "lint-staged": {
        "*.js": [
            "prettier-eslint --write \"src/**/*.js\"",
            "git add"
        ]
    },
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "jongold"
        }
    ],
    "name": "react-sketchapp",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "*",
        "react-test-renderer": "*"
    },
    "pre-commit": "lint-staged",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/airbnb/react-sketchapp.git"
    },
    "scripts": {
        "build": "npm run build:react && npm run build:flow",
        "build:flow": "flow-copy-source -v -i '**/__tests__/**' src lib",
        "build:react": "babel src -d lib --ignore **/__mocks__/**",
        "check": "npm run test && npm run flow && npm run lint",
        "clean": "rimraf lib react-example.sketchplugin",
        "docs:build": "npm run docs:prepare && gitbook build",
        "docs:clean": "rimraf _book",
        "docs:prepare": "gitbook install",
        "docs:publish": "npm run docs:clean && npm run docs:build && cd _book && git init && git commit --allow-empty -m 'update book' && git fetch git@github.com:airbnb/react-sketchapp.git gh-pages && git checkout -b gh-pages && git add . && git commit -am 'update book' && git push git@github.com:airbnb/react-sketchapp.git gh-pages --force",
        "docs:watch": "npm run docs:prepare && gitbook serve",
        "flow": "flow",
        "lint": "eslint .",
        "lint-staged": "lint-staged",
        "prepublishOnly": "npm run clean && npm run check && npm run build",
        "test": "jest --config .jestrc",
        "test:ci": "jest --config .jestrc --runInBand",
        "test:watch": "npm run test -- --watch",
        "watch": "npm run build:react -- --watch"
    },
    "version": "0.10.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
