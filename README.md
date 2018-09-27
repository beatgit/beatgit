
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

```text
Free Public License 1.0.0

Permission to use, copy, modify, and/or distribute this software for any purpose with or 
without fee is hereby granted.

THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH REGARD TO 
THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS. IN NO EVENT 
SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR 
ANY DAMAGES WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION 
OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE 
USE OR PERFORMANCE OF THIS SOFTWARE.
```

> Well-crafted Contributions are Welcome.

**INTENDED USE:** The *Logic and Code contained within* forms a **Developer Tool** and is intended to operate as part of a *Web Software Development Toolchain* on which a *Production System* operates indirectly. It is **NOT INTENDED FOR USE IN HIGH-LOAD ENVIRONMENTS** as there is *little focus on Runtime Optimization* in order to *maximize API utility, compatibility and flexibility over time*.

If you need more than what is contained within, study the Code, understand the Logic, and build your own Runtime Optimized Implementation that is API Compatible and share it with others who follow the *Logic and API Contract* specified within. This Community of Users will likely want to use Your Work in their own *Software Development Toolchains*.
