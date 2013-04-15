# spm-build

> the build tools for spmjs.org

-----

spm build is designed to build standard cmd modules.

**自定义构建，请不要用这个库，除非你清楚自己在做什么！**


## Standard Module

A standard module contains:

- a package.json
- a src directory
- a dist directory

```
package.json
src/
  module-name.js
dist/
  module-name.js   <-- will be created by spm-build
```

Learn more on [package.json](http://docs.spmjs.org/en/package).


## Install

Install spm-build with npm:

    $ npm install spm-build -g


## API

```
var builder = require('spm-build')
```

### builder.loadTasks()

It will load all tasks of the default build. Including:

- grunt-cmd-transport
- grunt-cmd-concat
- grunt-contrib-uglify
- grunt-contrib-copy
- grunt-contrib-cssmin
- grunt-contrib-clean
- spm-install
- spm-newline
