# webpack-clean-plugin
A Webpack plugin for removing files and folders.

[![Build Status][travis-image]][travis-url]

## Installation
``
npm install webpack-clean-plugin --save-dev
``

## Example Webpack Config

`` javascript
var WebpackCleanPlugin = require('webpack-clean-plugin');

module.exports = {
    plugins: [
        new WebpackCleanPlugin({
            on: "emit",
            path: ['./static', './build']
        })
    ]
}
```

#####on
One of Webpack build steps. Such as `emit` `compilce` and so on.
``javascript
emit
```

#####path
The Array of file and dictory or just a string.
``javascript
['./static', './build'] or './build'
```

