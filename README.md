# grunt-trimtrailingspaces

Trim trailing spaces from each line of the selected files

## Getting Started

Add this to your project's `Gruntfile.js` gruntfile:
```js
grunt.loadNpmTasks('grunt-trimtrailingspaces');
```

Then add "grunt-trimtrailingspaces" to your package.json dependencies. This can be done with:
```js
npm install grunt-trimtrailingspaces --save-dev
```
Or by manually editing the "package.json" by adding the following line inside `devDependencies` object:
```js
  "grunt-trimtrailingspaces": "~0.1.0"
```

Later on it would be possible to install the plugin with the command `npm install`

It can be updated with the command `npm update`, in case there is a newer version in the NPM repository.

The name to use in your own task definitions is `trimtrailingspaces`.

## Documentation

Add an entry to your "Gruntfile.js", within the `initConfig` object, which will define the 
files of which will the trailing spaces to be removed.

```js
  ...

  trimtrailingspaces: {
    extensions: ['js', 'css', 'html'],
    directories: ['.', 'templates', 'public_html/js', 'public_html/css'],
    encoding: 'utf8'
  }

  ...
```

To run it:

```js
grunt trimtrailingspaces
```

## Dependencies

This module depends only on one 3rd party module, namely [string.js](http://stringjs.com/).


## License
Copyright (c) 2013 Juga Paazmaya <olavic@gmail.com>
Licensed under the MIT license.