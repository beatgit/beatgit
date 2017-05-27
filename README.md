
| License | Source | &#8212;&raquo; | [Website](https://github.com/beatgit/beatgit/blob/master/Projects/2017_05-Website/main.sh) | [npm](https://github.com/npm/npm) |
| :---: | :---: | :---: | :---: | :---: |
| [FPL](https://opensource.org/licenses/FPL-1.0.0) | [github.com/beatgit/beatgit](https://github.com/beatgit/beatgit) | [![CircleCI](https://circleci.com/gh/beatgit/beatgit.svg?style=svg)](https://circleci.com/gh/beatgit/beatgit) | [beatgit.github.io/beatgit](https://beatgit.github.io/beatgit) | `beatgit`

beatgit
=======

A Bash and [NodeJS](https://nodejs.org/) Toolchain that helps you Leverage [git](https://git-scm.com/) at a more Abstract Level for a Seamless Workflow with Others.

Usage
-----

### Start Your Own Node

```javascript
require("beatgit").rise({
    "pkey": "<NodeJS compatible Private Key>",
    "attach": "github.com/${GITHUB_USER}/${GITHUB_REPOSITORY}"
}).then(function (TRUNK) {

    // trunk.id ~ Public Globally Unique ID (Public Key based)
    // trunk.connect ~ Abstract Object to handle Communication
    // trunk.fs ~ Globally Distributed Encrypted Filesystem
    // trunk.workspace ~ Local Tools API

    return TRUNK.connect.send(
        "https://github.com/beatgit/beatgit.git",
        TRUNK.fs("${__DIRNAME__}")
    }).then(function () {

        return workspace.open("localhost:$(PORT)");
    });
}).catch(console.error);
```

Provenance
==========

Original Source Logic under [Free Public License](https://opensource.org/licenses/FPL-1.0.0) by [Christoph Dorn](http://christophdorn.com) since 2017.
