# Workflow: Front-End with Gulp & Nunjucks

Automated workflow for front-end dev, using [Gulp.js](http://gulpjs.com/) task runner.

This is version 2 and supercedes this workflow [repo](https://github.com/cubiio/workflow).

Version 2 includes two key changes:

* Add Nunjucks template management
* Simplified Gulp file (no folder structure) 


## How to scaffold a project

### Clone files and folders

Clone this git repo into the new project.

```$ git clone https://github.com/cubiio/workflow_frontend_gn```

Change the remote url to the new project remote url.

```
$ git remote remove origin
$ git remote add origin url-to-new-git-repo
```

If/when moving top level folder `workflow`, take care to also move `.hidden` files as well.

### Install dependencies

To install packages/dependencies:

| File | Command run|  
| --- | --- |  
|`package.json` | `npm install`|  
|`bower.json` | `bower install`| 


#### Check all dependencies are installed. 

For example, `npm rsyncwrapper` is not a Gulp dependency and may not be installed.



```
// gulpfile.js
const rsync = require('rsyncwrapper').rsync;

// terminal
$ npm install --save-dev rsyncwrapper
```

### Update npm dependencies

Check if packages need updating:
```npm outdated```

To update:

```
$ npm update
// or
$ npm-check -u
```

### Update Bower dependencies

Check what is installed and if outdated:

```
$ bower list
```

To update:

```
$ bower-update
```




