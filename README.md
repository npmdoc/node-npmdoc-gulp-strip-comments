# npmdoc-gulp-strip-comments

#### api documentation for  [gulp-strip-comments (v2.4.5)](https://github.com/RnbWd/gulp-strip-comments)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-strip-comments.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-strip-comments) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-strip-comments.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-strip-comments)

#### Strip comments from code

[![NPM](https://nodei.co/npm/gulp-strip-comments.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/gulp-strip-comments)

- [https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "authors": [
        "David Wisner <dwisner6@gmail.com>",
        "Vitaly Tomilov <vitaly.tomilov@gmail.com>"
    ],
    "bugs": {
        "url": "https://github.com/RnbWd/gulp-strip-comments/issues"
    },
    "dependencies": {
        "decomment": "^0.8.7",
        "gulp-util": "^3.0.8",
        "through2": "^2.0.1"
    },
    "description": "Strip comments from code",
    "devDependencies": {
        "coveralls": "^2.11.9",
        "istanbul": "^0.4.3",
        "jasmine-node": "^1.14.5"
    },
    "directories": {},
    "dist": {
        "shasum": "76a5587078e6a03332925a452d2b744c1bb6cda5",
        "tarball": "https://registry.npmjs.org/gulp-strip-comments/-/gulp-strip-comments-2.4.5.tgz"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "ea9518b1d8ba5a5c05f05a9ebe4ccfe36e4a548f",
    "homepage": "https://github.com/RnbWd/gulp-strip-comments",
    "keywords": [
        "strip comments",
        "gulpplugin",
        "strip",
        "gulp",
        "comment",
        "decomment",
        "remove",
        "clean",
        "stream",
        "minimize",
        "reduce",
        "remove",
        "comments"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "rnbwd"
        },
        {
            "name": "vitaly.tomilov"
        }
    ],
    "name": "gulp-strip-comments",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/RnbWd/gulp-strip-comments.git"
    },
    "scripts": {
        "coverage": "istanbul cover ./node_modules/jasmine-node/bin/jasmine-node test",
        "test": "jasmine-node test",
        "travis": "istanbul cover ./node_modules/jasmine-node/bin/jasmine-node test --captureExceptions && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage"
    },
    "version": "2.4.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
