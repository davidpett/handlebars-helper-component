# {{component}} [![NPM version](https://badge.fury.io/js/handlebars-helper-component.png)](http://badge.fury.io/js/handlebars-helper-component)

> Handlebars helper, alternative to built-in partials. Like Assemble itself, this helper will automatically determine the correct context to use, or a context may be explicitly passed in as a second parameter.

This helper was designed for usage with [Assemble](https://assemble.io), initially as a response to [this question on StackOverflow](http://stackoverflow.com/a/20854630/1267639). Feel free to fork it and customize it for your own needs.

If you find a bug or have a feature request, [please create an issue](https://github.com/helpers/handlebars-helper-component/issues).

## Installation
Use [npm](npmjs.org) to install the package: `npm i handlebars-helper-component`.

### Register the helper

The easiest way to register the helper with [Assemble](https://github.com/assemble/assemble) is to add the module to `devDependencies` and `keywords` in your project's package.json:

```json
{
  "devDependencies": {
    "handlebars-helper-component": "*"
  },
  "keywords": [
    "handlebars-helper-component"
  ]
}
```

Alternatively, to register the helper explicitly in the Gruntfile:

```javascript
grunt.initConfig({
  assemble: {
    options: {
      // the 'handlebars-helper-component' npm module must also be listed in
      // devDependencies for assemble to automatically resolve the helper
      helpers: ['handlebars-helper-component', 'foo/*.js']
    },
    files: {
      'dist/': ['src/templates/*.hbs']
    }
  }
});
```
Visit [assemble.io/plugins](http:/assemble.io/plugins/) for more information about [Assemble](http:/assemble.io/) plugins.
