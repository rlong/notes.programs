


setup
=====




project
-------


```
npm install --save-dev webpack
```


config
------

create a file `webpack.config.js`:
```
const config = {
    entry: [
        './node_modules/jquery/dist/jquery.min.js'
    ],
    output: {
        filename: 'node_modules.js'
    }
};

module.exports = config
```


