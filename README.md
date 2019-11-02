## GoBrBr Dependences

# Babel, Webpack

yarn add @babel/core @babel/preset-env @babel/preset-react webpack webpack-cli

# React, React DOM

yarn add react, react-dom

# Babel Config

preset-env, preset-react

# Webpack Config

entry:

    => path ( 'src', 'index.js' )

output:

    => path ( 'public' )
    => filename: 'bundle.js'

module:

    rules:
    
        test => '*.js',
        exclude => 'node_modules'
        use
            => loader: 'babel-loader' 
