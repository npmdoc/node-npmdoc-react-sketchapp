# api documentation for  [react-sketchapp (v0.9.4)](https://github.com/airbnb/react-sketchapp)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-sketchapp.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-sketchapp) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-sketchapp.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-sketchapp)
#### A React renderer for Sketch.app

[![NPM](https://nodei.co/npm/react-sketchapp.png?downloads=true)](https://www.npmjs.com/package/react-sketchapp)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-react-sketchapp_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-sketchapp/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jon Gold",
        "email": "jon.gold@airbnb.com",
        "url": "http://jon.gold"
    },
    "bugs": {
        "url": "https://github.com/airbnb/react-sketchapp/issues"
    },
    "contributors": [
        {
            "name": "Ben Wilkins",
            "email": "ben.wilkins@airbnb.com"
        },
        {
            "name": "Leland Richardson",
            "email": "leland.richardson@airbnb.com"
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
        "shasum": "38bd57b1cc0a308bef4bcf0c9fbf229c0b06f3e6",
        "tarball": "https://registry.npmjs.org/react-sketchapp/-/react-sketchapp-0.9.4.tgz"
    },
    "gitHead": "172b4a4f3c6cfa2f9d44b777feacba3a5645594f",
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
            "name": "jongold",
            "email": "hello@designedbygold.com"
        }
    ],
    "name": "react-sketchapp",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "*",
        "react-test-renderer": "*"
    },
    "pre-commit": "lint-staged",
    "readme": "ERROR: No README data found!",
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
    "version": "0.9.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-sketchapp](#apidoc.module.react-sketchapp)
1.  object <span class="apidocSignatureSpan">react-sketchapp.</span>debug

#### [module react-sketchapp.debug](#apidoc.module.react-sketchapp.debug)
1.  [function <span class="apidocSignatureSpan">react-sketchapp.debug.</span>dump (obj)](#apidoc.element.react-sketchapp.debug.dump)
1.  [function <span class="apidocSignatureSpan">react-sketchapp.debug.</span>timeFunction (fn, label)](#apidoc.element.react-sketchapp.debug.timeFunction)



# <a name="apidoc.module.react-sketchapp"></a>[module react-sketchapp](#apidoc.module.react-sketchapp)



# <a name="apidoc.module.react-sketchapp.debug"></a>[module react-sketchapp.debug](#apidoc.module.react-sketchapp.debug)

#### <a name="apidoc.element.react-sketchapp.debug.dump"></a>[function <span class="apidocSignatureSpan">react-sketchapp.debug.</span>dump (obj)](#apidoc.element.react-sketchapp.debug.dump)
- description and source-code
```javascript
function dump(obj) {
  log('#####################################################################################');
  log('## Dumping object ' + obj);
  log('## obj class is: ' + obj.className());
  log('#####################################################################################');
  log('obj.properties:');
  log(obj.class().mocha().properties());
  log('obj.propertiesWithAncestors:');
  log(obj.class().mocha().propertiesWithAncestors());
  log('obj.classMethods:');
  log(obj.class().mocha().classMethods());
  log('obj.classMethodsWithAncestors:');
  log(obj.class().mocha().classMethodsWithAncestors());
  log('obj.instanceMethods:');
  log(obj.class().mocha().instanceMethods());
  log('obj.instanceMethodsWithAncestors:');
  log(obj.class().mocha().instanceMethodsWithAncestors());
  log('obj.protocols:');
  log(obj.class().mocha().protocols());
  log('obj.protocolsWithAncestors:');
  log(obj.class().mocha().protocolsWithAncestors());
  log('obj.treeAsDictionary():');
  log(obj.treeAsDictionary());
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-sketchapp.debug.timeFunction"></a>[function <span class="apidocSignatureSpan">react-sketchapp.debug.</span>timeFunction (fn, label)](#apidoc.element.react-sketchapp.debug.timeFunction)
- description and source-code
```javascript
function timeFunction(fn, label) {
  var a = MSMoment.new().timestamp();

  var res = fn();

  var b = MSMoment.new().timestamp();

  var time = (b - a).toFixed(3);

  log(label + ': ' + time);

  return res;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
