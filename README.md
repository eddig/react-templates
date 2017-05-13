 React templates
## What we need
### Basic
- `webpack` for creating bundles from modules
- `babel-core` for transpliting js code into js code that most of web browsers understand
  - `babel-preset-es2015` for transpliting modern ES6 features (const, arrow functions, rest, spread, and etc)
  - `babel-preset-react` for transpliting JSX syntax (`<App />`)
  - `babel-loader` for integrating babel into webpack
- `react` for developing React application. This is a React framework
  - `react-dom` for connecting React app with the web browser DOM
### Hot Module Replacement
- `webpack-dev-server` for updating the web browser on changes in code
- `react-hot-loader` for supporting the partial update of React components
### HTML Template
- `html-webpack-plugin` for converting template into HTML
### File and Url source
- `file-loader` for coping static files that import from js (`import 'owl.png'`)
- `url-loader` if the file size less limit, it generate data url, otherwise use `file-loader` for coping file
### ESLint
- `eslint` for verify that the js code is valid and satisfy the rules
- `eslint-config-airbnb` set of the rules and configs from an Airbnb developers team
- `eslint-plugin-import` for resolving the `import/export` resources and modules
- `eslint-import-resolver-webpack` for using the webpack `resolve` config when resolving `import/export`
- `eslint-plugin-jsx-a11y` for checking accessibility in JSX
- `eslint-plugin-react` for checking JSX syntax
- `eslint-loader` for integrating eslint and webpack
### Flow
- `flow-bin` static type checker
- `babel-eslint` need for linting typed js code
