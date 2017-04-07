# api documentation for  [gulp-strip-comments (v2.4.5)](https://github.com/RnbWd/gulp-strip-comments)  [![npm package](https://img.shields.io/npm/v/npmdoc-gulp-strip-comments.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-gulp-strip-comments) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-strip-comments.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-strip-comments)
#### Strip comments from code

[![NPM](https://nodei.co/npm/gulp-strip-comments.png?downloads=true)](https://www.npmjs.com/package/gulp-strip-comments)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-strip-comments_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-strip-comments/build/apidoc.html)

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
            "name": "rnbwd",
            "email": "dwisner6@gmail.com"
        },
        {
            "name": "vitaly.tomilov",
            "email": "vitaly.tomilov@gmail.com"
        }
    ],
    "name": "gulp-strip-comments",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-strip-comments](#apidoc.module.gulp-strip-comments)
1.  [function <span class="apidocSignatureSpan">gulp-strip-comments.</span>html (options)](#apidoc.element.gulp-strip-comments.html)
1.  [function <span class="apidocSignatureSpan">gulp-strip-comments.</span>text (options)](#apidoc.element.gulp-strip-comments.text)



# <a name="apidoc.module.gulp-strip-comments"></a>[module gulp-strip-comments](#apidoc.module.gulp-strip-comments)

#### <a name="apidoc.element.gulp-strip-comments.html"></a>[function <span class="apidocSignatureSpan">gulp-strip-comments.</span>html (options)](#apidoc.element.gulp-strip-comments.html)
- description and source-code
```javascript
html = function (options) {
    return main(options, decomment.html);
}
```
- example usage
```shell
...

Unlike the default **strip** method, it instructs the library that 'text' is not a JSON, JavaScript or HTML, rather a plain text
 that needs no parsing or validation, only to remove '//' and '/**/' comments from it according to the 'options'.

This method is good for any text file that uses syntax '//' and '/**/' for comments, such as: '.CSS', '.CPP', '.H', etc.

Please note that while the same rules apply for the text blocks ('''', '""' and \'\'), you should not use this method for JSON or
 JavaScript, as it can break your regular expressions.

### [strip.html(options)](https://github.com/vitaly-t/decomment#decommenthtmlhtml-options--string)

Unlike the default **strip** method, it instructs the library not to parse
or validate the input in any way, rather assume it to be HTML, and remove all
'<!-- comment -->' entries from it according to the 'options'.

### [strip.getEOL()](https://github.com/vitaly-t/decomment#decommentgeteoltext--string)
...
```

#### <a name="apidoc.element.gulp-strip-comments.text"></a>[function <span class="apidocSignatureSpan">gulp-strip-comments.</span>text (options)](#apidoc.element.gulp-strip-comments.text)
- description and source-code
```javascript
text = function (options) {
    return main(options, decomment.text);
}
```
- example usage
```shell
...
##### options.trim ⇒ Boolean

* 'false (default)' - do not trim comments
* 'true' - remove empty lines that follow removed full-line comments

NOTE: This option has no effect when option 'space' is enabled.

### [strip.text(options)](https://github.com/vitaly-t/decomment#decommenttexttext-options--string)

Unlike the default **strip** method, it instructs the library that 'text' is not a JSON, JavaScript or HTML, rather a plain text
 that needs no parsing or validation, only to remove '//' and '/**/' comments from it according to the 'options'.

This method is good for any text file that uses syntax '//' and '/**/' for comments, such as: '.CSS', '.CPP', '.H', etc.

Please note that while the same rules apply for the text blocks ('''', '""' and \'\'), you should not use this method for JSON or
 JavaScript, as it can break your regular expressions.
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
