# npmtest-git-hooks

#### basic test coverage for  git-hooks (v1.1.8)  [![npm package](https://img.shields.io/npm/v/npmtest-git-hooks.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-git-hooks) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-git-hooks.svg)](https://travis-ci.org/npmtest/node-npmtest-git-hooks)

#### A tool to manage project Git hooks

[![NPM](https://nodei.co/npm/git-hooks.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/git-hooks)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-git-hooks/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-git-hooks/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-git-hooks/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-git-hooks/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-git-hooks/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-git-hooks/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-git-hooks/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-git-hooks/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-git-hooks/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-git-hooks/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-git-hooks/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-git-hooks/build/test-report.html](https://npmtest.github.io/node-npmtest-git-hooks/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-git-hooks/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-git-hooks/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-git-hooks/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-git-hooks/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-git-hooks/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-git-hooks/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-git-hooks/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-git-hooks/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "git-hooks",
    "description": "A tool to manage project Git hooks",
    "author": "Alexander Tarmolov <tarmolov@gmail.com>",
    "version": "1.1.8",
    "repository": "https://github.com/tarmolov/git-hooks-js",
    "contributors": [
        "Alexander Tarmolov <tarmolov@gmail.com> (http://tarmolov.ru/)",
        "Denis Khananein <i@zloylos.me> (http://zloy.me/)",
        "Ikonnikov Konstantin"
    ],
    "keywords": [
        "git",
        "hooks",
        "hook",
        "lint",
        "test",
        "development",
        "applypatch-msg",
        "commit-msg",
        "post-applypatch",
        "post-checkout",
        "post-commit",
        "post-merge",
        "post-receive",
        "pre-applypatch",
        "pre-auto-gc",
        "pre-commit",
        "pre-push",
        "pre-rebase",
        "pre-receive",
        "prepare-commit-msg"
    ],
    "engines": {
        "node": ">=0.8.x"
    },
    "engine-strict": true,
    "scripts": {
        "postinstall": "./bin/git-hooks --install",
        "preuninstall": "./bin/git-hooks --uninstall",
        "test": "jscs . && jshint . && mocha --reporter spec --recursive tests",
        "coverage": "istanbul cover _mocha --recursive tests"
    },
    "main": "lib/git-hooks",
    "files": [
        "bin",
        "examples",
        "lib"
    ],
    "devDependencies": {
        "chai": "2.3.0",
        "istanbul": "0.3.17",
        "jscs": "1.13.1",
        "jshint": "2.8.0",
        "mocha": "2.2.5"
    },
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
