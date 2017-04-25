# npmdoc-react-hyperscript-helpers

#### basic api documentation for  [react-hyperscript-helpers (v1.2.0)](https://github.com/jador/react-hyperscript-helpers#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-hyperscript-helpers.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-hyperscript-helpers) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-hyperscript-helpers.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-hyperscript-helpers)

#### Terse syntax for hyperscript using react

[![NPM](https://nodei.co/npm/react-hyperscript-helpers.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-hyperscript-helpers)

- [https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-hyperscript-helpers/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tyler Graham"
    },
    "bugs": {
        "url": "https://github.com/jador/react-hyperscript-helpers/issues"
    },
    "dependencies": {},
    "description": "Terse syntax for hyperscript using react",
    "devDependencies": {
        "babel-cli": "^6.5.1",
        "babel-core": "^6.2.1",
        "babel-preset-es2015": "^6.1.18",
        "babel-preset-stage-2": "^6.1.18",
        "chai": "^3.4.1",
        "eslint": "^2.7.0",
        "eslint-config-airbnb": "^6.2.0",
        "eslint-plugin-react": "^4.2.3",
        "mocha": "^2.3.4",
        "rimraf": "^2.4.4",
        "typescript": "^1.7.5"
    },
    "directories": {},
    "dist": {
        "shasum": "56f925ba7114c9d7e82dbfacedcc9cb343bb564e",
        "tarball": "https://registry.npmjs.org/react-hyperscript-helpers/-/react-hyperscript-helpers-1.2.0.tgz"
    },
    "gitHead": "25371e371ca0ccebed313fd0050cf7ef3a75139c",
    "homepage": "https://github.com/jador/react-hyperscript-helpers#readme",
    "keywords": [
        "hyperscript",
        "react",
        "jsx",
        "hyperscript-helpers",
        "react-hyperscript",
        "react-hyperscript-helpers"
    ],
    "license": "ISC",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "jador"
        }
    ],
    "name": "react-hyperscript-helpers",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": ">=0.13.0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/jador/react-hyperscript-helpers.git"
    },
    "scripts": {
        "build": "npm run build:babel && npm run build:ts-def",
        "build:babel": "babel src --out-dir lib",
        "build:ts-def": "babel-node ./generate-ts-def.js",
        "clean": "rimraf lib",
        "lint": "eslint src test",
        "postversion": "git push && git push --tags",
        "prepublish": "npm run clean && npm run build",
        "test": "npm run test:mocha && npm run test:tsc",
        "test:mocha": "mocha -c -r babel-core/register ./test/**/*Spec.js",
        "test:tsc": "npm run build && npm run test:tsc:fake-install && npm run test:tsc:compile && npm run test:tsc:cleanup",
        "test:tsc:clean-fake": "rm -f node_modules/react-hyperscript-helpers",
        "test:tsc:cleanup": "npm run test:tsc:clean-fake && rm test/type-definitions.js",
        "test:tsc:compile": "tsc test/type-definitions.ts --module commonjs",
        "test:tsc:fake-install": "npm run test:tsc:clean-fake && ln -s .. node_modules/react-hyperscript-helpers"
    },
    "typings": "./lib/index.d.ts",
    "version": "1.2.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
