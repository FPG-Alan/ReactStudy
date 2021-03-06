# `react-dom`

This package serves as the entry point of the DOM-related rendering paths. It is intended to be paired with the isomorphic React, which will be shipped as `react` to npm.

Dom相关的渲染器入口点, 旨在与同构React配合(也就是NPM的`react`包)



## Installation

```sh
npm install react react-dom
```

## Usage

### In the browser

```js
var React = require('react');
var ReactDOM = require('react-dom');

class MyComponent extends React.Component {
  render() {
    return <div>Hello World</div>;
  }
}

ReactDOM.render(<MyComponent />, node);
```

### On the server

```js
var React = require('react');
var ReactDOMServer = require('react-dom/server');

class MyComponent extends React.Component {
  render() {
    return <div>Hello World</div>;
  }
}

ReactDOMServer.renderToString(<MyComponent />);
```

## API

### `react-dom`

- `findDOMNode`
- `render`
- `unmountComponentAtNode`

### `react-dom/server`

- `renderToString`
- `renderToStaticMarkup`
