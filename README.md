# React Webpack Babel

> notes on [this](https://www.valentinog.com/blog/react-webpack-babel/) article

# Setting up webpack

- webpack config in `webpack.config.js`

# Setting up babel

- transforming code from ES6 to browser friendly JS is called transpiling.
- Webpack can't transpile ES6 to to ES5 but it has the concept of loaders
- loaders are like transformers, they take something as input and produces an output
- babel-loader is the transformer for ES6 ⇒ older JS
- babel-loader makes use of Babel
- Babel must be configured (`.babelrc`)to use presets:
    - babel preset env (ES6 ⇒ ES5)
    - babel preset react (JSX etc ⇒ JS)
- can also add in plugins like [class properties](https://babeljs.io/docs/en/babel-plugin-proposal-class-properties)

# Writing React components

- basic react stuff

# The HTML webpack plugin

- without this webpack will just create a bundle.js. We want this bundle.js to be linked to a html file.
- need to load html files and also want to map our file in src to a index.html file in dist. This requires 2 modules:
    - `npm i html-webpack-plugin html-loader --save-dev`

# Webpack dev server

- can use webpack dev server cli to watch for changes and server files