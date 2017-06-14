

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

var webpack = require('webpack');

const config = {
    entry: [
        './node_modules/jquery/dist/jquery.min.js'
    ],
    output: {
        filename: 'node_modules.js'
		},
    plugins: [

        new webpack.optimize.CommonsChunkPlugin({
            name: "commons",
            chunks: [
                "jquery"
            ],
};

module.exports = config
```


