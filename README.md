# NPM GROOVY LINT

[![Version](https://img.shields.io/npm/v/npm-groovy-lint.svg)](https://npmjs.org/package/npm-groovy-lint)
[![Downloads/week](https://img.shields.io/npm/dw/npm-groovy-lint.svg)](https://npmjs.org/package/npm-groovy-lint) 
[![GitHub contributors](https://img.shields.io/github/contributors/nvuillam/npm-groovy-lint.svg)](https://gitHub.com/nvuillam/npm-groovy-lint/graphs/contributors/)
[![GitHub stars](https://img.shields.io/github/stars/nvuillam/npm-groovy-lint?style=social&label=Star&maxAge=2592000)](https://GitHub.com/nvuillam/npm-groovy-lint/stargazers/)
[![License](https://img.shields.io/npm/l/npm-groovy-lint.svg)](https://github.com/nvuillam/npm-groovy-lint/blob/master/package.json) 
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)
[![Say Thanks!](https://img.shields.io/badge/Say%20Thanks-!-1EAEDB.svg)](https://saythanks.io/to/nicolas.vuillamy@gmail.com)

Wrapper for excellent groovy linter [CodeNarc](http://codenarc.sourceforge.net/), using the great [jdeploy](https://github.com/shannah/jdeploy) and [Groovy](https://groovy-lang.org/)!

**npm-groovy-lint** allows you to run CodeNarc via command line without any installation issue

Easy to integrate in a CD/CI process (Jenkins Pipeline,CircleCI...)

# INSTALLATION

```
    npm install -g npm-groovy-lint
```

For advanced usage,  you may need to define [RuleSet file(s)](http://codenarc.sourceforge.net/codenarc-creating-rule.html)

You can use [this one](https://github.com/nvuillam/npm-groovy-lint/blob/master/src/dist/test/RuleSet-All.txt) as a starter

# USAGE

```
    npm-groovy-lint OPTIONS
```
See OPTIONS in [CodeNarc documentation](http://codenarc.sourceforge.net/codenarc-command-line.html)

# EXAMPLES

```
    $npm-groovy-lint -report="xml:MyGroovyLinterReport.xml"

    $npm-groovy-lint -basedir="src" -rulesetfiles="file:config/codenarc/RuleSet-all.txt" -title="MyGroovyLinterReport" -maxPriority1Violations=0 -report="html:MyGroovyLinterReport.html"
```

# CONTRIBUTE

Contributions are very welcome !

- Fork the repo and clone it on your computer
- Run `npm run test` to check your updates (jdeploy.js is manually updated by `npm run prepare-package` script)
- Once your code is ready, documented and linted, please make a pull request :)

