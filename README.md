![BaseWeb](http://f.cl.ly/items/201U3Y1g0c2M1u1Z3i0n/baseweb-banner.png "BaseWeb — A fresh front-end development framework.")

Currently v1.2.0

## About
BaseWeb is a SCSS front-end development framework built to make working on web based projects more enjoyable. It&#39;s focused on keeping your projects simple, organized and responsive.

### Upcoming Features
The main features being worked on right now are blocks. The following list of blocks are currently on the production list:

* Modals
* Tooltips
* Dropdowns
* Menus
* Pagination
* Tabs

## Documentation
Documentation is currently being worked on and you can view them if you clone or download the repo. There will also be an online version at [http://getbaseweb.com/](http://getbaseweb.com/).

### Upcoming Features
Upcoming features and updates to BaseWeb documentation:

* Add some form of change or development log, similar to [Cargo Devlog](http://cargocollective.com/devlog).
* Add a blog to highlight new features and post tutorials.
* Incorporate [markdown-it](https://www.npmjs.com/package/markdown-it) node module for use with the devlog, blog and readme.
* Setup auto deployment for docs to [http://getbaseweb.com/](http://getbaseweb.com/).

## Build Scripts

BaseWeb uses [Node](https://nodejs.org/), [Jake](http://jakejs.com/) and [Jake-Builds](https://github.com/sebnitu/jake-builds) for building both the source and docs. For more information on how to update build scripts using this stack, make sure to checkout [Jake-Builds](https://github.com/sebnitu/jake-builds).

### Node Packages
Run `npm install` to install required node modules for build scripts. This is the following node stack used to build BaseWeb assets and documentation files:

| Node Modules   | Versions   | Description |
|----------------|------------|-------------|
| `jake`         | `8.0.12`   | The JavaScript build tool for Node.js |
| `node-watch`   | `0.3.4`    | Used in handling the watch task |
| `node-sass`    | `2.1.1`    | Used for compiling and minifying src and doc CSS from SCSS files |
| `uglify-js`    | `2.4.19`   | Used to compile and minify our JavaScript files |
| `imagemin`     | `3.1.0`    | Used to optimize our image files |
| `mustache`     | `2.0.0`    | Used to build our HTML files for docs, examples and readme |

*Keep in mind that if you use the imagemin module, [Jpegtran](http://jpegclub.org/jpegtran/) should be installed globally. You can install it with [Homebrew](http://brew.sh/) using: `brew install jpeg`*

### Jake Tasks
To see the full list of available Jake tasks for a project, use `jake -ls`. The following tasks are available for building BaseWeb and related files:

| Jake Tasks            | Description                                          |
|-----------------------|------------------------------------------------------|
| `jake build:scss`     | Compiles and minifies SCSS                           |
| `jake build:js`       | Compiles and minifies JavaScript                     |
| `jake build:img`      | Optimizes images                                     |
| `jake build:docs`     | Build documentation                                  |
| `jake build:examples` | Build examples                                       |
| `jake watch`          | Watch for change to files and rebuild if they change |

## Copyright and License

BaseWeb and BaseWeb documentation copyright (c) 2015 [Sebastian Nitu](http://sebnitu.com). BaseWeb is released under the [MIT license](https://github.com/sebnitu/BaseWeb/blob/master/LICENSE) and BaseWeb documentation is released under [Creative Commons](https://github.com/sebnitu/BaseWeb/blob/master/docs/LICENSE).