# grunt-jscrush

> Grunt task to jscrush a file and save its result. (jscrush via http://www.iteral.com/jscrush/)

## Getting Started
This plugin requires Grunt `~0.4.1`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-jscrush --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-jscrush');
```

## The "jscrush" task

### Overview
In your project's Gruntfile, add a section named `jscrush` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  jscrush: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

### Options

It works without any options. If you got suggestions for options tell me @makepanic :)

### Usage Examples

#### Default Options
In this example, the default options are used to crush a file conaining a random color generation method from http://paulirish.com/2009/random-hex-color-code-snippets/ . 
It takes the content from 'src/rndm-color.js' saves the result to 'dest/crush.min.js'.

```js
grunt.initConfig({
  jscrush: {
    options: {},
    files: {
      'dest/crush.min.js': ['src/rndm-color.js'],
    },
  },
})
```

## Release History
0.0.1 initial release
