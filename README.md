## GoBrBr Dependences

### Babel, Webpack

yarn add @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli

## React, React DOM

yarn add react, react-dom

## Babel Config

    presets: [
            "@babel/preset-env",
            "@babel/preset-react"
        ],

## Webpack Config

entry: 

    path.resolve(__dirname, 'src', 'index.js'),

output:

    {
        path: path.resolve(__dirname, 'public'),
        filename: 'bundle.js'
    },

module: 

    { 
        rules: [
            {
                test: /\.js$/,
                exclude: /node_modules/,
                use: {
                    loader: 'babel-loader'
                }
            }
        ]
    }
