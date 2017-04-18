# npmtest-requestretry

#### test coverage for  [requestretry (v1.12.0)](https://github.com/FGRibreau/node-request-retry#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-requestretry.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-requestretry) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-requestretry.svg)](https://travis-ci.org/npmtest/node-npmtest-requestretry)

#### request-retry wrap nodejs request to retry http(s) requests in case of error

[![NPM](https://nodei.co/npm/requestretry.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/requestretry)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-requestretry/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-requestretry/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-requestretry/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-requestretry/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-requestretry/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-requestretry/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-requestretry/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-requestretry/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-requestretry/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-requestretry/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-requestretry/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-requestretry/build/test-report.html](https://npmtest.github.io/node-npmtest-requestretry/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-requestretry/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-requestretry/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-requestretry/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-requestretry/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-requestretry/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-requestretry/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-requestretry/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-requestretry/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Francois-Guillaume Ribreau",
        "url": "http://fgribreau.com"
    },
    "bugs": {
        "url": "https://github.com/FGRibreau/node-request-retry/issues"
    },
    "contributors": [
        {
            "name": "juliendangers"
        },
        {
            "name": "Osbert Orr"
        }
    ],
    "dependencies": {
        "extend": "^3.0.0",
        "lodash": "^4.15.0",
        "request": "^2.74.0",
        "when": "^3.7.7"
    },
    "description": "request-retry wrap nodejs request to retry http(s) requests in case of error",
    "devDependencies": {
        "bluebird": "^3.4.6",
        "chai": "^3.2.0",
        "conventional-changelog": "^1.1.0",
        "conventional-changelog-cli": "^1.2.0",
        "coveralls": "^2.11.12",
        "kew": "~0.7.0",
        "mocha": "^3.0.2",
        "nyc": "^8.1.0",
        "q": "~1.4.1",
        "rsvp": "^3.2.1",
        "sinon": "1.17.5",
        "updtr": "^0.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "7f10a2cd0edb7e43bf9a8b6cbfeda202fb320860",
        "tarball": "https://registry.npmjs.org/requestretry/-/requestretry-1.12.0.tgz"
    },
    "gitHead": "aef934cb31c0ecdffae069a5a84e5a3df526806f",
    "homepage": "https://github.com/FGRibreau/node-request-retry#readme",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "fgribreau"
        }
    ],
    "name": "requestretry",
    "nyc": {
        "exclude": [
            "node_modules",
            "dist",
            "coverage",
            "webpack.config.js",
            "test"
        ]
    },
    "optionalDependencies": {},
    "repository": {
        "url": "git+https://github.com/FGRibreau/node-request-retry.git"
    },
    "scripts": {
        "changelog": "conventional-changelog -i CHANGELOG.md -s -r 0",
        "changelog-git": "npm run changelog && git add CHANGELOG.md && git commit -m 'docs(changelog): updated' && git push origin master",
        "send-coverage": "cat ./coverage/lcov.info | coveralls",
        "test": "mocha -t 2000 -R spec $(find test -name '*.test.js')",
        "test-coverage": "nyc --all --statements=100 --lines=100 --functions=100 --branches=100 --check-coverage --reporter=lcov --reporter=cobertura --report-dir=coverage -- mocha -R spec -t 100000  $(find test -name '*.test.js')",
        "test-watch": "mocha -t 100000 -R min -w $(find test -name '*.test.js')",
        "update": "updtr"
    },
    "version": "1.12.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
